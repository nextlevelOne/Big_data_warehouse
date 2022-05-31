# Big_data_warehouse
behavior Data ----> Flume----> ODS(raw/back up)-> DWD(data preprocess and cleaning)->DWS(daily ) DWT(yearly)-> ADS(stast and index: mysql) --> output  
business Data ----> Sqoop----> ODS(raw/back up)-> DWD(data preprocess and cleaning)->DWS(daily ) DWT(yearly)-> ADS(stast and index: mysql) --> output


bussiness need:
1.user behavioral data collection platform buid

2.bussinees data collection platform buid

3.Data Warehouse modelling

4.events, users, merchandises, regions tables

5.ad hoc enqury

6.clusters efficiency alert 

7.hive metadata management

8.data quality monotiring 

9.authority management


Tech stack Selection:
1.Data Size(which database)
2.bussiness need(effectiveness:fast flink or slow spark)
3.industry experience(if all flink among Faang, we use flink as well)
4.maturity of tech (data warehouse ---> data center(so so) ----> data lake(not mature))
5.development and maintenence expense
6.total expense


Data transportation: 
Flume, Kafka(buffer area when data size is huge), sqoop(bussiness data),logstash, DataX

Data storage:
Mysql(small size ADS) , HDFS(large size ), HBase, Redis, MongoDB

Data Calculation:
Hive, Tez(fast, in ram), Spark(selected), Flink, Storm

Data query:
Presto, Kylin, Impala, Druid, ClickHouse, Doris

Data visualization:
Echarts, Superset, Tableu, powerBI

Task scheduling:
Azkabam, Oozie, Airflow

Clusters monitoring:
Zabbix, Prometheus

metadata management:
Atlas

Authority management:
Ranger

Apache specs:
Hadoop.      3.1.3
zookeeper    3.5.7
MySql.       5.7.16
Hive         3.1.2
Flume.       1.9.0
Kafaka.      2.4.1.    
Kafka Eagle  1.4.5
Azkaban.     3.84.4
Spark.       3.0.0
Hbase.       2.0.5
Phoenix.     5.0.0
Sqoop.       1.4.6
Presto.      0.189
Kylin.       3.0.1
Atlas        2.0.0
Ranger.      2.0.0
Solr.        7.7.0
