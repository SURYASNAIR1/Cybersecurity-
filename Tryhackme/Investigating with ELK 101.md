**NAME : SURYA S NAIR**

**ROLL NUMBER : CB.EN.P2CYS22007**

                                               **Investigating with ELK 101**

Learning Objectives : 

How to utilize the Kibana interface to search, filter, and create visualizations and dashboards, while investigating VPN logs for anomalies. 

 overview of Elasticstack components and how they work together.

**Elastic stack**

Elastic stack is the collection of different open source components linked together to help users take the data from any source and in any format and perform a search, analyze and visualize the data in real-time.

**Elasticsearch**

Elasticsearch is a full-text search and analytics engine used to store JSON-formated documents. Elasticsearch is an important component used to store, analyze, perform correlation on the data, etc. Elasticsearch supports RESTFul API to interact with the data.

**Logstash**

Logstash is a data processing engine used to take the data from different sources, apply the filter on it or normalize it, and then send it to the destination which could be Kibana or a listening port. A logstash configuration file is divided into **three parts**.

The **input part** is where the user defines the source from which the data is being ingested. 

The **filter part** is where the user specifies the filter options to normalize the log ingested above. 

The **Output part** is where the user wants the filtered data to send. It can be a listening port, Kibana Interface, elasticsearch database, a file, etc.

**Beats**

Beats is a host-based agent known as Data-shippers that is used to ship/transfer data from the endpoints to elasticsearch. Each beat is a single-purpose agent that sends specific data to the elasticsearch.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/38236615-24c4-4cf7-94c3-a8c027ca4452)

**Kibana**

Kibana is a web-based data visualization that works with elasticsearch to analyze, investigate and visualize the data stream in real-time. It allows the users to create multiple visualizations and dashboards for better visibility—more on Kibana.

How they work together:

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/d83e2190-9ba9-4b23-bef2-91f18a5f58a2)

Beats is a set of different data shipping agents used to collect data from multiple agents. Like Winlogbeat is used to collect windows event logs, Packetbeat collects network traffic flows.
Logstash collects data from beats, ports or files, etc., parses/normalizes it into field value pairs, and stores them into elasticsearch.
Elasticsearch acts as a database used to search and analyze the data.
Kibana is responsible for displaying and visualizing the data stored in elasticsearch. The data stored in elasticseach can easily be shaped into different visualizations, time charts, infographics, etc., using Kibana.



![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/d4d112cb-70b2-4f22-bf7b-bcbc52271a0c)
