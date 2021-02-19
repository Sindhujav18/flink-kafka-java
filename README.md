# Big Data Project- Flink-Kafka-Java

To perform operations on dataset using bigdata tools like flink and kafka.

## Group Members

<table>
<td align="center"><a href="https://github.com/Sindhujav18"><img src="https://avatars.githubusercontent.com/u/60013028?s=400&u=ef2dc873708871440e68a0055f565f1b7355892d&v=4" width="100px;" alt=""/><br /><sub><b>Sindhuja Valeti</b></sub></a><br /></td>

<td align="center"><a href="https://github.com/sindhurani29"><img src="https://avatars.githubusercontent.com/u/60019365?s=460&u=1848679a76d03414de088d61ca9d2bc3f518a937&v=4" width="100px;" alt=""/><br /><sub><b>Sindh Rani Goli</b></sub></a><br /></td>

<td align="center"><a href="https://github.com/Mohanalavala"><img src="https://avatars.githubusercontent.com/u/60022212?s=400&u=676fdd8ee2b9ed0e005879701cfdc37f14483d39&v=4" width="100px;" alt=""/><br /><sub><b>Mohan Krishna Alavala</b></sub></a><br /></td>

<td align="center"><a href="https://github.com/vineetha1996"><img src="https://avatars.githubusercontent.com/u/59989572?v=4" width="100px;" alt=""/><br /><sub><b>Vineetha Yenugula</b></sub></a><br /></td>

<td align="center"><a href="https://github.com/dexterstr"><img src="https://avatars.githubusercontent.com/u/31917612?s=400&v=4" width="100px;" alt=""/><br /><sub><b>Tarun Sarpanjeri</b></sub></a><br /></td>

<td align="center"><a href="https://github.com/neeleshsaladi"><img src="https://avatars.githubusercontent.com/u/42808129?s=460&u=133da9540a40568c5847d37a0a2c7454ae83c3da&v=4" width="100px;" alt=""/><br /><sub><b>Neelesh Saladi</b></sub></a><br /></td>

</table>

## Mohan Krishna Alavala

## Demonstration Skill:
- I'm going to give demonstration on installation and configuration of kafka on windows machine.

## Prerequisites:
- Apache Kafka 2.13
- Zookeeper 3.4
- Maven
- Java (Java 8 or Java 11)
- IntelliJ IDE
- Powershell

## Introduction to Kafka
- You can instal kafka by clicing on the following [link](https://kafka.apache.org/downloads) 
- After download is completed, you can get a tar file. Extract the tar file by useing command 
1. tar -xzf kafka_2.13-2.7.0.tgz
2. cd kafka_2.13-2.7.0
- After that you need to set the environment variable under KAFKA_HOME with C:\kafka_2.13-2.7.0

## Kafka set up using Maven
- To demonstrate I'm creating a project using maven in IntelliJ IDE.
- You need to slect the Maven in the
 left pane and java version on the start screen. Now click on finish
 ![image1](https://github.com/Sindhujav18/flink-kafka-java/blob/main/int1.png)

- Next, you need to select the name of the project, which will be the artifact id and click on finish.
![image2](https://github.com/Sindhujav18/flink-kafka-java/blob/main/int2.png)
- Now, you need to add dependencies to pom.xml file, there are some mandotory dependencies that you need to add.
![image3](https://github.com/Sindhujav18/flink-kafka-java/blob/main/int3.png)
- Demonstration Video: https://app.vidgrid.com/view/0POsipXWwQ6Q

## Basic commands to use kafka
- To start Kafka environment
---
``bin/zookeeper-server-start.sh config/zookeeper.properties``

``bin/kafka-server-start.sh config/server.properties``

## References
- https://www.tutorialspoint.com/apache_kafka/apache_kafka_installation_steps.htm 
- https://kafka.apache.org/quickstart 

---
## Sindhu Rani Goli
## Demonstration skill:
- Demonstrating on kafka application using intelliJ idea.
- Creating topic, running and display 10 messages using powershell and intelliJ 

## Prerequisites:
- Apache Kafka 2.13
- Java (Java 8 or Java 11)
- Zookeeper 3.4
- IntelliJ IDE
- Powershell
- Maven

## Steps involved:

- Installation of intelliJ idea and create a new Maven project using appropriate ID's and name of project.
- Adding plugins and required dependencies in pom.xml file which is called configuration.
- Then, logging is enabled in our kafka application.
- Create log4j2.xml file in resources. This defines a console appender and formats the output.
- We define 3 loggers root logger, console logger and application logger.
- we create a java class on right clicking on src main java node in project explorer and give class and package names.
- Then edit confiurations by selecting edit configurations and then applications in templates. 
- Now the the zoomkeeper and kafka commands are run and topic name is given as well in powershell.
- Run the project in intelliJ idea and the messages are displayed.

## Output:

![image1]()

## Demonstration video:
Link: https://app.vidgrid.com/view/LdVb2QAG0peC 


---
## Sindhuja Valeti

## Demonstration Skill: 

- Creating Kafka Streams application.
- Reading a stream from kafka cluster and printing key value pair on console

## Prerequisites:

- Apache Kafka installed (2.7.0)
- JDK installed
- IntelliJ IDE installed (Community Edition : https://www.jetbrains.com/idea/download/#section=windows)

## Procedure and Commands:

- After installing IntelliJ IDE successfully, create a new Maven project with group ID, artifactID and project name.

- Add all the dependencies like kafka-clients, kafka-streams, log4j2 to integrate Kafka with intelliJ IDE.

- Now create a kafka producer java class under the package structure, the source code for producer is [kafka-producer](https://github.com/Sindhujav18/flink-kafka-java/blob/main/kafka-producer)

- The producer class contains the source code, that generates sample text messages.

- We will start reading the streams from a given topic using kafka streams java class.

- source code for kafka streams is [kafka-streams](https://github.com/Sindhujav18/flink-kafka-java/blob/main/kafka-streams)

- After creating producer and streams java files, now start the zookeeper service, kafka server and create a topic in the local host.

- Now run the producer class and Streams class in intelliJ IDE.

## Output snippet :

 ![](https://github.com/Sindhujav18/flink-kafka-java/blob/main/Flink-Kafka-Interaction_Images/kafka%20streams%20application.PNG?raw=true)












## Overview Of Apache Flink and Apache Kafka:
- Apache Flink is a stream processing framework that can be used easily with Java. 
- Apache Kafka is a distributed stream processing system supporting high fault-tolerance.

## Flink Usage:
Apache Flink allows a real-time stream processing technology. The framework allows using multiple third-party systems as stream sources or sinks.
In Flink – there are various connectors available :
- Apache Kafka (source/sink)
- Apache Cassandra (sink)
- Amazon Kinesis Streams (source/sink)
- Elasticsearch (sink)
- Hadoop FileSystem (sink)
- RabbitMQ (source/sink)
- Apache NiFi (source/sink)
- Twitter Streaming API (source)

## Kafka Usage:







### Flink-Kafka-Interaction:

<p align="center">
<img src="https://github.com/Sindhujav18/flink-kafka-java/blob/main/Flink-Kafka-Interaction_Images/1-kafka-flink-pipeline-1.png"
     alt="Size Limit logo by Anton Lovchikov" width="598" height="236">
 </p>


### Resources:
- [Apache_Flink_Kafka_Guide](https://www.ververica.com/blog/kafka-flink-a-practical-how-to)
- [Apache_Flink_Kakfa_connection](https://ci.apache.org/projects/flink/flink-docs-stable/dev/connectors/kafka.html)
## Demonstration

#### Vineetha Yenugula
In our project i have used a simple Flink job to show how to integrate Apache Kafka to Flink using the Flink Connector for Kafka.

- You can find the detailed information like prerequisites, commands and how to run an application in my [Repo_Link](https://github.com/vineetha1996/rt-flink-kafka-java/blob/main/README.md)

