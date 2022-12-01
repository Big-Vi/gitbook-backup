---
description: How to access Memphis after installation
---

# 2 - Access

## How to configure public access to Memphis

### <mark style="color:purple;">Localhost</mark>

Run

```
kubectl port-forward service/memphis-cluster 6666:6666 9000:9000 7770:7770 --namespace memphis > /dev/null &
```

Credentials

```
UI/CLI root username - root
UI/CLI root Password - kubectl get secret memphis-creds -n memphis -o jsonpath="{.data.ROOT_PASSWORD}" | base64 --decode
```

[http://localhost:9000](http://localhost:9000)

{% hint style="info" %}
If a simpler localhost connection is needed for more services, use [Kubefwd](https://kubefwd.com/).
{% endhint %}

### <mark style="color:purple;">Production</mark>

#### Step 1: Deploy self-signed cert

1. Install [mkcert](https://github.com/FiloSottile/mkcert) and generate a certificate

{% code lineNumbers="true" %}
```
mkcert -install
mkcert -cert-file memphis.pem -key-file memphis-key.pem "*.memphis.dev"
```
{% endcode %}

2\. Create a secret with the new cert and private key

```
kubectl create secret generic tls-secret --from-file=memphis.pem --from-file=memphis-key.pem -n memphis
```

3\. Reinstall Memphis with the cert

```
helm install my-memphis memphis --set analytics='false',cluster.enabled="true",websocket.tls.cert="memphis.pem",websocket.tls.key="memphis-key.pem",websocket.tls.secret.name="tls-secret" --create-namespace --namespace memphis --wait
```

#### Step 2: Create the LB

1. Run the following

{% code lineNumbers="true" %}
```
kubectl expose service memphis-cluster --port=9000,7770  --name=external-service --type=LoadBalancer -n memphis
kubectl -n memphis-sandbox patch svc external-service -p '{"spec":{"ports": [{"port": 443,"name":"https","targetPort": 9000}]}}'
```
{% endcode %}

2\. Add the certificate to the LB as well