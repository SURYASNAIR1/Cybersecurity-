**21CY683 - CYBER SECURITY LAB - III**

**Name: Surya S Nair**

**Date: 27th March 2023**
 
**Assignment Topic: LAN based insider attacks**


*Make use of Ettercap/arpspoof tool to perform ARP Cache Poisoning based attacks in a LAN environment*:

**1.Perform Password stealing (over plaintext) using ARP Cache Poisoning attacks.**

Ans: Arp means Address Resolution Protocol.

ARP Cache Poisoning is a type of attack where an attacker sends fake Address Resolution Protocol messages to a local network.

These messages are used to map an IP address to a MAC address in a network.

An attacker can use ARP Cache Poisoning to modify the ARP tables of a victim's computer and redirect its network traffic to the attacker's machine.

In the case of password stealing, the attacker can use ARP Cache Poisoning to intercept the victim's login credentials. 

When a victim tries to log in to a website or service, the victim's computer sends the login credentials over the network in plaintext. 
The attacker can intercept these plaintext credentials using ARP Cache Poisoning and use them to log in to the victim's account.

Here Iam using ettercap tool to perform ARP poisoning.

Ettercap and arpspoof are two tools commonly used for ARP Cache Poisoning attacks.
Ettercap is a network security tool that allows the user to sniff and intercept network traffic. 

It can be used to perform ARP Cache Poisoning attacks, and it supports various plugins for password sniffing, including HTTP, FTP, and Telnet.
Arpspoof is a simple command-line tool that can be used to redirect network traffic to the attacker's machine.

To perform ARP Cache Poisoning and password stealing using these tools, the attacker needs to follow the steps:

Identify the victim's IP address and MAC address.
Use arpspoof to redirect the victim's network traffic to the attacker's machine.
Use Ettercap to sniff the network traffic and intercept the victim's login credentials.
Use the stolen credentials to log in to the victim's account.

![5](https://user-images.githubusercontent.com/123303806/227956561-7d00c49d-dacf-4e66-ad62-3ca1a599e7ae.png)

![1st qz ans 1](https://user-images.githubusercontent.com/123303806/227957167-4177ebfd-60d3-4e30-b4c6-9fd8e4f2744b.png)

![6](https://user-images.githubusercontent.com/123303806/227957764-d7138173-5825-4048-ba4a-deed416095b6.png)

![2](https://user-images.githubusercontent.com/123303806/227958119-29e89b78-c97d-42da-a925-ab1e532c2336.png)

![3](https://user-images.githubusercontent.com/123303806/227958447-e2f04cdc-579c-4687-8dec-c0bff5aef82e.png)

![3](https://user-images.githubusercontent.com/123303806/227958594-444c285b-b40c-4e01-87bf-5047103d0c89.png)

![4](https://user-images.githubusercontent.com/123303806/227958971-3d1a9809-5183-4276-b494-df7ef74ccba4.png)

![1](https://user-images.githubusercontent.com/123303806/227959243-995df8f8-478c-4fc4-a20a-d0c6e51629fc.png)

![7](https://user-images.githubusercontent.com/123303806/227959447-b15e798c-a604-4010-b66e-e000deab55b3.png)


**2.Perform Denial of Service (DoS) attacks using ARP Cache Poisoning attacks .**

Ans : ARP Cache Poisoning, also known as ARP Spoofing, is a technique used to intercept network traffic by manipulating the ARP tables of devices on a local network. The attacker can use this technique to redirect traffic to their own machine, allowing them to intercept sensitive information such as passwords and other confidential data.

Ettercap is a tool that is widely used for ARP Cache Poisoning attacks. It is an open-source tool that runs on both Windows and Linux and can be used to perform a variety of network attacks, including sniffing, spoofing, and man-in-the-middle attacks.

To perform an ARP Cache Poisoning attack using Ettercap, you can follow these steps:

Install and configure Ettercap on your machine.

Identify the IP addresses of the target machines that you want to attack.

Use the arpspoof tool, which is included with Ettercap, to spoof the ARP tables of the target machines. This will redirect network traffic to your machine.

To perform a DoS attack using ARP Cache Poisoning, you can use Ettercap to flood the network with ARP packets. This will cause the ARP tables of all machines on the network to become corrupted, resulting in a DoS attack.


![2qz ans 1st scrnsht](https://user-images.githubusercontent.com/123303806/227954900-e2a2fef8-d815-445a-8464-a326fd5637c3.png)

![2nd qz ans 2nd scrnsht](https://user-images.githubusercontent.com/123303806/227954960-3e350a5f-907b-40f4-952a-23edccd77c7f.png)

![2nd qz ans 3rd scrnsht](https://user-images.githubusercontent.com/123303806/227955036-1a2b63b4-6c0d-41a9-b988-ed52c60db040.png)

![2nd qz ans 4th scrnsht](https://user-images.githubusercontent.com/123303806/227955068-6a7f97cd-407e-4f4c-ad10-f1e974cf9082.png)

![2nd qz 5th scrnsht](https://user-images.githubusercontent.com/123303806/227955109-0ac16eed-d57c-4c59-bfbd-52ce8e9ed732.jpg)

**3.Perform DNS Spoofing attack using ARP Cache Poisoning attacks.**

Ans : DNS Spoofing is a technique used to redirect network traffic from legitimate websites to malicious websites by modifying DNS records. Attackers can use this technique to steal sensitive information such as usernames, passwords, and credit card details. ARP Cache Poisoning can be used to perform DNS Spoofing by redirecting traffic to a machine that is running a fake DNS server.

To perform a DNS Spoofing attack using Ettercap and ARP Cache Poisoning, you can follow these steps:

Install and configure Ettercap on your machine.

Identify the IP addresses of the target machines that you want to attack.

Use the arpspoof tool, which is included with Ettercap, to spoof the ARP tables of the target machines. This will redirect network traffic to your machine.

Use Ettercap to intercept and modify DNS traffic.

Once the ARP tables of the target machines have been spoofed, you can use Ettercap to intercept and modify DNS traffic. Ettercap provides a wide range of options for intercepting and modifying DNS traffic, including sniffing packets, filtering traffic based on protocol or content, and even injecting packets into the network.

  ![3rd qz ans 1st scrnsht](https://user-images.githubusercontent.com/123303806/227955769-00fe1328-0243-49da-a9a2-7cdbcf2eeb34.png)

  ![3rd qz ans 2nd scrnsht](https://user-images.githubusercontent.com/123303806/227955802-54153ddd-cf2e-4803-bfc6-5da31ae71d5d.png)

  ![3rd qz ans 3rd scrnsht](https://user-images.githubusercontent.com/123303806/227955833-d725e1d0-7718-40d3-80e0-72bc70a1c79f.png)

  ![3rd qz ans 4th scrnsht](https://user-images.githubusercontent.com/123303806/227955865-c02825d7-f272-4775-851d-eb8eca33d60c.png)

  ![3rd qz ans 5th scrnsht](https://user-images.githubusercontent.com/123303806/227955905-c5e67acb-3de7-45b2-9ed3-5c348384b4db.png)

  ![3rd qz ans 6th scrnsht](https://user-images.githubusercontent.com/123303806/227955940-06c38057-d07c-4cb9-bf82-934327f6c313.png)


**4.Invoke ‘sslstrip tool’ for stealing passwordsfrom any machine that is connected toa LAN by stripping the HTTPSconnection.**
  
Ans: The sslstrip tool is a tool that can be used to perform a man-in-the-middle attack on HTTPS connections by stripping the encryption from the traffic. This allows an attacker to intercept and read sensitive information such as usernames and passwords.

To use Ettercap and ARP Cache Poisoning to invoke the sslstrip tool, you can follow these steps:

Install and configure Ettercap on your machine.

Identify the IP addresses of the target machines that you want to attack.

Use the arpspoof tool, which is included with Ettercap, to spoof the ARP tables of the target machines. This will redirect network traffic to your machine.

![4th qz ans 1 scrnsht](https://user-images.githubusercontent.com/123303806/227992294-e7501e5c-08c7-45e2-8e62-bfbc6108518d.png)

![4th qz ans 2nd scrnsht](https://user-images.githubusercontent.com/123303806/227992334-371dd6a9-52a4-4082-a3a8-3e9d1efa5587.png)

![4th qz ans 3rd scrnsht](https://user-images.githubusercontent.com/123303806/227992382-14702193-e1c0-4333-a70a-a8800d546964.png)

![4th qz ans 4th scrnsht](https://user-images.githubusercontent.com/123303806/227992418-809264c2-4a92-4039-be11-8a69698475d6.png)

![4th qz ans 5th scrnsht](https://user-images.githubusercontent.com/123303806/227992465-f8118095-6b78-421b-8f1c-fcfbba0dedda.png)

![image](https://user-images.githubusercontent.com/123303806/227994185-2e87c802-9070-4991-9879-546f30a40fea.png)

**5.Use arp_cop and scan_poisoner plugins to learn about the detection of ARP attacks.**
  
Ans: The arp_cop and scan_poisoner plugins are useful tools in Ettercap that can be used to detect ARP Cache Poisoning attacks.

To use the arp_cop plugin follow these steps:

Open a terminal window and start Ettercap.

Once Ettercap has started, click on the "Sniff" menu and select "Unified Sniffing".

In the "Unified Sniffing" window, select the network interface that you want to use and click on the "Start" button.

Once the sniffing session has started, click on the "Plugins" menu and select "Manage the plugins".

In the "Manage the plugins" window, select the "arp_cop" plugin and click on the "Enable" button.

Once the arp_cop plugin has been enabled, Ettercap will monitor the network for ARP Cache Poisoning attacks. If an attack is detected, Ettercap will display a warning message.

To use the scan_poisoner plugin, you can follow these steps:

Open a terminal window and start Ettercap.

  Once Ettercap has started, click on the "Sniff" menu and select "Unified Sniffing".

In the "Unified Sniffing" window, select the network interface that you want to use and click on the "Start" button.

Once the sniffing session has started, click on the "Plugins" menu and select "Manage the plugins".

In the "Manage the plugins" window, select the "scan_poisoner" plugin and click on the "Enable" button.

Once the scan_poisoner plugin has been enabled, Ettercap will scan the network for hosts that are sending out ARP packets. If a host is detected that is sending out a large number of ARP packets, Ettercap will display a warning message.

Both the arp_cop and scan_poisoner plugins can be used to detect ARP Cache Poisoning attacks in a LAN environment. However, it is important to note that these plugins are not foolproof and may not detect all attacks. It is still important to take other security measures, such as using encryption and strong passwords, to protect your network.

![5 th 1st](https://user-images.githubusercontent.com/123303806/228022361-06bb71da-c983-4745-96ec-2dd04aa5827b.png)

![5th 2nd 1](https://user-images.githubusercontent.com/123303806/228022475-57ea5ce0-d37e-4aaa-9179-fe1f64d8f611.png)


  
