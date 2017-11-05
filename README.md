# SMACK Stack

* Big-Data platform
* Realtime analytics
* Fast-Data solution
* Data processing pipeline architecture
* Ingestion, aggregation, analysis
* All are Apache projects (except Akka)
* Highly available, resilient, and distributed

## Spark
<p align="left">
<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/spark.png?raw=true" alt="Spark">

* Spark batch jobs
    * Easy to use
* Spark Streaming uses micro batches to address realtime usecases
    * compare to real time processing like Apache Flink
* Spark SQL: Sql like descriptive interface

</p>

## Mesos

<p align="left">
<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/mesos.png?raw=true" alt="Mesos">

* Scheduling framework: Providing ressources for applications and jobs
* Hardware abstraction
* distributes workload across the cluster
* Orchestrate components and manage ressources
* DC/OS: DataCenter Operating System
    * using mesos
    * Microservices and Container

</p>

## Akka

<p align="left">
<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/akka.png?raw=true" alt="Akka">

* implementation of the actor framework
* allows to create message-driven applications
* actor based concurrency
* fault-tolerant
* commonly used with scala, but java is possible
* `akka-http` for REST services

</p>

## Cassandra

<p align="left">
<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/cassandra.png?raw=true" alt="Cassandra">

* NoSQL
* Wide Column Store
* linear, horizontal scaling
* No single point of failure
* Performance
* Connectors for spark and mesos
* Possible to be used accross multiple data centers

</p>

## Kafka

<p align="left">
<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/kafka.png?raw=true" alt="Kafka">

* Distributed messaging system
* high availability, high throughput, low latency
* using a distributed commit log internally

</p>

