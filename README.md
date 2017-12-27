# What’s TRON? [![Build Status](https://travis-ci.org/tronprotocol/java-tron.svg?branch=feature%2Fconsensus)](https://travis-ci.org/tronprotocol/java-tron) [![GitHub last commit](https://img.shields.io/github/last-commit/tronprotocol/java-tron.svg)](https://github.com/tronprotocol/java-tron/commits/develop) [![GitHub issues](https://img.shields.io/github/issues/tronprotocol/java-tron.svg)](https://github.com/tronprotocol/java-tron/issues) [![license](https://img.shields.io/github/license/tronprotocol/java-tron.svg)](LICENSE)

TRON is a block chain-based decentralized smart protocol and an application development platform. It allows each user to freely publish, store and own contents and data, and in the decentralized autonomous form, decides an incentive mechanism and enables application developers and content creators through digital asset distribution, circulation and transaction, thus forming a decentralized content entertainment ecosystem.

TRON is a product of Web 4.0 and the decentralized internet of next generation.

# Quick Start

**Download and build**

```shell
> git clone https://github.com/tronprotocol/java-tron.git
> cd java-tron
> gradle build
```

**Import project to IDEA**

1. [File] -> [New] -> [Project from Existing Sources...]
2. Select java-tron/build.gradle
3. Dialog [Import Project from Gradle], confirm [Use auto-import] and [Use gradle wrapper task configuration] have been
 selected，then select Gradle JVM（JDK 1.8）and click [OK]

# Testing

- Install Kafka, create two topics (block and transaction)
- Adjust constant **DEFAULT_BOOTSTRAP_SERVERS** in ConsumerProperty.java file and ProducerProperty.java file to your Kafka's host（like：192.168.1.199:9092）
- IDEA: [Edit Configurations...] -> [Program arguments]: **--type server**
- Run Tron (server)
- IDEA: [Edit Configurations...] -> [Program arguments]: **--type normal**
- Run Tron (client)
- Execute `help` command on the client



