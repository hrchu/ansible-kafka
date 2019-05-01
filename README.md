# ansible-kafka
This will deploy multinode kafka cluster based on the Confluent guide. It setups three nodes, and each node runs both kafka and zookeeper in the docker containerization way.

## Getting start
1. setup ssh passwordless 
2. `$apt install ansible`
3. update vars in `hosts` file
4. `$ansible-playbook kafka.yml`

## Reference
* https://docs.confluent.io/current/kafka/multi-node.html#cp-multi-node
* https://docs.confluent.io/current/installation/docker/installation/index.html#cp-docker-install
