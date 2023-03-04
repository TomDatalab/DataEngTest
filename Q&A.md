### :speaking_head: Instructions
<img src="https://raw.githubusercontent.com/MicaelliMedeiros/micaellimedeiros/master/image/computer-illustration.png" min-width="400px" max-width="400px" width="400px" align="right" alt="TomDatalab">

<p align="left"> 
  Choose a quiet and peaceful place to perform the tests. The main objective is that we can understand the level of knowledge of the candidate. Be honest with your answers. There is no pre-established time for completing the tests, <strong>do your best</strong>.<br>
</p>

## <img width="45" alt="about" src="https://raw.github.com/elizarov/elizarov/master/about.png"> Good luck !

:blue_book: <strong><b>1)</b></strong>  What is Data Engineering? 
<u>It's related to the process to collect data from any aource and create processes to ge this data, load it in a correct data store based on the caracteristics of this data, clean it, enrich it and become it available to be used by Data Analysis and Machine Learning models.</u>

:blue_book: <strong><b>2)</b></strong> What is Data Modeling?
<u>A conceptual model that will define how the data needs to be saved and organized.</u>

:blue_book: <strong><b>3)</b></strong> What are the design schemas available in data modeling?
<u>We have a lot ot possibilities to archive it and it will dependes on how the data will be used and on the characterists of the data. We can star schema or snowflake schema for a BI solution, or relational model to archive ACID transacions on a sistem, document model for a document noSQL database, data lakehouse for big data enviromnets, between others.</u>

:blue_book: <strong><b>4)</b></strong> What is the difference between a data engineer and a data scientist?
<u>Data Engineers will be responsable for collect and process data from any aource from bacth or streaming sources and for create processes to ge this data, load it in a correct data store based on the caracteristics of this data, clean it, enrich it and become it available. In the other hands the Data Scientists will be responsable for analise the data available and apply apply some matematical or estatistics algoritms searching for some patterns or answers for some negocial questions. this work will be not just related to create this models but to control all the life cicle of it in batch or streaming model production processes.</u>

:blue_book: <strong><b>5)</b></strong> What are the differences between structured and unstructured data?
<u>basically structured data has a data model attached on it (schema of data). Example of it: delimited csv files. Unstructured data doesn't have it. examples of it: IOT data, videos/ images files, emails texts between others. </u>

:blue_book: <strong><b>6)</b></strong> What are the features of Hadoop?
<u>Hadoop is a framework that was created by Yahoo. It was created to enable the ability of storage and process data in a parallel way using file formats. It's a open source framework with high scalabity (it grows in a horizontal way) and it's provides fault tolerance to guarantee data realibility between the cluster nodes.</u>

:blue_book: <strong><b>7)</b></strong> Which frameworks and applications are important for data engineers?
<u>Now a days the most important frameworks, in my opinion, for data engineers are Apache Spark and Kafka. The first one is a replace tool to handle the process part of the processing layer from the lambda achitecture. It replaces MapReduce because do the processing work using memory not disk. The second one is the ost powerfull tool for real streaming. </u>

:blue_book: <strong><b>8)</b></strong> What is HDFS?
<u>It's part of the main hadoop ecosistem and is responsable for store the data into chunks of files distributed between all nodes available into the cluster. All chunks of files are replicated 3 times (that can be configurable) to avoid lose data when some node going down.</u> 

:blue_book: <strong><b>9)</b></strong> What is a NameNode?
<u>in the most part of parallel architecutes you will have like a controler and works (for each framework you will enconter the same think with different mames, like spark: driver/workers). The nameNome is the controler node for HDFS clusters.</u>

:blue_book: <strong><b>10)</b></strong> What are the repercussions of the NameNode crash?
<u>the HDFS will stop to work. no data will be lose. In production enviroments it's recommended to have a high availability for it using a Active and Standby nameNode.</u>

:blue_book: <strong><b>11)</b></strong> What is a block and block scanner in HDFS?
<b>searched for this one!</b> <u>Block is the way hadoop saves data into dataNodes. by design it's 64MB of size and it could be configured. In the other hands Block scanner is a process that verify each block checksum to try find any data corruption into blocks storaged on HDFS datanodes.</u> 

:blue_book: <strong><b>12)</b></strong> What are the components of Hadoop?
<u>The main features of it are: HDFS (Hadoop Distributed File System) that is used for storage the data, Yarn (Yet Another Rresource Negociator) that is responsable for manage the resources and MapReduce that is used to process data using the local disks available in each node of the hadoop cluster</u>

:blue_book: <strong><b>13)</b></strong> Explain MapReduce in Hadoop.
<u>MapReduce a programming framework that is used inside Hadoop to process the data in a parallel way between the cluster nodes. It's done using hard disk.</u>

:blue_book: <strong><b>14)</b></strong> What is the Heartbeat in Hadoop?
<u>It's the way DataNodes can comunicate with NameNodes.</u>

:blue_book: <strong><b>15)</b></strong> How does the NameNode communicate with the DataNode?
<u>All communication between Namenode and Datanode is initiated by the Datanode, and responded to by the Namenode.</u>

:blue_book: <strong><b>16)</b></strong> What happens when the block scanner detects a corrupt data block?
<u>DataNode will report to the NameNode about the corrupted block. Then NameNode will start the process of creating a new replica using the correct replica of the corrupted block present in other DataNodes. The corrupted data block will not be deleted until the replication count of the correct replicas matches with the replication factor (3 by default).</u>

:blue_book: <strong><b>17)</b></strong> Explain indexing.
<u>Indexing is a technique to save the data in a way that benefits the search for it.</u>

:blue_book: <strong><b>18)</b></strong> Explain the main methods of reducer.
<u>setup(): At the start of a task, setup() method is called to configure various parameters for Reducer. reduce(): This is the main operation of Reducer. In reduce() method we define the task that has to be done for a set of values that share a key. cleanup(): Once reduce() task is done, we can use cleanup() to clean any intermediate data or temporary files.</u>

:blue_book: <strong><b>19)</b></strong> What is COSHH?
<u>It's a Hadoop scheduling system. The main objective of COSHH is to improve the mean completion time of jobs.</u>

:blue_book: <strong><b>20)</b></strong> What is the relevance of Apache Hadoop's Distributed Cache?
<u>It's a way to copy small files or archives to worker nodes in time. Hadoop does this so that these worker nodes can use them when executing a task. To save the network bandwidth the files get copied once per job.</u>

:blue_book: <strong><b>21)</b></strong> What are the four Vs of Big Data?
<u>When the parallel storage/process paradigm was created by google it was designed with 3 main Vs: 1. Volume - related to store large amount of data. Velocity - related to how muth performatically this data is saved and retrived. Variety - related to how many different file formats can be saveds and processed. Insade the usage of this paradigm into Datalake design 2 new Vs comes. It's: veracity - related to how much reliable the data saved is. Value - related to how much the data saved is important for the company.</u>

:blue_book: <strong><b>22)</b></strong> Explain the Star Schema in Brief.
<u>It's a design created by Kimball using as starting point Snowflake Schema created by Immon to save data into a Data Warehousing in a performatically way to be readed (It's done by reducing the amount if joins operations to retrive the data). Using it the data is saved in dimensions and fact tables where dimesions have the explanation of each entity of the data and fact has the merge of this entities with the measures of the information organized by time.</u>

:blue_book: <strong><b>23)</b></strong> Explain the Snowflake Schema in Brief.
<u>It was the first design for data Warehousing created by Immon. Considering that at the time save data with redudance was expensive, this model design tried to save the dimension data without have a redudance. This way we have small dimesions tables but more joins to retrive it.</u>

:blue_book: <strong><b>24)</b></strong> Name the XML configuration files present in Hadoop.
<u>CORE-SITE.XML - It informs Hadoop daemons where the NAMENODE runs in the cluster. It also informs the Name Node as to which IP and ports it should bind. HDFS-SITE.XML - It contains the configuration settings for NAMENODE, DATANODE, SECONDARYNODE. MAPRED-SITE.XML - It contains the configuration settings for MapReduce.</u>

:blue_book: <strong><b>25)</b></strong> What is Hadoop Streaming?
<u>Hadoop streaming is a utility that comes with the Hadoop distribution. The utility allows you to create and run Map/Reduce jobs with any executable or script as the mapper and/or the reducer.</u>

:blue_book: <strong><b>26)</b></strong> What is the Replication factor?
<u>It's a configuration that will setup the amount if replicas for the same data block that needs to exist inside the HDFS cluster. Default value is 3.</u>

:blue_book: <strong><b>27)</b></strong> What is the difference between HDFS block and InputSplit?
<u>HDFS Block the physical part of the disk which has the minimum amount of data that can be read/write. While MapReduce InputSplit is the logical chunk of data created by theInputFormat specified in the MapReduce job configuration.</u>

:blue_book: <strong><b>28)</b></strong> What is Apache Spark?
<u>It's a framework for processing data stored in HDFS. It's more performatically bacause use memory to save the data is being processed in memory.</u>

:blue_book: <strong><b>29)</b></strong> What is the difference between Spark and MapReduce?
<u>MapReduce save temporary data between each step of map/reduce in hard disk. Spark do it in memory.Spark's data processing speeds are up to 100x faster than MapReduce.</u>

:blue_book: <strong><b>30)</b></strong> What are Skewed tables in Hive?
<u>It occurs when data is wronglly distributed between the files/partitions into HDFS. That means most part of the data is in just one file/partition and the rest of it in the another ones. Once the process for file/partition is distributed between nodes to be done in a parallel way, when it happens one single node will handle almost all data to be processed.</u>

:blue_book: <strong><b>31)</b></strong> What is SerDe in the hive?
<u>It allows Hive to read data from a table, and write it back out to HDFS in any custom format.</u>

:blue_book: <strong><b>32)</b></strong> What are the table creation functions in Hive?
<u>It's CREATE TABLE command. It's used just to create a metadata inside hive point to a expecific location into HDFS. Using it it's possible to read/write data from/into HDFS folder using SQL commands.</u>

:blue_book: <strong><b>33)</b></strong> What are *args and **kwargs used for?
<u>It's used when it's not possible to know about the number of arguments to pass for a function.</u>

:blue_book: <strong><b>34)</b></strong> What do you mean by spark execution plan?
<u>It's the way spark convert commands to process data from one given language to actually java code will be runned into nodes JVM.</u>

:blue_book: <strong><b>35)</b></strong> What is executor memory in spark?
<u>Every spark application will have one executor on each worker node. The executor memory is basically a measure on how much memory of the worker node will the application utilize.</u>

:blue_book: <strong><b>36)</b></strong> Explain how columnar storage increases query speed.
<u>A columnar storage stores data by columns instead of rows, it can store more data in a smaller amount of memory.</u>

:blue_book: <strong><b>37)</b></strong> What is schema evolution?
<u>Table schema can change along the way it's used. Schema evolution means the table metadata will guarantee the new files with new schema can be merge together with the old files without the same schema information.</u>

:blue_book: <strong><b>38)</b></strong> What do you mean by data pipeline?
<u>A data pipeline is a way to automate the movement and transformations of data between source and target storage.</u>

:blue_book: <strong><b>39)</b></strong> What is orchestration?
<u>It's a way into data pipeline to organizate and schedule tasks.</u>

:blue_book: <strong><b>40)</b></strong> What are different data validation approaches?
<u>We have a lot of them. It will depends on the way the data is stored/processed. The main ones is: Data type validation, constraint validation and  schema validation.</u>

:blue_book: <strong><b>41)</b></strong> What was the algorithm you used in a recent project?
<u>do not know what you mean by "algorithm".</u>

:blue_book: <strong><b>42)</b></strong> Have you earned any certification related to this field?
<u>Yes. SQL Server certifications related of relational databases, certifications related to business intelligence architecture, certifications related to cloud (azure and GCP), certifications related to data engineering (microsoft, google and databricks/spark programming).</u>

:blue_book: <strong><b>43)</b></strong> What is the difference between no-code and low-code?
<u>Low-code mean you will need to code less than you would if you were developing something by yourself. Some of the work will be done by the framework. No-code mean you will not do code anything to do the job. You will just say for the framework what you need to do and it will do it for you.</u>

:blue_book: <strong><b>44)</b></strong> What tools did you use in your recent projects?
<u>Mainly spark on databricks (batch and streaming). Beside of it all tools related of data engineering inside Azure.</u>

:blue_book: <strong><b>45)</b></strong> What challenges did you face in your recent project and how did you overcome them?
<u>The most recent one was related to streaming data into spark without to give for the streaming process the schema of the data. I used for handle it a feature from databricks called auto-loader. It can create for you on the fly the schema of the data that is being processed but it can not handle datatype change into the schema evolution. The way I worked around this issue was creating a process before the auto-loader job to convert every json primary datatype to string and all dict datatype to arrays. This way, auto-loader will never have datatype change into our user case.</u>

:blue_book: <strong><b>46)</b></strong> Which Python libraries would you recommend for effective data processing?
<u>pyspark if you have spark. It will use dataframe API to process the data into the worker nodes in a parallel way.</u>

:blue_book: <strong><b>47)</b></strong> How do you handle duplicate data points in a SQL query?
<u>Uuse DISTINCT command.</u>

:blue_book: <strong><b>48)</b></strong> Have you ever worked with big data in a cloud computing environment?
<u>Yes. In GCP and Azure environments.</u>

:blue_book: <strong><b>49)</b></strong> What are the roles and responsibilities of a data engineer?
<u>A data engineer is responsible for collecting, managing, and converting raw data into information that can be interpreted by data scientists and business analysts. It needs to mantain this data processings was created and handle failures and performance on it.</u>

:blue_book: <strong><b>50)</b></strong> How to become a Data Engineer?
<u>I think the Data Engineer position is not just related with use some tools or to know them well. It's most related of understand the data and the company's processes to create the better possible way to load/process/read it. So in my opition the one want it will need to have a pretty good understand about data architecture and paradimgs and them, after that, choose a set of tools to become more specialty as possible on it.</u>

:blue_book: <strong><b>51)</b></strong> What are the differences between Ralph Kimball's approaches and Bill Inmon?
<u>Besides the star schema/snowflake schema thing, in my opinion is that Kimball's one focus on individual business areas (it has a Bottom-Up Approach) and Inmon's one focus on Enterprise-wide area (it has Top-Down Approach).</u>

:blue_book: <strong><b>52)</b></strong> What is Apache Airflow?
<u>It's a open-source orchestration tool created by Airbnb. It is an platform for developing, scheduling, and monitoring batch-oriented workflows.</u>

:blue_book: <strong><b>53)</b></strong> What is a parquet file?
<u>It's a open source file format that saves the data in a columnar storage way. It's most used by memory optimized tools for processing data.</u>

:blue_book: <strong><b>54)</b></strong> What are the differences between a Data Warehouse, Data Mart and a data lake?
<u>Using Kimball's architecture Data Mart is a star schema model with dimesion and fact tables. Data Warehouse is a set of Data Marts merged together using conformed dimensions. The data uses relational database to save and retrive data. It's uses ETL process to process the data. Datalake was a new architecture design created after hadoop adoption. It storages data in a raw format before to do transformation on it (using ELT process design). </u>

:blue_book: <strong><b>55)</b></strong> What are the differences in uses and applications for ETL, ELT and Streaming?
<u>ETL = Extraction, Transformation and Load. Used to transform data before to stores it into the target storage. In the other hands, ELT = Extraction, Load and Transformation. Used into a datalake/lakehouse architecture to create a source of truth for raw data. This way we do not have data silos (all company can have the same data and use it for their processes getting the data from the same source). Streaming process is just a way to do ETL/ELT processes in a realtime manner.</u>

:blue_book: <strong><b>56)</b></strong> What is a data lake house?
<u>It's a new design paradigm recently created to have both (datalake and data warehouse) it the same place. It guarantee the data will be stored in a long term file storage/ processed in a parallel way with schema, data lineage and control of access. This way the data do not need to be copied a lot of times between places for each usage that could have (BI, application systems, Machine learning).</u>

:blue_book: <strong><b>57)</b></strong> What is your perception about the use of data in the near future?
<u>"data is the new oil." It means that companies around the word needs to have a data driven culture to continue alive.</u>

:blue_book: <strong><b>58)</b></strong> Why do you like working with data?
<u>I love to know that I'm working with the most important thing for a organization and to know that my work is important for them.</u>

:blue_book: <strong><b>59)</b></strong> What is Normalization?
<u>It's a database design to reduce data reduncancy.</u>

:blue_book: <strong><b>60)</b></strong> What is Denormalization?
<u>It's a database design to create redundancy on the data to increace performance on reads.</u>

:blue_book: <strong><b>61)</b></strong> What is OLTP?
<u>On-line Transactional Process - It's a type of data processing that consists of executing a number of transactions occurring concurrently.</u>

:blue_book: <strong><b>62)</b></strong> What are the differences between OLTP and OLAP?
<u>On-line Transational Process is used for performe writes for a transactional system and On-line Analytical Process is used for guarantee performance to query complex historical aggregated data.</u>

:blue_book: <strong><b>63)</b></strong> What are ACID properties?
<u>Atomicity - All changes to data are performed as if they are a single operation. Consistency - Data is in a consistent state when a transaction starts and when it ends. Isolation - The intermediate state of a transaction is invisible to other transactions. Durability - After a transaction successfully completes, changes to data persist and are not undone, even in the event of a system failure.</u>

:blue_book: <strong><b>64)</b></strong> What is NoSQL?
<u>It means "Not Only" SQL. It's uses CAP paradigm to decide two of three possibilities: Consistency, Availability, Partition Tolerance. We have 4 families of NoSQL: Document, Column-Oriented, Key-Value and Graph.</u>

:blue_book: <strong><b>65)</b></strong> Pros and Cons of SQL and NoSQL ?
<u>NoSQL will be more performatically and powerfull to write and query data. But it will lose some capabilities from transactional side. In the other hands, on transactional world it's possiblr to guarantee ACID complience easely.</u>

:blue_book: <strong><b>66)</b></strong> What is a View? (in SQL show us an example of use for views)
<u>View is a table expression on transactional database. It's a database object that encapsulate a query. It's most used for handle data access.</u>

:blue_book: <strong><b>67)</b></strong> What is DBMS?
<u>Database Management System is the computer software that enables storing, manipulating, managing and securing a large set of data.</u>

:blue_book: <strong><b>68)</b></strong> What is RDBMS? How is it different from DBMS?
<u>Technically Relational Database Management System is a type of Database Management System. The difference between them is RDBMS manages and maintains data in the tabular format.</u>

:blue_book: <strong><b>69)</b></strong> What is a Primary Key?  
<u>One of the 5 types of relational database column constraints. genarally used inside a clustered index. Garantes the value unicity of a single or composity key of table. Can be created in a Natural or Surrogate key.</u>

:blue_book: <strong><b>70)</b></strong> What is a UNIQUE constraint?
<u>it's another type of a database column constraint. it's inforce a single or composite columns can not have duplicated values.</u>

:blue_book: <strong><b>71)</b></strong> What is a Foreign Key?
<u>Another type of database column constraint. It's a reference of a Primary Key in another table. It's used to garantes consistence betweeen the tables reletionship.</u>

:blue_book: <strong><b>72)</b></strong> What is an Index? Explain its different types.
<u>Index it's a way to organize the database data pages. Relational databases have two types of indexes: clustered and nonclustered index. And in databases like SQL Server we can have a row or colummar way to create a index.</u>

:blue_book: <strong><b>73)</b></strong> What is the difference between Clustered and Non-clustered index?
<u>Clustered index are created using a single or a composite columns and the data saved inside the table will be organized based on it. In the other hands, the Non-clustered index will create a copy of the original pages of the table and will organize the data in this new set of pages based on the columns was choosen. The data in this new pages will have just the columns were selected and the primary key of the table to do a lookup with the clustered index when the query ask for a column that is not on the non-clustered index created. </u>

:blue_book: <strong><b>74)</b></strong> What is Data Integrity? 
<u>It's related to the reliability that the data has. it's possible to guarantee it in a physical and logical way.</u>

:blue_book: <strong><b>75)</b></strong> What are Entities and Relationships? <u>In database design one entity represents a set of information that is independent from another. Relationship is the way that we can merge this informations together to retrive data as it's needed.</u>

:blue_book: <strong><b>76)</b></strong> What are the TRUNCATE, DELETE and DROP statements?
<u>TRUNCATE is a DML operation that is minimal logged at the transaction log.This operation will delete all data at once and if the table has a identity it will be reinicialized. DELETE is a operation that will delete expecific rows at the table based on the WHERE clause. DROP is a DDL operation that will delete the table data and the table structured (schema). </u>


:blue_book: <strong><b>77)</b></strong> What are Aggregate and Scalar functions? 
<u>AGGREGATE function is a type that will use a set of rows returned to return a result (SUM and COUNT are examples). SCALAR function is a type of function that will execute row by row.</u>
