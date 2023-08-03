---
description: What is Memphis.dev
cover: .gitbook/assets/Banner- Memphis.dev streaming .jpg
coverY: 0
---

# Introduction

We are happy to announce Memphis #1 hackathon [#SaveZakar](https://memphis.dev/blog/save-zakar-hackathon/)!📣 📣 📣&#x20;

<figure><img src=".gitbook/assets/Hackathon banner.png" alt=""><figcaption></figcaption></figure>

For more information and to sign up, enter the [#SaveZaker hackathon](https://memphis.dev/blog/save-zakar-hackathon/).

## The challenges

When your application requires a message broker or a queue,\
Implementing one will require you to -

* Build a dead-letter queue, create observability, and a retry mechanism
* Build a scalable environment
* Create client wrappers
* Tag events to achieve multi-tenancy
* Enforce schemas and handle transformations
* Handle back pressure. Client or queue side
* Configure monitoring and real-time alerts
* Create a cloud-agnostic implementation
* Create config alignment between production to a dev environment
* Spent weeks and months learning the internals through archival documentation, ebooks, and courses
* Onboard your developers

And the list continues...

## So, What is Memphis.dev?

Memphis.dev is more than a broker. It's a new streaming stack. \
\
It significantly accelerates the development of real-time applications that require a streaming platform with high throughput, low latency, easy troubleshooting, fast time-to-value,\
minimal platform operations, and all the observability you can think of.

### The four main components of Memphis

1. Memphis Broker. A distributed engine, which also acts as the primary storage layer for produced events or data.
2. Memphis Functions. Developer-first serverless stream processing to transform and enrich ingested events on-the-fly.
3. Schemaverse. Schema management and enforcement tool built within Memphis to help users increase data quality and avoid upstream breaks.
4. Memphis Connect. A modular framework to enable fast pull and push of data to and from different sources and destinations.

### **Core** characteristics**.**

1. Reliability - Queues and brokers are a mission-critical component in the modern application architecture and should be highly available and stable as possible.
2. Performance and Efficiency - Provide great performance while maintaining efficient resource consumption.
3. Developer Experience - Enable rapid development and ultra-short time-to-production.
4. Observability - Increase observability, integrations with 3rd-party monitoring tools, real-time notifications, stream lineage, and therefore troubleshooting time reduction.

## Walkthrough

{% embed url="https://app.storylane.io/share/upo0paxdvynz" %}

## High-level diagram

<figure><img src=".gitbook/assets/overview (1).jpeg" alt=""><figcaption></figcaption></figure>

## Use cases examples

* Async task management
* Real-time streaming pipelines
* Data ingestion
* Async communication between services on k8s
* Queuing
* Multiple destinations to a single message
* Ingest Grafana loki logs
* Stream video frames
