# ansible-kafka
Deploy multinode kafka cluster based on Confluent guide

## Getting start
1. setup ssh passwordless 
2. `$apt install ansible`
3. update vars in `hosts` file
4. `$ansible-playbook kafka.yml`

## Reference
* https://docs.confluent.io/current/kafka/multi-node.html#cp-multi-node
* https://docs.confluent.io/current/installation/docker/installation/index.html#cp-docker-install
