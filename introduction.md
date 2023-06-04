1.What is Apache kafka ? 
=> Apache kafka is a distributed message streaming platform that uses publish and 
subscribe mechanism to stream the records.It is orginally developed by Linkedin and later doneted to Kafka Foundation. It is opensource and used by many tech jiant company like linkedin , walmart,Netflix,uber,airbnb etc.

What is stream ? 
=> it means flow of data

what is record ? 
=> According to kafka it is Data.

What is centralized database ? 
=> Where all the data will be stored in one place. if database gets affected, all the data will be 
lost .

What is distributed database? 
=> instead of loading one database , the data will be stored in multiple locations.If one database gets
affected , other data base will remain safe.

It has two type.
1.When we copy the full Entity to the multiple location , we consider it as replication
2.When we break the entity and store it to different location part by part means the whole data
can be distributed in equally or randomly.

What is Messaging System ? 
# Records , Data and messages these three are same in messaging System!
=>
A messaging system is responsible for transferring data from one application to another so the applications can focus on data without getting bogged down on data transmission and sharing.

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




