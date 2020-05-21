# kafka-java-app
- Command to run a zookeeper service

  `.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties`  
- Command for Running Kafka service  

  `.\bin\windows\kafka-server-start.bat .\config\server.properties`
- command for Creating a topic 

`.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic test`

- command for running consumer app

  `java -cp target/kafa-java-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.jeevanmure.MyConsumer test group1`
  
- command for running producer
  
  `java -cp target/kafa-java-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.jeevanmure.MyProducer test group1`
