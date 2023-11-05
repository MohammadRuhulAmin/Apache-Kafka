<h1>How to start/stop zookeeper ? </h1>
<ul>
	<li>Step 1 : go to conf and make a file zoo.conf </li>
	<li>Step 2 remove comments </li>
	<li>Step 3:  4lw.commands.whitelist=*(add this)</li>
	<li>step 4: <b>getting all the commands :</b>  bin/zkServer.sh  </li>
	<li>step 5: bin/zkServer.sh start-foreground  (it will execute infornt of terminal) </li>
	<li>step 6: to stop zookeeper server : bin/zkServer.sh stop </li>

</ul>