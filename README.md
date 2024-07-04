[![Build Status](https://github.com/debezium/container-images/actions/workflows/image-builds-auth.yml/badge.svg?branch=main)](https://github.com/debezium/container-images/actions/workflows/image-builds-auth.yml)
[![License](http://img.shields.io/:license-mit-brightgreen.svg)](https://opensource.org/licenses/MIT)
[![Quay.io](https://img.shields.io/badge/quay.io-images-brightgreen)](https://quay.io/organization/debezium)

This repository contains the primary container images for Debezium, and they are automatically built and published on [Quay.io](https://quay.io/organization/debezium).

# What is Debezium?

Debezium is a distributed platform that turns your existing databases into event streams, so applications can quickly react to each row-level change in the databases. Debezium is built on top of Kafka and provides Kafka Connect compatible connectors that monitor specific database management systems. Debezium records the history of data changes in Kafka logs, so your application can be stopped and restarted at any time and can easily consume all of the events it missed while it was not running, ensuring that all events are processed correctly and completely.

Debezium is open source under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

# How to build

    cp ~/Documents/github/ibnummuhammad/kafka/clients/build/libs/kafka-clients-3.7.0.jar ~/Documents/github/ibnummuhammad/debezium-container-images/kafka/2.6/libs/kafka-clients-3.7.0.jar
    cp ~/Documents/github/ibnummuhammad/kafka/connect/api/build/libs/connect-api-3.7.0.jar ~/Documents/github/ibnummuhammad/debezium-container-images/kafka/2.6/libs/connect-api-3.7.0.jar
    cp ~/Documents/github/ibnummuhammad/kafka/connect/json/build/libs/connect-json-3.7.0.jar ~/Documents/github/ibnummuhammad/debezium-container-images/kafka/2.6/libs/connect-json-3.7.0.jar
    cp ~/Documents/github/ibnummuhammad/kafka/connect/runtime/build/libs/connect-runtime-3.7.0.jar ~/Documents/github/ibnummuhammad/debezium-container-images/kafka/2.6/libs/connect-runtime-3.7.0.jar
    cp ~/Documents/github/ibnummuhammad/kafka/connect/transforms/build/libs/connect-transforms-3.7.0.jar ~/Documents/github/ibnummuhammad/debezium-container-images/kafka/2.6/libs/connect-transforms-3.7.0.jar

    ./build-debezium.sh 2.6

# License

The Dockerfiles, scripts, and other files in this Git repository are licensed under the [MIT license](https://opensource.org/licenses/MIT). However, the resulting container images contain software licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html) and other licenses (see specific container images for details).

# Tutorial for running Debezium with Docker

We have a [tutorial](https://debezium.io/documentation/reference/tutorial.html) that walks you through running Debezium using Docker. Give it a go, and [let us know what you think](https://debezium.io/community/)!
