**Nmap (Network Mapper)** :

⦁	Is a footprinting tool or a reconnaissance tool.

⦁	It is used to get more information  about the target or the IP or the website.

⦁	It is mostly used by pentesters and hackers.

a) Explain the subnet and use the NMAP Command to scan the services for the whole subnet.

Ans : To scan the services for the whole subnet, you can use the following 
NMAP command: nmap -sV <subnet_address>/24
This will scan all the hosts in the subnet, and use the -sV flag to detect the version of the services running on each host.
The "/24" at the end of the subnet address specifies the subnet mask, indicating that the scan should include all hosts within the same Class C network.

![image](https://user-images.githubusercontent.com/123303806/226387050-79a648db-ff14-4ea4-829a-dbf85fad107b.png)

b) What is a firewall andmention its types. Use the NMAP command to detect that a firewall protects the host.

Ans : A firewall is a network security device that monitors and filters incoming and outgoing network traffic based on predetermined security rules. There are two main types of firewalls: network-based and host-based.

To detect if a firewall is protecting the host, you can use the following 
NMAP command:nmap -sA <host_address>
This will use the "ACK scan" (-sA) option to determine if the host is protected by a firewall that is blocking certain types of traffic.

![image](https://user-images.githubusercontent.com/123303806/226388067-fc959020-dbad-4060-8445-bd80e49b9e8c.png)


c) Use the NMAP command to scan a network and determinewhich devices are up and running.

Ans : To scan a network and determine which devices are up and running, you can use the following NMAP command:nmap -sn <network_address>
This will perform a "ping scan" (-sn), sending ICMP echo requests to all hosts in the network to see which ones respond.

![image](https://user-images.githubusercontent.com/123303806/226389160-8e0d7642-0d4c-4f8c-aefc-d5b92c5a1027.png)


d) What are vertical and horizontal scanning?

Ans : Vertical scanning involves scanning a single target for multiple ports and services, while horizontal scanning involves scanning multiple targets for a single port or service.
vertical and horizontal scanning refer to different techniques for exploring hosts and services on a local area network (LAN).

Horizontal scanning, also known as ping scanning, is a technique used to discover hosts that are alive and responsive on a network. It involves sending ICMP echo requests (pings) to all IP addresses in a given range and listening for responses. This allows the scanner to identify hosts that are up and running on the network, but it does not provide much detail about the services or applications running on those hosts.

Vertical scanning, on the other hand, is a more comprehensive technique that involves scanning a single host or a range of hosts for specific ports and services. This allows the scanner to obtain more detailed information about the services running on each host, including the version number and any vulnerabilities that may be present. Vertical scanning is more resource-intensive than horizontal scanning, as it requires probing each host and service individually, but it can provide more valuable information for vulnerability assessment and penetration testing.

In summary, horizontal scanning is used to quickly identify active hosts on a network, while vertical scanning is used to perform a more thorough analysis of the services and vulnerabilities present on those hosts. Both techniques are commonly used in local area network scanning and reconnaissance using Nmap.

e) Use the NMAP command to scan multiple hosts. [HINT: Add hosts into a file and scan it.

Ans : To scan multiple hosts, you can create a file containing the list of hosts (one per line), and then use the following NMAP command: nmap -sV -iL <filename>
The "-iL" option specifies the input file containing the list of hosts to scan.
  
  ![image](https://user-images.githubusercontent.com/123303806/226393113-61b50442-e37c-4d79-8c97-2f04352e3f0b.png)

  ![image](https://user-images.githubusercontent.com/123303806/226393202-5238950a-69bc-408c-835c-7145d4a0418b.png)

f) Use NMAP commands to export the output inXML format.
  
Ans : To export the output in XML format, you can use the following NMAP command:nmap -oX <output_filename> <target_address>
This will save the scan results in XML format to the specified output file.

  ![image](https://user-images.githubusercontent.com/123303806/226394068-edbbd224-6200-40bd-b97d-b44eeef56217.png)

g) Use the NMAP command to getOS information about a host.
  
Ans : ) To get OS information about a host, you can use the following NMAP command:nmap -O <host_address>
This will perform an OS detection scan (-O) to determine the operating system running on the target host.

  ![image](https://user-images.githubusercontent.com/123303806/226394720-06b06308-a381-4699-aee9-d9a19dfc03ef.png)

h) Explain ping sweeping and Perform ping sweeping using Nmap
  
  Ans : Ping sweeping involves sending ICMP echo requests to a range of IP addresses to determine which ones are active and responsive. To perform ping sweeping using NMAP, you can use the following command: nmap -sn <IP_range>
For example, to scan the range of IP addresses from 192.168.1.1 to 192.168.1.255, you would use the command:
nmap -sn 192.168.1.0/24
This will send ICMP echo requests to all IP addresses in the range, and report back which ones responded.
  
  ![image](https://user-images.githubusercontent.com/123303806/226402749-ece3a90b-d8d7-4818-9b03-28e3adedab0b.png)

  1.What is a web application firewall? How do you use Nmap to detect a WAF? Perform WAF fingerprint detection using NMAP.
  
Ans : A web application firewall (WAF) is a security tool that helps protect web applications by monitoring and filtering HTTP traffic between a web application and the Internet. It is designed to detect and block common web application attacks, such as SQL injection, cross-site scripting (XSS), and others. WAFs can be implemented as hardware appliances, software solutions, or cloud-based services.

  Nmap is a powerful network scanning tool that can be used to detect various network devices and services. To detect a WAF using Nmap, we can perform a WAF fingerprint detection scan. This involves sending HTTP requests with various payloads and analyzing the responses to identify common WAF signatures.
To perform a WAF fingerprint detection scan using Nmap, we can use the following command:nmap -p80 --script=http-waf-fingerprint <target_ip>
This command scans port 80 of the target IP address and runs the http-waf-fingerprint script to detect the presence of a WAF. The output of the scan will include information about the detected WAF, if any.

Note that this method of detecting WAFs may not always be accurate, as some WAFs may not leave clear fingerprints. Additionally, some WAFs may be configured to hide their presence, making them more difficult to detect. It is always important to use multiple security measures and tools to ensure comprehensive web application security.

  ![image](https://user-images.githubusercontent.com/123303806/226403657-cac71b49-ad25-4b7c-9a68-030684020633.png)
  
  ![image](https://user-images.githubusercontent.com/123303806/226403751-17322a74-6559-448d-97cb-eedcf4be9cc5.png)

  2.What is EXIF data? Tryto find EXIF data of images on a website using NMAP NSE.
  
  Ans : :EXIF (Exchangeable Image File Format) is a metadata standard used in digital photography. It stores information about various parameters related to the image, such as camera make and model, aperture, shutter speed, ISO, and more.

Nmap includes a script called http-exif-spider in the NSE (Nmap Scripting Engine) that can be used to extract EXIF data from images on a website. This script scans a web server for image files and extracts their EXIF metadata. Here's an example command to use the http-exif-spider script:
nmap --script=http-exif-spider <target_website>
Replace <target_website> with the website URL you want to scan. This command will scan the website for image files and extract the EXIF data from them.
Note that this script requires that the website has publicly accessible images with EXIF data. It may not be able to extract data from images that are stored in a format that does not support EXIF, or images that have had their metadata removed or altered. Additionally, this script may not work on websites that require authentication or have other security measures in place.

  ![image](https://user-images.githubusercontent.com/123303806/226404061-62b5d236-66ab-4639-a619-6d90737d7201.png)

  ![image](https://user-images.githubusercontent.com/123303806/226404138-24ee8d26-58f2-4737-a5fa-a18176f98884.png)

  3.Use NMAP NSE to find all subdomains of the website. 

Ans : To find all subdomains of a website using Nmap, we can use the dns-brute script in the Nmap Scripting Engine (NSE). This script will perform a brute-force subdomain enumeration by querying a DNS server for a large number of possible subdomains.

Here's an example command to use the dns-brute script:
nmap --script dns-brute <target_website>
Replace <target_website> with the website URL you want to scan. This command will use a default wordlist of subdomains to query against the target DNS server. You can also specify a custom wordlist using the dns-brute.wordlist script argument.

Note that this script can generate a large number of DNS queries and may trigger security alerts from some network monitoring tools. Additionally, this script may not work on websites that have implemented measures to prevent subdomain enumeration, such as rate limiting or DNS query filtering.

  ![image](https://user-images.githubusercontent.com/123303806/226404469-61f03c9d-3148-4473-bf6d-74b2cfc294c0.png)
  
  ![image](https://user-images.githubusercontent.com/123303806/226404558-8f62fae9-87c3-4d90-9273-a612a055dca6.png)
  
4.Perform a vulnerability scan on the target host using NMAP NSE.
  
Ans: Nmap includes a variety of scripts in the Nmap Scripting Engine (NSE) that can be used to perform vulnerability scans on target hosts. Here's an example command to use some of these scripts:
nmap --script vuln <target_host>
Replace <target_host> with the IP address or hostname of the host you want to scan for vulnerabilities. This command will run a selection of vulnerability-related NSE scripts against the target host.

Note that this command will not detect all vulnerabilities on the target host, as the scripts in the NSE are limited in their coverage. It is important to use multiple tools and techniques to ensure comprehensive vulnerability detection and remediation. Additionally, it is important to obtain permission before scanning a host for vulnerabilities, as unauthorized scanning can be illegal and result in serious consequences.
  
  ![image](https://user-images.githubusercontent.com/123303806/226404812-2e857b20-1cbf-4b33-9e54-9bacd9385b83.png)


  



  
