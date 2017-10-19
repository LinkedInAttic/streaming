# LinkedIn Streaming Team open-source projects

This is an umbrella repository to provide reference of all open-source projects
developed by LinkedIn Streaming team. Each project is tracked as a git
submodule in this repository. Link to the github homepage of each
project can be found in the README below.

## Getting Started

### Checkout all projects
```
git submodule update --init
```

### Checkout a selected project
```
git submodule update --init -- <relative path to submodule>
```

### Pull latest code from all projects
```
git submodule foreach 'git pull origin master'
```

## Projects

Here is the list of projects and their description.

## likafka

### Burrow (https://github.com/linkedin/burrow)

Burrow is a monitoring companion for Apache Kafka that provides consumer lag
checking as a service without the need for specifying thresholds. It monitors
committed offsets for all consumers and calculates the status of those
consumers on demand. An HTTP endpoint is provided to request status on demand,
as well as provide other Kafka cluster information. There are also configurable
notifiers that can send status out via email or HTTP calls to another service.

### Kafka Monitor (https://github.com/linkedin/kafka-monitor)

Kafka Monitor is a framework to implement and execute long-running kafka system
tests in a real cluster. It complements Kafka’s existing system tests by
capturing potential bugs or regressions that are only likely to occur after
prolonged period of time or with low probability. Moreover, it allows you to
monitor Kafka cluster using end-to-end pipelines to obtain a number of derived
vital stats such as end-to-end latency, service availability and message loss
rate. You can easily deploy Kafka Monitor to test and monitor your Kafka
cluster without requiring any change to your application.

### Cruise Control (https://github.com/linkedin/cruise-control)

Cruise Control is a product that helps run Apache Kafka clusters at large
scale. Due to the popularity of Apache Kafka, many companies have bigger and
bigger Kafka clusters. At LinkedIn, we have 1800+ Kafka brokers, which means
broker deaths are an almost daily occurrence and balancing the workload of
Kafka also becomes a big overhead. Kafka Cruise control addresses this
operation scalability issue by tracking resource utilization in the cluster and
automatically rebalance partitions across brokers if needed. It is highly
customizable and user can specify rules to determine when and how partitions
should reassigned across brokers.

### li-apache-kafka-clients (https://github.com/linkedin/li-apache-kafka-clients)

li-apache-kafka-clients is a wrapper Kafka clients library built on top of
vanilla Apache Kafka clients. It provides proprietary features such as large
message support and auditing which are not available in vanilla Kafka clients.




