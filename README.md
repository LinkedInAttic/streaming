# LinkedIn Streaming Team open-source projects

This is an umbrella repository to host all open-source projects developed by
LinkedIn Streaming team. Each project is tracked as a git submodule.

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

### Burrow (https://github.com/linkedin/Burrow)

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





