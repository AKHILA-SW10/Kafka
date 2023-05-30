# Kafka
Execution steps:

Terminal 1:
$ tar -xzf kafka_2.13-3.4.0.tgz
$ cd kafka_2.13-3.4.0
$ bin/zookeeper-server-start.sh config/zookeeper.properties

Terminal 2:
$ cd kafka_2.13-3.4.0
$ bin/kafka-server-start.sh config/server.properties

Terminal 3:
$ cd kafka_2.13-3.4.0
$ bin/kafka-console-consumer.sh --topic quickstart-events --from-beginning --bootstrap-server localhost:9092

