Some tips, for those willing to run PIG in map-reduce mode, using a local hadoop cluster.
Make sure that Pig can reach your cluster, on my configuration, I had to do this:
export HADOOP_HOME=~/work/hadoop-2.9.0/

After this, when I launch PIG I have the following output:

.... (ommited for brevity)
2018-02-06 23:03:35,569 [main] INFO  org.apache.pig.backend.hadoop.executionengine.HExecutionEngine - Connecting to hadoop file system at: hdfs://localhost:9000
2018-02-06 23:03:36,649 [main] INFO  org.apache.pig.PigServer - Pig Script ID for the session: PIG-default-717063b8-934a-4d21-abcd-cf8880bfa112
2018-02-06 23:03:36,649 [main] WARN  org.apache.pig.PigServer - ATS is disabled since yarn.timeline-service.enabled set to false
grunt> 
The last line is of course our grunt shell, from where we are going to execute the commands.

