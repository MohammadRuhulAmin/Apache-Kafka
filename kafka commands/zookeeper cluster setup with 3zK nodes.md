
  server         server         server         server 
(zookeeper )   (zookeeper )  (zookeeper )    (zookeeper )
    |            |              |               |
	                                          client(kafka server)
	                          client(kafka server)
				 |			 			 
	|            client (kafka server)
	|
	|
	client (kafka server)
	
	
<p>	any of the zookeeper server can be leader using an algorithm. zookeeper leader will decide 
	to take if it will take the request or not for processing </p>
	
<b style="color:red;">In zookeeper cluster we must run odd number of zookeeper server.</b>

configuring zookeeper cluster Node1 in config/zoo.cfg

tickTime=2000 // it is 2000 mili seconds 
initLimit=10 // zookeeper node will connect to zookeeper cluster by 10 unites of time
syncLimit=5 //  zookeeper cluster will kick if a zookeeper node is unable to sync in between 5 unit of time 
dataDir=/tmp/zookeeper-1 // it holds the client (kafka's) information 
clientPort=2181 // kafka will connect to this port number to communicate with zookeeper cluster
maxClientCnxns=60 // the maximum number of client or kafka which can connect to a single zookeeper node

4lw.commands.whitelist=*

 // here 1,2,3 are the 3 unique identifire.
 

server.1=localhost:2788:3788 // here 2788 are used to communicate among zookeeper server to another zookeeper server 
 // here 3788 port used for leader election
server.2=localhost:2888:3888 // 
server.3=localhost:2988:3988

	
	