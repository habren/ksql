# KSQL Documentation

| Overview | [Installation](/docs/installation) | [Quick Start Guide](/docs/quickstart/) | [Concepts](/docs/concepts.md) | [Syntax Reference](/docs/syntax-reference.md) | [Examples](/docs/examples.md) | [FAQ](/docs/faq.md)  |
|----------|--------------|-------------|------------------|------------------|------------------|------------------|

> *Important: This release is a *developer preview* and is free and open-source from Confluent under the Apache 2.0 license.*

# Overview
KSQL is an open source streaming SQL engine that implements continuous, interactive queries against Apache Kafka™. It allows you to query, read, write, and process data in Apache Kafka in real-time, at scale using SQL commands. KSQL interacts directly with the [Kafka Streams API](http://docs.confluent.io/current/streams/concepts.html), removing the requirement of building a Java app. 

### Use cases
Common KSQL use cases are:

- Fraud detection - identify and act on out of the ordinary data to provide real-time awareness. 
- Personalization - create real-time experiences and insight for end users driven by data. 
- Notifications - build custom alerts and messages based on real-time data. 
- Real-time Analytics - power real-time dashboards to understand what’s happening as it does. 
- Sensor data and IoT - understand and deliver sensor data how and where it needs to be. 
- Customer 360 - provide a clear, real-time understanding of your customers across every interaction.

KSQL lowers the barriers for using real-time data in your applications. It is powered by a scalable streaming platform without the learning curve or additional management complexity of other stream processing solutions.

### Terminology 
When using KSQL, the following terminology is used.

#### Stream
A stream is an unbounded sequence of structured values that are stored in a Kafka topic. The structure of the values is specified in a schema. In Kafka streams vocabulary, a KSQL stream is a [KStream](http://docs.confluent.io/current/streams/concepts.html?highlight=kstream#kstream) plus a schema. 

#### Table
A table in KSQL is finite, where the bounds are defined by the size of the key space. The key space is an evolving collection of structured values, where the structure of the values is specified in a schema. These values are stored in a changelog topic in Kafka. In Kafka Streams vocabulary, a KSQL table is a [KTable](http://docs.confluent.io/current/streams/concepts.html?highlight=ktable#ktable) plus a schema.

#### Topic
A topic is a category or feed name where records are published. For more information, see the [Apache Kafka documentation](https://kafka.apache.org/documentation/#intro_topics).

## Modes of operation

You can use KSQL in standalone, client-server, application, and embedded modes. See this [document](/docs/concepts/) for more information.

## Getting Started

* Beginners: Try the [interactive quick start](/docs/quickstart/). The quick start configures a single instance in a lightweight Docker container or in a Kafka cluster. It demonstrates a simple workflow using KSQL to write streaming queries against data in Kafka.
* Advanced users: Try the [end-to-end KSQL demo](https://github.com/confluentinc/ksql).

