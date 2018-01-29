# ansible_kafka
создать топик с именем testing
```
/opt/kafka/bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic testing
```

интерактивный режим отправки сообщений в топик testing
```
/opt/kafka/bin/kafka-console-producer.sh --broker-list localhost:9092 --topic testing
```

чтение сообщений из топика testing
```
/opt/kafka/bin/kafka-console-consumer.sh --zookeeper localhost:2181 --topic testing --from-beginning
```
