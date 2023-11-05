
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
	
	
	