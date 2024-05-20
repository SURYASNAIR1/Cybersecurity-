**Name : SURYA S NAIR**

**Date : 11th May 2023**

**ASSIGNMENT 6 - Log analysis using SIEM - Splunk**

1. Understand the architecture of Splunk and the installation process. Setup collector and forwarder,then ensure the logs areaccumulated in Splunk. Familiarize yourself with the dashboard fields.

Ans :

The architecture of Splunk :

**Data Collection**: Splunk collects data from various sources, such as log files, network devices, APIs, and databases. This data can be sourced from both structured and unstructured formats, allowing organizations to gain insights from diverse data sets.

**Splunk Indexer**: The Splunk Indexer is responsible for indexing and storing the collected data. It breaks down the incoming data into events, assigns timestamps, and stores them in an optimized format for efficient searching and retrieval. The Indexer also performs data compression and maintains metadata for quick access.

**Search Head**: The Search Head is the user interface of Splunk. It provides a web-based interface for users to search, analyze, and visualize the indexed data. Users can create search queries, build reports and dashboards, and gain real-time insights from the data.

**Splunk Forwarder**: Splunk Forwarders are lightweight components that collect and forward data to the Splunk Indexer. They can be installed on source systems or dedicated servers, and they securely transmit the data over the network to the Indexer. Forwarders can handle data preprocessing, such as filtering and transforming, before sending it to the Indexer.

**Deployment Options**: Splunk offers flexible deployment options. It can be deployed as a single-instance setup where all components are installed on a single server, or it can be distributed across multiple servers for high availability and scalability. Splunk also supports distributed deployment configurations with multiple Indexers, Search Heads, and Forwarders to handle large-scale data processing.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/ab6fccd1-4984-474c-bf92-2ba8e260d978)

Here the universal forwarder is downloaded in kali linux and then we have forwarded log files into the splunk enterprise.

![1](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/f6e58e07-a8d7-4e79-87d7-ce936260c7c9)

![2](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/f661bbce-3c0e-4f69-bf93-26094b32f4ce)

![3](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/1fc29bc4-d1d2-4eaa-beb7-4b49d4f424a8)

![4](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/8a2a8d5e-2c1a-4e39-9c9a-443a52dbf5b7)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/d844e5a9-961e-407d-9066-432cd6b03ef3)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/46452f1a-ef55-4657-bd69-b097dad8a4b5)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/bedb58a4-0bd3-459d-9a82-862e583fbb8a)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/1ddc5336-59dd-4734-a7f2-c16ee8f2ad11)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/f5c3fea5-2953-4b98-85d5-d6b1273fe930)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/be8e1810-66f6-42e0-948f-6c65a3165f6d)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/0ee971ec-f5bd-4631-b628-2beb2a288e46)

2.Run Splunk >> Forwarder can be inthe same system or another system(user’s convenience) >>Make sure the logs are indexing in the Splunk enterprise.

•Run any network and port scanning commands from the host to the target machine. Run at least 5 to 8 commands. (If required,any tools can also beused).

•Use the search section in Splunk to analyze the firewall logs to findthe log of the above process and the exact IP from where the scan was performed. HINT: Use the “stats” command.

•Analyze the log file and create an alert for any further similar activities.

Ans : Here we have created scan.log file into the /var/log file .The nmap commands output is saved into the scan.log file by using nmapcommands>>scan.log the nmap commands are nmap -o ,-sV,-A,finding host in subnet is performed. the the logs are forwarded into the enterprise.the name of the log file is used to scan the log of nmap commands are done.

![WhatsApp Image 2023-05-11 at 23 03 24](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/b893ab35-a5dc-4b49-8e86-033fbfae9f28)

![WhatsApp Image 2023-05-11 at 23 04 00](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/b21f2ada-97e0-4a44-b1ba-11ab21b2f97a)

![WhatsApp Image 2023-05-11 at 23 05 12](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/ea4a04a1-74bf-4a4b-9172-706ea0b69e3d)

Runned nmap commands.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/ad427adf-7b6f-4963-92ed-4952cefc0788)

3. Run Splunk >> Forwarder can be in the same system or another system (user’s convenience) >>Make sure the logs are indexing in the Splunk enterprise. Perform any communication using unencrypted traffic.Use the Splunk search section to check the firewall logs to analyze which application uses unencrypted data.Analyze the log file and create an alert for any further similar activities.

Ans :
Here we have entered into the vulnerable website , the logs are saved and then forwarded the log into the splunk enterprise.In the splunk , we have searched query based on access.log.1 and the get request in the search query field,so we obtained the searches in the kali.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/b709cf66-3b7b-4981-92a1-17735722ab68)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/5432238d-e93a-4726-86c3-712052667ad8)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/a6df9f68-c2c2-40ef-8bd9-638bc56f9034)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/27763e48-7c8b-4fe0-8684-9a298000b838)

5. Run Splunk >> Forwarder can be in the same system or another system (user’s convenience) >>Make sure the logs are indexing in the Splunk enterprise.Logout of the target system and perform multiple failed attempts. Then use the search section to filter out the failed attempt logs. Hint: Use the “stats” command.Analyze the log file and create an alert for any further similar activities.Here we have tried to login into the kali ,then by analysing the log in the splunk forwarder,we can analyse by entering authentication in the query of splunk.

Ans :
![WhatsApp Image 2023-05-16 at 12 36 47](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/44dbb80c-7a3d-47f6-9320-a755989d9873)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/1b964cee-48a2-4447-bdf5-9c69047ef920)



