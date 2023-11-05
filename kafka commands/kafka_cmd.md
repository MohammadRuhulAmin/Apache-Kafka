<h3>How to start/stop zookeeper ? </h3>
<ul>
	<li>Step 1 : go to conf and make a file zoo.conf </li>
	<li>Step 2 remove comments </li>
	<li>Step 3:  4lw.commands.whitelist=*(add this)</li>
	<li>step 4: <b>getting all the commands :</b>  bin/zkServer.sh  </li>
	<li>step 5: bin/zkServer.sh start-foreground  (it will execute infornt of terminal) </li>
	<li>step 6: to stop zookeeper server : bin/zkServer.sh stop </li>
</ul>


<h3>How to start/stop kafka Server ? </h3>
<ul>
	<li>Step 1 : to start kafka server we need to execute bin/kafka-server-start.sh script  </li>
	<li>Step 2 :to stop kafka server we need to execute bin/kafka-server-stop.sh script </li>
	<li>Step 3: we need to configure conf/server.properties </li>
	<li>step 4: in server.properties broker.id = 1  </li>
	<li>step 5: listeners=PLAINTEXT://localhost:9092 </li>
	<li>step 6: to check if kafka is running or not using zookeeper : echo dump | nc | localhost 2181 | grep brokers </li>

</ul>

<h3> How to create a topic? </h3>
<p> We will use kafka-topic.sh script to create topics</p>
<ul>
	<li>creating topic : bin/kafka-topics.sh --bootstrap-server localhost:9092 --create --topic myTopic --partitions 1 -- replication-factor 1</li>
	<li>to see topic list : bin/kafka-topics.sh --bootstrap-server localhost:9092 --list</li>
	<li>to know details about a topic : bin/kafka-topics.sh --bootstrap-server localhost:9092 --describe --topic myTopic</li>
	
</ul>

