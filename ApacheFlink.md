Apache Flink is an open source stream processing framework developed by the Apache Software Foundation. The core of Apache Flink is a distributed streaming dataflow engine written in Java and Scala.[1][2] Flink executes arbitrary dataflow programs in a data-parallel and pipelined manner.[3] Flink's pipelined runtime system enables the execution of bulk/batch and stream processing programs.[4][5] Furthermore, Flink's runtime supports the execution of iterative algorithms natively.[6]

Flink provides a high-throughput, low-latency streaming engine[7] as well as support for event-time processing and state management. Flink applications are fault-tolerant in the event of machine failure and support exactly-once semantics.[8] Programs can be written in Java, Scala,[9] Python,[10] and SQL[11] and are automatically compiled and optimized[12] into dataflow programs that are executed in a cluster or cloud environment.[13]

Flink does not provide its own data storage system and provides data source and sink connectors to systems such as Amazon Kinesis, Apache Kafka, HDFS, Apache Cassandra, and ElasticSearch.[14]