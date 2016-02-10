<code>
nohup bin/zookeeper-server-start.sh config/zookeeper.properties  > zk.nohup &
nohup bin/kafka-server-start.sh config/server.properties  > k0.nohup &
bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic test
bin/kafka-topics.sh --list --zookeeper localhost:2181
</code>
