# stealify-gitlab
A Gitlab Distribution that is using the Stealify Software Encapsulation Framework

# Gitlab
Gitlab is a good Software Project to start with it is relativ essential for building good software so lets investigate 

it is composed out of many software products and servers exposing the gitlab api's and interfaces. All this software is coded in diffrent languages. So this is defacto a Project that is Polyglot so Stealify simply is the next step.

## Goals
- Replace the gitlab omnibus release we will use the code name gitlab graal to hornor the guys at oracle that did the amazing job with the graal framework
- https://about.gitlab.com/blog/2018/10/29/why-we-use-rails-to-build-gitlab/ should get referenced and how we overcome the dilema :)
- Reduce traffic and storage overhead https://docs.gitlab.com/omnibus/package-information/defaults.html
  - https://github.com/omniauth/omniauth - ruby
  - Redis - apache ignite
  - PostgreSQL - apache ignite
  - NGINX - vertx
  - consul - apache ignite - atomx
  - gitlab geo - apache ignite
  - fs - apache ignite
  - logging - apache ignite
  - Jaeger - OpenTelemetry + apache ignite
  
  ![me](https://raw.githubusercontent.com/stealify/stealify-gitlab/master/gitlab.svg?sanitize=true)


## jaeger
OpenTelemetry
On 28-May-2019, the OpenTracing and OpenCensus projects announced their intention to merge into a new CNCF project called OpenTelemetry. The Jaeger and OpenTelemetry projects have different goals. OpenTelemetry aims to provide APIs and SDKs in multiple languages to allow applications to export various telemetry data out of the process, to any number of metrics and tracing backends. The Jaeger project is primarily the tracing backend that receives tracing telemetry data and provides processing, aggregation, data mining, and visualizations of that data. The Jaeger client libraries do overlap with OpenTelemetry in functionality. OpenTelemetry will natively support Jaeger as a tracing backend and eventually might make Jaeger native clients unnecessary. For more information please refer to a blog post Jaeger and OpenTelemetry.

Multiple storage backends
Jaeger supports two popular open source NoSQL databases as trace storage backends: Cassandra and Elasticsearch. There is also embedded database support using Badger. There are ongoing community experiments using other databases, such as ScyllaDB, InfluxDB, Amazon DynamoDB. Jaeger also ships with a simple in-memory storage for testing setups.

OpenTelemtry is integrate into Stealify by default
