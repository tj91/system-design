## Pinot

Real-time distributed **OLAP** datastore, built to deliver scalable real-time analytics with low latency. It can ingest from batch data sources (such as Hadoop HDFS, Amazon S3, Azure ADLS, Google Cloud Storage) as well as stream data sources (such as Apache Kafka).

Apache Pinot includes the following:
- Ultra **low-latency** analytics even at extremely high throughput.
- **Columnar** data store with several smart indexing and pre-aggregation techniques.
- Scaling up and out with **no upper bound**.
- **Consistent performance** based on the size of your cluster and an expected query per second (QPS) threshold.

Whats is Pinot? </p> https://www.youtube.com/watch?v=_lqdfq2c9cQ

### Ingestion

**Batch** : Pinot supports Spark, Flink, Hadoop etc for batch ingestion
**Streaming** : Pinot has out-of-the-box real-time ingestion support for Kafka, Kinesis etc


**How Pinot helps to solve realtime analytics**

Following image shows requirements for real time analytics, and how tools like Presto etc are used for internal dash boarding
<p align="center">
<img src="https://github.com/tj91/system-design/assets/1821801/baeff1b7-d723-49d2-afc3-47cdb2958f7a" width="200" height="266">
</p>
