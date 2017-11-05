# SMACK Stack

* Collection of technologies that can be used to create a Big-Data platform.
* Realtime analytics
* Fast-Data solution
* Enable explorative data analysis
* Fast and simple deployment
* Acronym SMACK for Spark (Engine), Mesos (Manager), Akka (Model), Cassandra (Database) and Kafka (Message Broker)
* Data processing pipeline architecture
* Ingestion, aggregation, analysis
* All are Apache projects (except Akka)
* Highly available, resilient, and distributed

## Spark

<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/spark.png?raw=true" alt="Spark">

* Spark batch jobs
    * Easy to use
* Spark Streaming uses micro batches to address realtime usecases
    * compare to real time processing like Apache Flink
* Spark SQL: Sql like descriptive interface


## Mesos

<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/mesos.png?raw=true" alt="Mesos">

* Scheduling framework: Providing ressources for applications and jobs
* Hardware abstraction
* distributes workload across the cluster
* Orchestrate components and manage ressources
* DC/OS: DataCenter Operating System
    * using mesos
    * Microservices and Container


## Akka

<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/akka.png?raw=true" alt="Akka">

* implementation of the actor framework
* allows to create message-driven applications
* actor based concurrency
* fault-tolerant
* commonly used with scala, but java is possible
* `akka-http` for REST services


## Cassandra

<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/cassandra.png?raw=true" alt="Cassandra">

* NoSQL
* Wide Column Store
* linear, horizontal scaling
* No single point of failure
* Performance
* Connectors for spark and mesos
* Possible to be used accross multiple data centers


## Kafka

<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/kafka.png?raw=true" alt="Kafka">

* Distributed messaging system
* high availability, high throughput, low latency
* using a distributed commit log internally
* Producers publish to a pub/sub message queue
* Data will be partioned within topics
* Partitions can be distributed to cluster nodes
* Consumers will receive the requested messages

