# SMACK Stack

The SMACK stack is a collection of technologies which can be composed and form a Big-Data platform. The acronym SMACK stands for Spark (engine), Mesos (manager), Akka (model), Cassandra (database) and Kafka (message broker). All except Akka are Apache projects. The goal is to achieve a highly available, resilient and distributed data processing architecture to enable explorative, realtime data-analysis and fast deployment.


## Spark

<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/spark.png?raw=true" alt="Spark">

* Spark: Engine for large-scale data processing
    * batch jobs
    * Easy to use
    * Faster than Hadoop MapReduce
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

