# kafka-poc

- start local kafka (1 zookeeper instance + 2 kafka instances)
- 1 producer instance producing stock quotes
- multiple consumer instances (same consumer group and different consumer groups)
- try to reproduce multiple deliveries (at least once)

# topic commands

## create topic

```
 kafka-topics --create --topic andrei-rules --bootstrap-server broker:29092,broker_bob:29093 --partitions 2 --replication-factor 2
```

## describe topic

```
kafka-topics --describe --topic andrei-rules --bootstrap-server broker:29092,broker_bob:29093
```