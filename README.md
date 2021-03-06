# ansible-kafka
This script will deploy a typical multinode kafka cluster guided by Confluent. 

## What's inside?
It will setup a three node cluster, kafka and zookeeper are co-location on each node. kafka and zookeeper are deployed in the containerization way.

It will install following components: 
 - Apache Kafka® 2.3.0 and zookeeper from Confluent Platform 5.3.0
 - kafkacat 1.4.0
 - latest stable docker-ce and docker-compose from docker.com

## Feature highlight
 - rolling update
 - ansible best practice project struture
 - [todo] 

## Alternatives
 * If all you need is an simple all-in-one kafka setup for development, use [docker-compose templates ](https://github.com/confluentinc/cp-docker-images/tree/5.3.0-post/examples) provided by Confluent.
 * For complex kafka cluster setup, use [ansible playbook](https://github.com/confluentinc/cp-ansible) powered by Confluent.

## Requirements
We use this script with following system confiuration:
 * ubuntu 16.04
 * ansible 2.8

## Getting start
1. setup ssh passwordless 
2. `$apt install ansible`
3. update configs in `hosts` and `group_vars/all` file
4. `$ansible-playbook -i hosts site.yml`

## Reference
* https://docs.confluent.io/current/kafka/multi-node.html#cp-multi-node
* https://docs.confluent.io/current/installation/docker/installation/index.html#cp-docker-install

## TODO:
* Remove host vars in group_vars/all
* Set /etc/hosts
