# Apache Kafka
__What is Apache kafka ?__    
=> Apache kafka is a distributed message streaming platform that uses publish and 
subscribe mechanism to stream the records.It is orginally developed by Linkedin and later doneted to Kafka Foundation. It is opensource and used by many tech jiant company like linkedin , walmart,Netflix,uber,airbnb etc.

---

__What is stream ?__   
=> it means flow of data

---

__what is record ?__   
=> According to kafka it is Data.

---

__What is centralized database ?__   
=> Where all the data will be stored in one place. if database gets affected, all the data will be 
lost .

---

__What is distributed database?__   
=> instead of loading one database , the data will be stored in multiple locations.If one database gets
affected , other data base will remain safe.  

It has two type.  
1.When we copy the full Entity to the multiple location , we consider it as replication  
2.When we break the entity and store it to different location part by part means the whole data  
can be distributed in equally or randomly.

---

__What is Messaging System ?__   
 _Records , Data and messages these three are same in messaging System!_
=>A messaging system is responsible for transferring data from one application to another so the applications can focus on data without getting bogged down on data transmission and sharing.  

it is two type :  
a. point to point messaging system  
    *messages are parsed in queue  
    * A perticular message can be consumed by a maximum of one receiver only  
    * There is no time dependency laid for the reveiver to receive the message  
    * When the receiver receives the message, it will send an acknoledgement back to the Sender.  
b. public subscribe messaging  
system:
    * Messages are persisted in a Topic  
    * A particular message can be consumed by any number of consumers.  
    * There is a time dependency laid for the consumer to consume the message.  
    * when the subscriber receives the message, it doesnt send an acknoledgement to the publisher.  

---

__What is Topic ?__    
=>Topic is like a queue with some additional featers!messages doesnot delete in topic.The subscriber can get 
the messages from the topic when they need in a limited time interval.Kafka is a public subscribe messaging 
system.

---# Apache Kafka
__What is Apache kafka ?__    
=> Apache kafka is a distributed message streaming platform that uses publish and 
subscribe mechanism to stream the records.It is orginally developed by Linkedin and later doneted to Kafka Foundation. It is opensource and used by many tech jiant company like linkedin , walmart,Netflix,uber,airbnb etc.

---

__What is stream ?__   
=> it means flow of data

---

__what is record ?__   
=> According to kafka it is Data.

---

__What is centralized database ?__   
=> Where all the data will be stored in one place. if database gets affected, all the data will be 
lost .

---

__What is distributed database?__   
=> instead of loading one database , the data will be stored in multiple locations.If one database gets
affected , other data base will remain safe.  

It has two type.  
1.When we copy the full Entity to the multiple location , we consider it as replication  
2.When we break the entity and store it to different location part by part means the whole data  
can be distributed in equally or randomly.

---

__What is Messaging System ?__   
 _Records , Data and messages these three are same in messaging System!_
=>A messaging system is responsible for transferring data from one application to another so the applications can focus on data without getting bogged down on data transmission and sharing.  

it is two type :  
a. point to point messaging system  
    *messages are parsed in queue  
    * A perticular message can be consumed by a maximum of one receiver only  
    * There is no time dependency laid for the reveiver to receive the message  
    * When the receiver receives the message, it will send an acknoledgement back to the Sender.  
b. public subscribe messaging  
system:
    * Messages are persisted in a Topic  
    * A particular message can be consumed by any number of consumers.  
    * There is a time dependency laid for the consumer to consume the message.  
    * when the subscriber receives the message, it doesnt send an acknoledgement to the publisher.  

---

__What is Topic ?__    
=>Topic is like a queue with some additional featers!messages doesnot delete in topic.The subscriber can get 
the messages from the topic when they need in a limited time interval.Kafka is a public subscribe messaging 
system. _A stream of messages belonging to a perticular catagory called Topic, similar to a table in a database
the unique identifier of a topic is it's Name. We can create topic as many as we want!_  
Topic Has two categories.  
1. Partision  
    (All the messages are splitted in to partision. it is ordered and immutable. Each partision has unique id name offset) Producer application will produce messages in Partision and the consumer will get messages
    from pertision.
2. Replication  
    (It is backup of partision).Producer application will never write messages to replica and the consumer
    will never get messsages from replica.replica can never read or write data

---

__What is Broker ?__  
=> Broker is a software process who manage the topics.Broker can track the information that which consumer
application has access the amount message from which topic from a pertision!Broker is also known as
kafka server.

__What is Kafka Cluster ?__  
=>A set of brokers who are communicating with eachother to perform the management and maintance task are 
collectively known as kafka cluster. 


---
# Kafka Architecture

__Describe Kafka Architecture__  
=>Kafka Cluster is made of some broker.inside a broker there are some topics.Topics are splitted into some
partisions.Kafka cluster is managed by zookeeper cluster. the zookeeper cluster has some zookeeper nodes.  
    
There will be some procuder applications. Some producer may produce  messages to topic level and some may   
produce message in pertision level.

Also there will be some consumer application . They will consume the messages from topic level or pertision level.  
There will be consumer group.Each consumer application is assigned inside a consumer Group.






