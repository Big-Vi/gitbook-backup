# Table of contents

## 👉 Getting Started

* [Step 1 - Installation](README.md)
* [Step 2 - Hello World](getting-started/2-hello-world.md)
* [Tutorials](getting-started/tutorials/README.md)
* [Use cases](getting-started/3-use-cases.md)
* [Public Case Studies](getting-started/public-case-studies.md)
* [How to contribute?](getting-started/how-to-contribute.md)
* [Roadmap](https://memphis.dev/roadmap)

## ⭐ Memphis

* [Overview](memphis/overview.md)
* [Architecture](memphis/architecture.md)
* [Key concepts](memphis/concepts/README.md)
  * [Message broker](memphis/concepts/message-broker.md)
  * [Station](memphis/concepts/station.md)
  * [Producer API](memphis/concepts/producer.md)
  * [Consumer API](memphis/concepts/consumer.md)
  * [Consumer Group](memphis/concepts/consumer-groups.md)
  * [Storage and Redundancy](memphis/concepts/storage-and-redundancy.md)
  * [Security/Authentication](memphis/concepts/security.md)
  * [Scaling](memphis/concepts/scaling.md)
  * [Ordering](memphis/concepts/ordering.md)
  * [Dead-letter Station (DLS)](dashboard-ui/troubleshooting/dead-letter.md)
  * [Delayed messages](memphis/key-concepts/delayed-messages.md)
  * [Idempotency (Duplicate processing)](memphis/concepts/idempotency.md)
  * [Failover Scenarios](memphis/concepts/failover-scenarios.md)
* [Schemaverse](memphis/schemaverse-schema-management/README.md)
  * [⭐ Getting started](memphis/schemaverse-schema-management/formats/README.md)
    * [Protobuf](memphis/schemaverse-schema-management/formats/protobuf.md)
    * [JSON Schema](memphis/schemaverse-schema-management/formats/json-schema.md)
    * [GraphQL](memphis/schemaverse-schema-management/formats/graphql.md)
    * [Avro](memphis/schemaverse-schema-management/formats/avro.md)
  * [Comparison](memphis/schemaverse-schema-management/comparison.md)
  * [KB](memphis/schemaverse-schema-management/kb.md)
* [Memphis configuration](memphis/memphis-configuration.md)
* [Benchmark](memphis/benchmark.md)
* [Comparisons](memphis/comparisons/README.md)
  * [NATS Jetstream vs Memphis](memphis/comparisons/nats-vs-memphis.md)
  * [RabbitMQ vs Memphis](memphis/comparisons/rabbitmq-vs-memphis.md)
  * [AWS SQS vs Memphis](memphis/comparisons/aws-sqs-vs-memphis.md)
  * [Apache Kafka vs Memphis](memphis/comparisons/apache-kafka-vs-memphis.md)
  * [Apache Pulsar vs Memphis](memphis/comparisons/apache-pulsar-vs-memphis.md)
  * [ZeroMQ vs Memphis](memphis/comparisons/zeromq-vs-memphis.md)
* [Privacy](memphis/privacy.md)

## ☁ Memphis cloud

* [Private beta](https://memphis.dev/cloud)

## 📦 Deployment

* [Terraform](deployment/cloud-deployment/README.md)
  * [Deploy on AWS](deployment/cloud-deployment/deploy-on-aws.md)
  * [Deploy on GCP](deployment/cloud-deployment/deploy-on-gcp.md)
  * [Deploy on DigitalOcean](deployment/cloud-deployment/deploy-on-digitalocean.md)
  * [Deploy on Azure](deployment/cloud-deployment/deploy-on-azure.md)
* [Kubernetes](deployment/kubernetes/README.md)
  * [1 - Installation](deployment/kubernetes/1-installation.md)
  * [2 - Access](deployment/kubernetes/2-access.md)
  * [3 - Upgrade](release-notes/how-to-upgrade.md)
* [Docker](deployment/docker-compose.md)
* [Production Best Practices](deployment/production-best-practices.md)

## SDKs and Protocols

* [REST (Webhook)](https://github.com/memphisdev/memphis-http-proxy)
* [Node.js / TypeScript / NestJS](https://github.com/memphisdev/memphis.js)
* [Go](https://github.com/memphisdev/memphis.go)
* [Python](https://github.com/memphisdev/memphis.py)
* [Kotlin](https://github.com/memphisdev/memphis.kt)
* [.NET](https://github.com/memphisdev/memphis.net)
* [Java](https://github.com/memphisdev/memphis.java)
* [NATS Jetstream](sdks-and-protocols/nats-jetstream/README.md)
* [Rust](sdks/rust.md)
* [Scala](sdks/scala.md)

## Dashboard (GUI)

* [General](dashboard-gui/general.md)
* [Signup](dashboard-gui/signup.md)
* [Login](dashboard-gui/login.md)
* [Overview](dashboard-gui/overview.md)
* [Stations](dashboard-gui/stations.md)
* [Users](dashboard-gui/users.md)
* [Profile](dashboard-gui/settings.md)

## 🔌 Integrations

* [Monitoring](integrations/monitoring/README.md)
  * [Elasticsearch Observability](integrations/monitoring/elasticsearch-observability.md)
  * [Datadog](integrations/monitoring/datadog.md)
  * [Grafana](integrations/monitoring/grafana.md)
* [Notifications](integrations/notifications/README.md)
  * [Slack](integrations/notifications/slack.md)
* [Storage](integrations/storage/README.md)
  * [Amazon S3](integrations/storage/amazon-s3.md)
* [Other platforms](integrations/other-platforms/README.md)
  * [PostHog](https://github.com/PostHog/posthog-memphisdev-app)
  * [Argo](integrations/other-platforms/argo-and-memphis.md)

## 🗒 Release notes

* [Releases](release-notes/releases/README.md)
  * [v1.0.2-stable](release-notes/releases/v1.0.2-stable.md)
  * [v1.0.1](release-notes/releases/v1.0.1.md)
  * [V1.0.0 - GA](release-notes/releases/v1.0.0-lts.md)
  * [v0.4.5 - beta](release-notes/releases/latest-v0.4.5-beta.md)
  * [v0.4.4 - beta](release-notes/releases/v0.4.4-beta.md)
  * [v0.4.3 - beta](release-notes/releases/v0.4.3-beta.md)
  * [v0.4.2 - beta](release-notes/releases/v0.4.2-beta.md)
  * [v0.4.1 - beta](release-notes/releases/v0.4.1-beta.md)
  * [v0.4.0 - beta](release-notes/releases/v0.4.0-beta.md)
  * [v0.3.6 - beta](release-notes/releases/v0.3.6-beta.md)
  * [v0.3.5 - beta](release-notes/releases/v0.3.5-beta.md)
  * [v0.3.0 - beta](release-notes/releases/v0.3.0-beta.md)
  * [v0.2.2 - beta](release-notes/releases/v0.2.2-beta.md)
  * [v0.2.1 - beta](release-notes/releases/v0.2.1-beta.md)
  * [v0.2.0 - beta](release-notes/releases/v0.2.0-beta.md)
  * [v0.1.0 - beta](release-notes/releases/v0.1.0-beta.md)
