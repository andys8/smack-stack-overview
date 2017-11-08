# SMACK Stack

The SMACK stack is a collection of technologies which can be composed to create a private cloud architecture. The acronym SMACK stands for Spark (engine), Mesos (manager), Akka (model), Cassandra (database) and Kafka (message broker). All except Akka are Apache projects. The goal is to achieve a highly available, resilient and distributed data processing architecture to enable explorative, realtime data-analysis and fast deployment.


## Spark

<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/spark.png?raw=true" alt="Spark">

Spark is a engine for large-scale data processing and makes it easy to build parallel applications or batch jobs. An advantages over Hadoop MapReduce is superior performance. There is also support to query structured data using "Spark SQL". On the other hand, "Spark Streaming" addresses real time usecases. Incoming data is chunked into micro batches which will processed seperately. Due to batch processing architecture latency is in the order of seconds or minutes. In comparison: Stream processing frameworks like Apache Flink operate with millisecond latencies.


## Mesos

<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/mesos.png?raw=true" alt="Mesos">

Mesos is a scheduling framework to manage clusters. It provides ressources for application, services and jobs and abstracts the underlying hardware. The workload is distributed across the cluster. With the distributed operating system "DC/OS" on top of mesos deployment and scaling of containerized applications is provided in a single place.


## Akka

<img width="300" src="https://github.com/andys8/smack-stack-overview/blob/master/img/akka.png?raw=true" alt="Akka">

Akka is an implementation of the Actor Model and allows to create message-driven applications in Scala or Java. The toolkit is inspired by Erlang and its fault-tolerance due to actor based concurrency. Actors can modify local state but don't expose it. Instead they use asynchronous messages to interact with other actors.


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

