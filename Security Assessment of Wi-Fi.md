**21CY683 - CYBER SECURITY LAB - V**

**Name: Surya S Nair**

**Date: 8th April 2023**
 
**Assignment Topic: Security Assessment of Wi-Fi**


Wi-Fi, short for wireless fidelity, is a technology that allows devices to connect to the internet or other networks without the need for wires or cables. It uses radio waves to transmit data between devices and a wireless access point, which is connected to the internet or a network.Wi-Fi is the most widely used wireless technology that connects devices to the internet or other networks.Wi-Fi networks are susceptible to security vulnerabilities that can lead to data breaches and other security incidents. Therefore, conducting a security assessment of Wi-Fi networks is essential to identify potential vulnerabilities and protect against security threats.

1.Learn the basic working of Wi-Fi and its types with various types of attacks on it. 

Ans : Wi-Fi works by using radio waves to transmit data between devices and a wireless access point, which is connected to the internet or a network. The access point acts as a central hub that allows devices to connect to the network and communicate with each other.When a device wants to connect to a Wi-Fi network, it sends a request to the access point. The access point then assigns the device an IP address and allows it to communicate with other devices on the network.The data that is transmitted between devices and the access point is encrypted using various security protocols, such as WEP, WPA, and WPA2. Encryption helps to protect the data from being intercepted and read by unauthorized parties.Wi-Fi networks can operate in different frequency bands, such as 2.4 GHz and 5 GHz. The frequency band determines the range and speed of the network. For example, 2.4 GHz networks have a longer range but a slower data transfer rate, while 5 GHz networks have a shorter range but a faster data transfer rate.Overall, Wi-Fi provides a convenient and flexible way to connect devices to the internet or a network without the need for wires or cables.

Types of Wi-Fi networks:

**a.Public Wi-Fi**: This type of Wi-Fi network is available in public places such as coffee shops, airports, and hotels, and can be accessed by anyone. It is typically unsecured, which means that it is not encrypted, making it vulnerable to attacks.

**b.Private Wi-Fi**: This type of Wi-Fi network is typically used in homes and businesses, and is secured using a password or other authentication methods.

**c.Guest Wi-Fi**: This type of Wi-Fi network is often set up in businesses to allow visitors to connect to the internet without having access to the business's main network.

Types of Wi-Fi attacks:

**a.Eavesdropping**: This attack involves intercepting Wi-Fi traffic to steal sensitive information such as passwords, credit card numbers, or other personal data.

**b.Man-in-the-middle (MITM) attack**: This attack involves intercepting and modifying Wi-Fi traffic to gain access to sensitive information.

**c.Rogue access point**: This attack involves setting up a fake Wi-Fi network to trick users into connecting to it and stealing their data.

**d.Denial-of-service (DoS) attack**: This attack involves overwhelming a Wi-Fi network with traffic to disrupt its normal operation.

**e.Password cracking**: This attack involves using software to guess or crack the Wi-Fi network's password and gain access to the network.

**f.Packet injection**: This attack involves injecting malicious packets into a Wi-Fi network to exploit vulnerabilities and gain unauthorized access.


2.Perform Wi-Fi fingerprinting using Wigile, Inssider, and Kismet.

Ans : Wi-Fi fingerprinting is the process of gathering information about the Wi-Fi access points and their characteristics in a particular area. This information includes the Service Set Identifier (SSID), Media Access Control (MAC) address, signal strength, and other parameters that can be used to identify and locate APs. This information can be used for a variety of purposes, such as improving network performance, enhancing security, and location-based services.

Wigile, Inssider, and Kismet are all tools that can be used to perform Wi-Fi fingerprinting.

Wigile is an open-source tool that can be used to map Wi-Fi networks and their characteristics. It uses a GPS device to collect location information and a wireless adapter to capture information about nearby Wi-Fi networks. Wigile can identify the SSID, MAC address, channel, encryption type, and signal strength of the nearby networks.

![image](https://user-images.githubusercontent.com/123303806/230722300-6af031f5-bfe6-421d-90e5-ca152ba3239a.png)

Aircrack-ng is a set of tools in Kali Linux that can be used to assess Wi-Fi network security. It is capable of monitoring (capturing packets), attacking, and cracking Wi-Fi networks

![image](https://user-images.githubusercontent.com/123303806/230722308-db3fd608-2204-4d7a-9566-f8ac98cb08f7.png)

Use airodump to capture packet.

![image](https://user-images.githubusercontent.com/123303806/230722318-1afe1d29-356c-4001-9a3e-4860efe0128c.png)

Inssider is a commercial tool that provides a graphical representation of Wi-Fi networks in the area. It uses a wireless adapter to capture information about nearby networks and displays the information in a user-friendly interface. Inssider can identify the SSID, MAC address, channel, encryption type, and signal strength of the nearby networks.

![WhatsApp Image 2023-04-08 at 22 47 10](https://user-images.githubusercontent.com/123303806/230734422-2d7044d9-f1db-4561-b343-cbd686f295f2.jpg)


Kismet is an open-source tool that can be used for network discovery, packet sniffing, and intrusion detection. It can be used to capture and analyze wireless traffic in the area and provide detailed information about nearby Wi-Fi networks. Kismet can identify the SSID, MAC address, channel, encryption type, and signal strength of the nearby networks.

![image](https://user-images.githubusercontent.com/123303806/230722246-081410e6-010b-4cb2-b450-4ddf6d6c87da.png)

iwconfig is similar to ifconfig, but is dedicated to wireless networking interfaces.

![image](https://user-images.githubusercontent.com/123303806/230722254-d2388bf6-9be2-4120-bd4d-684aaffb1ed3.png)

 Display and modify IP Addresses using ip a command.

![image](https://user-images.githubusercontent.com/123303806/230722259-5c789eed-9b77-4ed6-95c6-254cfc480072.png)

Airmon-ng utility is a command-line tool used to enable monitor mode on wireless interfaces. It can also be used to switch back from Monitor mode to Managed Mode.Monitor Mode allows the wireless adapter to view the traffic on wireless networks.iwconfig is used to set the parameters of the network interface which are specific to the wireless operation.

![image](https://user-images.githubusercontent.com/123303806/230722282-41d26708-414f-4e1b-aa68-3a9b7204d9bb.png)

![image](https://user-images.githubusercontent.com/123303806/230722270-07235d26-7379-4b69-94ae-bfca72f17849.png)

The sudo kismet -c wlan0 command is a Linux command that launches the Kismet wireless network detector and sniffer program on the specified wireless network interface wlan0 with root privileges The "-c" option in the command specifies the channel on which the wireless interface should operate. 

![image](https://user-images.githubusercontent.com/123303806/230722288-6d3590b5-efd9-4dd1-bb62-a52050792cab.png)


Install Aircrack-ng suite by running the following command in the terminal:

sudo apt-get install aircrack-ng

Put your wireless interface in monitor mode using the following command:

sudo airmon-ng start wlan0

Start scanning for Wi-Fi networks using the following command:

sudo airodump-ng wlan0mon

Once the scan is complete, press CTRL+C to stop the scan.

Use the following command to export the scan results to a CSV file:

sudo airodump-ng -w output --output-format csv wlan0mon

Note: Replace output with the name of the file you want to save the results to.

Use the WiGLE website to upload the CSV file and view the results.

a. Log in to the WiGLE website (https://wigle.net/).

b. Click on the "Upload" button in the top menu bar.

c. Select the CSV file that you exported in step 5.

d. Click on the "Upload" button to upload the file.

3.Create an Access point with any Wi-Fi encryption standard and start testing the security of that connection using any Wi-Fi security testing tools,which should include (Aircrack-Ng, Wifite, not limited).Try to capture the 4-way handshake using these methods.

Ans : Wi-Fi Encryption Standards:

**a.** Wired Equivalent Privacy (WEP)

**b.** Wi-Fi Protected Access (WPA)

**c.** Wi-Fi Protected Access II (WPA2)
**d.** Wi-Fi Protected Access III (WPA3)

Wi-Fi Security Testing Tools:

**a.** Aircrack-ng: A suite of tools used to assess Wi-Fi network security. It includes packet sniffer, a detector for wireless LANs, WEP and WPA/WPA2-PSK cracker, and an analysis tool for 802.11 wireless LANs.

**b.** Wifite: An automated tool used to attack multiple wireless networks encrypted with WEP, WPA/WPA2-PSK.

**c.** Reaver: A tool that cracks WPS (Wi-Fi Protected Setup) keys and allows attackers to gain access to a wireless network using a PIN.

**d.** Wireshark: A network protocol analyzer that captures network traffic in real-time and displays it in a human-readable format.

![image](https://user-images.githubusercontent.com/123303806/230722594-acf00776-1bd1-4db3-8327-aee0bcc7802b.png)

Putting a wired adapter into promiscuous mode. It allows us to see all of the wireless traffic that passes by us in the air. 

![image](https://user-images.githubusercontent.com/123303806/230722600-66090f36-daf1-41d8-a22a-6256c0173dd3.png)

 Grab that traffic by simply using the airodump-ng command.
 
![image](https://user-images.githubusercontent.com/123303806/230722606-ced84e51-8951-4235-9527-8b5b560a45c8.png)

Focus Airodump-Ng on One AP on One Channel.We need the BSSID and channel to do this.

![image](https://user-images.githubusercontent.com/123303806/230722614-7537c96e-05eb-4465-acd5-e2807a83a2bf.png)

In order to capture the encrypted password, we need to have the client authenticate against the AP. If they're already authenticated, we can de-authenticate them (kick them off) and their system will automatically re-authenticate, whereby we can grab their encrypted password in the process.

![image](https://user-images.githubusercontent.com/123303806/230725217-f7b6486b-f3de-4ee2-bc11-39920ee36fc9.png)

Capture the Handshake.

![image](https://user-images.githubusercontent.com/123303806/230722632-09caf9f7-4f1a-4745-9c3d-daa47d4defce.png)

Aircrack-Ng That Password.

![image](https://user-images.githubusercontent.com/123303806/230722637-e6a505ca-9582-429b-a820-3bf56fad4447.png)

4.After capturing the required files for testing, use dictionary generation and password cracking tools to crack the Wi-Fi password.

a.You must use an existing word file to crack the password.

b.Also you have to create your dictionary file for cracking the passwords.

c.Keep 3 different types of passwords for your Wi-Fi to test it. Simple, medium,and complex passwords can be used for testing. Simple can be a dictionary word, medium can be of dictionary word with some numbers, and complex can be generated from any password generator online.

Ans : Passwords can be brute-forced but it is probably more efficient to use a dictionary. In Kali, wordlists can be found in /usr/share/wordlists. Fasttrack is good for testing weak passwords.

Here I have used an existing word file to crack password.Here we used the command aircrack-ng WPAcrack-03.csv -w fasttrack.txt from this we got the password.

![image](https://user-images.githubusercontent.com/123303806/230725999-725dd0b4-0da3-42dd-92c7-3b0975df9674.png)

![image](https://user-images.githubusercontent.com/123303806/230726005-0d4e1a8e-f8bb-4e83-a5ff-a5f10dc1b9ea.png)

![image](https://user-images.githubusercontent.com/123303806/230726014-68f059e4-6df5-47c7-a030-da049df68f63.png)

![image](https://user-images.githubusercontent.com/123303806/230726022-141044bf-f25b-493b-ad2d-f2d8560b6792.png)

![WhatsApp Image 2023-04-08 at 21 12 53](https://user-images.githubusercontent.com/123303806/230730329-956b3af7-4d0c-4ed7-8631-13955a78d052.jpg)

![image](https://user-images.githubusercontent.com/123303806/230726033-8ab72e2a-6143-400a-afe8-5d0a5bbf362b.png)

Here we have created a txt file which contains some possible passwords and then we tried to crack it.

5.Use Rouge AP (WifiPhisher) to create an Evil twin, perform a basic phishing attack using this rouge AP,and document the difference between the two attacks you have performed.

Ans : ![image](https://user-images.githubusercontent.com/123303806/230726047-465c2df1-f362-4dbc-b29d-fbd78909faa3.png)

6.Learn the protocol level working of WPA3 and how it differs from WPA2.

Ans : WPA3 (Wi-Fi Protected Access 3) is the latest security protocol for Wi-Fi networks, designed to improve upon the previous security standard, WPA2.The WPA3 protocol is designed to address the vulnerabilities and shortcomings of WPA2, which had become increasingly susceptible to attacks due to the hacking techniques.

**a.** Stronger Encryption: WPA3 uses the more secure encryption protocol, Simultaneous Authentication of Equals (SAE), which is also known as Dragonfly. SAE uses a stronger Diffie-Hellman key exchange algorithm and provides forward secrecy, which makes it much harder for hackers to intercept and decrypt Wi-Fi traffic.

**b.** Protection Against Offline Attacks: In WPA2, an attacker can capture the Wi-Fi traffic and use offline brute-force techniques to try and guess the Wi-Fi password. WPA3 addresses this vulnerability by implementing a feature called Simultaneous Authentication of Equals (SAE) which uses a key derivation function to protect against offline dictionary attacks.

**c.** Improved Authentication: WPA3 introduces a new feature called Opportunistic Wireless Encryption (OWE), which provides encrypted connections without requiring authentication from users. OWE is designed to provide a more secure connection for public Wi-Fi networks, where it can be difficult to distribute pre-shared keys (PSKs) to users.

**d.** Better Protection Against Password Guessing: WPA3 strengthens the protection against password guessing attacks by implementing a feature called Protected Management Frames (PMF). PMF helps to prevent unauthorized devices from connecting to the network by verifying the authenticity of devices before allowing them to connect.

**e.** Enhanced Protection for IoT Devices: WPA3 also includes a new feature called Wi-Fi Easy Connect, which provides a simpler and more secure method for connecting IoT devices to Wi-Fi networks. Wi-Fi Easy Connect eliminates the need for users to manually enter long and complex passwords by allowing devices to use a QR code to connect to the network.
