# ELK with Flocker and Docker

## How to use this repository

### Prerequisites

A Flocker cluster up and running. For more information about getting up and running with Flocker, [click here](https://docs.clusterhq.com/en/1.8.0/labs/installer-getstarted.html)

Docker Compose installed
```
$ curl -L https://github.com/docker/compose/releases/download/1.5.2/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose
$ chmod +x /usr/local/bin/docker-compose

```

### How to run

#### Single Node Deployment

From one of your Flocker nodes.

```
$ git clone https://github.com/wallnerryan/elk-flocker-compose
$ cd elk-flocker-compose
$ docker-compose -f docker-compose.yml up -d
```

#### Multi Node Deployment

From one of your Flocker nodes.

```
$ git clone https://github.com/wallnerryan/elk-flocker-compose
$ cd elk-flocker-compose/multi-node
# Edit IP Addresses marked as X.X.X.X or X-X-X-X
$ docker-compose -f docker-compose-multi.yml up -d
```
