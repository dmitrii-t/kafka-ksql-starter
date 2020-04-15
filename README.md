# Kafka KSQL starter

### Synopsis

The project is an example of ETL pipeline to calculate and populate transaction summaries for 
specified time range without coding KStream application.

### Prerequisites

1. Docker
1. Make
1. Bash

### Getting Started

To run complete project with docker containers and service provisioning use 

```bash
make start
```

To spin up docker containers only use


```bash
make up
```

To spin up particular service only use

```bash
make up <service>

# like for example
make up broker 
```

To run and attach to stdout of a particular service use

```bash
make run <service>

# for instance 
make run dataload

```

To stop all services use
```bash
make down
```

### TODO
1. Convert Avro `timestamp` to Postgres `Timestamp`

