# sparkStreaming2.2.0-Kafka1.0.0
This project is based on kafka 0.10.0.1 (or higher), and spark 2.2.0 (or higher.) 
It uses the new Kafka producer API to generate kafka Producer Records; 
It uses the spark-streaming-kafka-0-10_2.11 to create Direct Kafka Stream.

To produce records into KAFKA topic:
java com.hpeu.sparkStreaming.test.NewKafkaProducerTest topicName

To consume records from KAFKA topic:
spark-submit --master spark://node1:7077 --class com.hpeu.sparkStreaming.test.DirectKafkaConsumerTest sparkStreamingDemo-1.0-SNAPSHOT-jar-with-dependencies.jar bootstrapServer1:9092,bootstrapServer2:9092,bootstrapServer3:9092 topic1 SIGNAL4
