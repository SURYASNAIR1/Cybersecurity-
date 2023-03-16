Kali Linux is a popular operating system for ethical hacking and penetration testing. It comes with a variety of tools and utilities that are designed for different purposes.Here I have listed out the tools which are present in Kali Linux.

**1.Information Gathering**:

Information gathering is an important part of Ethical Hacking, where penetration testers or hackers try to get more information about the target so as to increase the probability of a successful attack.It is also a method used by analysts to determine the needs of customers and users.

**a.DNS Analysis**:

DNS or Domain Name System analysis is the process of examining the DNS infrastructure of a target domain or network to gather information about its DNS servers, subdomains, and other related information.

*i.dnsenum* :

⦁	Is used for enumerating DNS information about a domain. 

⦁ It can be used to identify DNS servers, DNS zone transfers, and email servers associated with a domain.

⦁	The tool performs a series of DNS queries to retrieve information about the domain, such as its IP addresses, subdomains, and email addresses. 

⦁ It uses a combination of DNS queries and other techniques to gather this information.

⦁	DNSenum can be used to identify potential security vulnerabilities associated with a domain. 

⦁	DNSenum is a powerful tool that can be used for reconnaissance and information gathering during penetration testing or vulnerability assessments. 

**b.IDS / IPS**:

One of the most popular tools for identifying and preventing security threats is the Intrusion Detection System/Intrusion Prevention System (IDS/IPS) identification tool. IDS/IPS identification tools in Kali Linux allow users to customize the rules used to identify threats. IDS/IPS identification tools in Kali Linux can be integrated with other security tools, such as firewalls and anti-virus software, to create a comprehensive security solution. 

*i.lbd* :

⦁	LBD stands for Load Balancing Detector.

⦁ Is a tool used to detect if a website is using load balancing. 

⦁ Load balancing is a technique used to distribute incoming traffic across multiple servers to improve performance and reliability.

⦁	LBD in Kali Linux works by sending a series of requests to a website and analyzing the responses.

⦁ It looks for patterns in the responses that indicate load balancing, such as the use of multiple IP addresses or different server names.

⦁ LBD can be used to detect load balancing on both HTTP and HTTPS websites. 

⦁	LBD is a useful tool for website administrators and security professionals to test the load balancing configuration of their websites.

⦁	It can also be used to test for load balancing on multiple ports, such as port 80 for HTTP traffic and port 443 for HTTPS traffic.

**c.Live Host Identification** :

Live Host Identification is a technique used to determine whether a particular IP address is currently active and responding to network traffic. This is important for network administrators who need to maintain an accurate inventory of active hosts on their network.

*i.Arping*:

⦁	Arping is a command-line tool in Kali Linux used for discovering and probing hosts on a network.

⦁	It is similar to the traditional "ping" tool but uses ARP (Address Resolution Protocol) instead of ICMP (Internet Control Message Protocol).

⦁	Arping sends out ARP requests to a specific IP address or a range of IP addresses on the network to check whether the target host is available and active. 

⦁	It can also be used to discover the MAC (Media Access Control) address of a host.

⦁	Arping in Kali Linux can be run in two modes: ARP request mode and ARP reply mode.

⦁	The ARP request mode sends out ARP requests to a specified target, while the ARP reply mode listens for incoming ARP requests and replies to them.

⦁	Arping can be used to detect duplicate IP addresses on the network, which can cause network connectivity issues. 

⦁	Arping is a simple and lightweight tool that is easy to use. 

**2.Vulnerability Analysis**:

Kali Linux is a popular operating system used by security professionals and ethical hackers for various penetration testing activities. One of the essential components of any security assessment is vulnerability analysis. A vulnerability analysis tool helps in identifying vulnerabilities in a system, application, or network that could potentially be exploited by attackers.

**a.Fuzzing**:

Is a testing technique that involves sending random or malformed data to a software application to identify potential vulnerabilities. Fuzzing is an essential component of software testing and can be used to test the security and stability of applications. 

*i.spike-generic_chunked* :

⦁	Spike is a powerful fuzzer and network protocol testing tool that includes various components including spike-generic_chunked.

⦁	Spike-generic_chunked is specifically designed to test applications that use the chunked transfer encoding for HTTP data.

⦁	The tool can be used to generate random or user-defined chunks of data to test an application's handling of the chunked transfer encoding.

⦁	The spike-generic_chunked tool is a powerful addition to Spike's suite of tools.

⦁	It can be used to test the security and stability of applications that use the chunked transfer encoding for HTTP data. 

**b.VoIP Tools** :

*i.voiphopper* :

⦁	voiphopper is a VoIP security testing tool that comes pre-installed in Kali Linux.

⦁	The tool is designed to test the security of VoIP networks by hopping between Wi-Fi access points and spoofing the MAC addresses of the wireless interface.

⦁	voiphopper can capture and analyze VoIP traffic over Wi-Fi, including SIP and RTP protocols, and it includes features for detecting and exploiting vulnerabilities in VoIP systems.

⦁	To use the tool, you must configure it with the MAC addresses of the Wi-Fi access points to hop between, as well as the IP address of the target VoIP system. 

⦁	The voiphopper tool is a powerful addition to Kali Linux's suite of VoIP testing tools and can be used to test the security of VoIP networks and systems. 

**c.nikto**:

⦁	nikto is an open-source web server scanner that comes pre-installed in Kali Linux.

⦁	The tool is designed to scan web servers for known vulnerabilities and misconfigurations, including outdated software versions, weak passwords, and configuration errors.

⦁	nikto can perform a wide variety of tests on web servers, including HTTP methods testing, server and software banner grabbing, directory and file discovery, and injection and XSS testing.

⦁	The tool provides a comprehensive report of the web server's security status.

⦁	nikto is a powerful and easy-to-use tool for web server security testing and is widely used by security professionals and web developers alike. 

**3.Web Application Analysis** : 

Web Application Analysis refers to all applications that are accessed through a browser. Security testing for your application is very important if data leaks or modifications are unacceptable and intolerable.

**A.CMS (Content Management System) and Framework identification**:

This tool is designed to help security professionals and ethical hackers identify the CMS and Frameworks used by a website or web application, which can be helpful in identifying potential vulnerabilities and attack vectors.The CMS and Framework identification tool in Kali Linux works by scanning a website or web application and analyzing its source code and HTTP response headers to determine the CMS and Frameworks used.

*i.wpscan* :

⦁	WPScan is a popular security tool in Kali Linux that is designed to scan WordPress websites for vulnerabilities and security issues.

⦁	The tool uses various techniques to identify potential vulnerabilities, including scanning for vulnerable plugins and themes, checking for weak passwords, and identifying common misconfigurations.

⦁	WPScan can be used to enumerate WordPress usernames, version numbers, installed plugins and themes, and other important information that can be useful for security testing and vulnerability assessment.

⦁	The tool can also be used to perform brute force attacks on WordPress login pages in order to identify weak passwords and gain unauthorized access to a website.

⦁	WPScan is a powerful and versatile tool that can be used by security professionals and ethical hackers to identify and exploit vulnerabilities in WordPress websites, and it is a valuable addition to any security testing toolkit. 

**B.Web Application Proxies** :

The main objective of a web application hacker is to gain deep insight into the inner workings of the application, and this is best accomplished by acting as a man in the middle and intercepting every request and response.

*i.burpsuite*:

⦁	Burp Suite is a popular web application testing tool that is included in the Kali Linux distribution. 

⦁ It provides a wide range of features that allow security testers and developers to identify vulnerabilities and security issues in web applications.

⦁	Burp Suite is designed to be highly customizable and flexible, allowing users to configure it to meet their specific testing needs.

⦁ It includes a proxy server, scanner, intruder, repeater, sequencer, and many other modules that can be used for a variety of testing tasks.

⦁	One of the key features of Burp Suite is its ability to intercept and modify HTTP and HTTPS traffic between the browser and web application. 

⦁ This allows security testers to analyze and manipulate the application's behavior.

**C.Web crawlers and Directory Brute Force** :

Web crawling is the process of getting specific information from websites using a bot or automated script. Kali provides the inbuilt applications to perform this activity. The benefit of web crawling is that it lets you import data without having to perform attacks manually, one by one.

*i.CuteCapt*:

⦁	 Is a command-line utility tool in Kali Linux that can be used to capture screenshots of web pages.

⦁	CuteCapt allows you to capture screenshots of web pages, either the entire page or just a selected region. This can be useful for capturing evidence or documenting the appearance of a website.

⦁	CuteCapt is a command-line tool, but it's simple and easy to use. You can specify the URL of the webpage you want to capture, the output file format, and the size of the screenshot.

⦁	Customizable Screenshot Size.

⦁	Supports Multiple Image Formats.

⦁	CuteCapt is open-source software and is available for free on the Kali Linux repository. This means that you can modify and distribute the software as you see fit, and you can also contribute to its development.

**4.Database assessment** :

A database security assessment examines the IT environment and identifies security vulnerabilities in databases, and examines the security controls implemented. The following are some of the advantages of conducting a database security assessment.It determines how successful security policies and procedures are.It enables a proactive security approach.It evaluates and verifies the security measures and mechanisms already implemented.It identifies security flaws and vulnerabilities in configurations and IT environments that can lead to data breaches, malicious infiltration, etc.It helps organizations to meet legal, regulatory, and compliance requirements such as It identifies security flaws and vulnerabilities in configurations and IT infrastructures, resulting in data breaches, hostile infiltration, and other problems.

i.SQLite database browser:
⦁	SQLite is a lightweight, file-based database system that is commonly used in small-scale applications. It is included in Kali Linux as a default package.
⦁	The SQLite database browser tool in Kali Linux is a graphical user interface (GUI) that allows you to view and edit SQLite databases. It provides a visual representation of the database structure and allows you to execute SQL queries.
⦁	The SQLite database browser tool in Kali Linux supports a variety of features, including the ability to create new tables, modify existing tables, and import/export data.
⦁	The tool is easy to use and provides a simple interface for managing SQLite databases. It can be accessed from the Kali Linux menu or by typing "sqlitebrowser" in the terminal.
⦁	The SQLite database browser tool in Kali Linux is an essential tool for developers and system administrators who need to manage SQLite databases. It is frequently used in testing and development environments to create and modify databases and to validate SQL statements.
ii.SQLMap :
⦁	Is an open-source penetration testing tool that automates the process of detecting and exploiting SQL injection vulnerabilities in web applications. It is included in Kali Linux as a default package.
⦁	SQLMap works by sending specially crafted SQL queries to a web application's database to determine if it is vulnerable to SQL injection attacks. It can also be used to extract data from vulnerable databases and perform other types of attacks.
⦁	SQLMap supports a wide range of database management systems, including MySQL, Oracle, PostgreSQL, and Microsoft SQL Server. It can also be used to test web application security on different platforms, such as Windows, Linux, and Mac OS.
⦁	The SQLMap tool in Kali Linux is highly configurable and allows you to customize the attack parameters to suit your needs. It supports a variety of attack techniques, including blind SQL injection, time-based SQL injection, and error-based SQL injection.
⦁	SQLMap is a popular tool for penetration testers and security professionals who need to assess the security of web applications that use SQL databases. It is easy to use and provides detailed reports on the vulnerabilities detected, making it an essential tool for anyone who wants to secure their web applications against SQL injection attacks.

5.Password Attacks :It takes nmap GNMAP/XML output and automatically brute-force services with default credentials using Medusa. It is a platform to perform security testing of web applications. It is a custom wordlist generator that spread a given url to a specified depth, optionally following external links.
A.Offline Attacks :
⦁	Offline password attacks involve attempting to crack password hashes that have been obtained through methods such as stealing a database of hashed passwords.
⦁	Kali Linux provides a variety of tools for offline password attacks, including John the Ripper, Hashcat, and Hydra.
⦁	These tools use various techniques such as brute-force attacks, dictionary attacks, and rule-based attacks to crack passwords.
⦁	It's important to note that offline password attacks can be time-consuming and resource-intensive, especially for complex passwords or hashed passwords that use strong encryption algorithms.
⦁	To protect against offline password attacks, it's important to use strong passwords that are difficult to crack and to use secure hashing algorithms that make it more difficult for attackers to crack password hashes. Additionally, multi-factor authentication can provide an additional layer of protection against password attacks.
i.Hashcat :
⦁	Is a popular password cracking tool that is included in the Kali Linux distribution.
⦁	The tool is designed to crack passwords by using brute-force attacks, dictionary attacks, rule-based attacks, and mask attacks.
⦁	Hashcat can crack password hashes for a wide variety of encryption algorithms, including MD5, SHA-1, SHA-2, and bcrypt.
⦁	The tool supports both CPU and GPU acceleration, making it a fast and efficient password cracking tool.
⦁	Hashcat can also be used to perform other tasks related to password cracking, such as generating wordlists and creating custom rule sets for use in rule-based attacks. However, it's important to note that the tool should only be used for legitimate security testing purposes, and not for illegal or malicious activities.
ii.Hashcat :
⦁	HashID is a tool included in Kali Linux that is used for identifying different types of hashes.
⦁	The tool can be used to identify hash types such as MD5, SHA-1, SHA-256, bcrypt, and many others.
⦁	HashID works by comparing the input hash to a database of known hash types and returning a list of potential matches.
⦁	The tool can be useful in identifying the type of hash used in a password database or other encrypted data, which can then be used to select an appropriate cracking tool.
⦁	HashID can also be used to generate example hashes for different hash types, which can be useful for testing and experimenting with different cracking tools.
iii.chntpw:
⦁	Is a tool included in Kali Linux that is used for resetting or removing Windows passwords.
⦁	The tool can be used to modify the SAM database, which stores Windows user account information, including password hashes.
⦁	chntpw can be used to reset or remove a Windows password by modifying the SAM database and replacing the password hash with a new one.
⦁	The tool can be run from a live Linux distribution or by booting into single-user mode on a Windows system.
⦁	chntpw is a powerful tool that should be used with caution, as modifying the SAM database incorrectly can cause system instability or even data loss. It is recommended to use the tool only for legitimate purposes, such as password recovery or system administration.
B.Online Attacks :
i.Hydra:
⦁	Is a popular online password attack tool that is available in Kali Linux, a powerful operating system used for penetration testing and ethical hacking. Here are five key points to know about Hydra:
⦁	Hydra is a command-line tool used for brute-force attacks on online passwords. It supports a wide range of protocols, including HTTP, FTP, SMTP, SSH, Telnet, and many others. Hydra can also be customized with various options to improve its performance and accuracy.
⦁	Hydra is an effective tool for testing the security of online accounts, but it should only be used for ethical and legal purposes. Using Hydra to attack accounts without permission is illegal and can result in serious legal consequences.
⦁	Hydra works by guessing passwords based on a list of possible options. It can be configured to use different password dictionaries and to try various combinations of characters, numbers, and symbols.
⦁	Hydra can be used to launch both dictionary attacks and brute-force attacks. A dictionary attack uses a pre-defined list of passwords, while a brute-force attack tries every possible combination of characters until it finds the correct password.
⦁	Hydra is just one of many online password attack tools available in Kali Linux. Other tools, such as Medusa, THC Hydra, and John the Ripper, can also be used for similar purposes. It's important to choose the right tool for the task at hand and to use it ethically and responsibly.
ii.Hydra-gtk :
⦁	Is a graphical user interface (GUI) version of the Hydra online password attack tool in Kali Linux. Here are five key points to know about Hydra-gtk:
⦁	Hydra-gtk is a user-friendly version of Hydra that provides a GUI interface for launching online password attacks. It is easier to use than the command-line version of Hydra, but it still requires a basic understanding of how password attacks work.
⦁	Like the command-line version of Hydra, Hydra-gtk is used for brute-force attacks on online passwords. It supports a wide range of protocols, including HTTP, FTP, SMTP, SSH, Telnet, and many others.
⦁	Hydra-gtk allows users to configure various options for the password attack, such as the username list, password list, and password length. Users can also set the number of parallel threads and customize the timeouts for each request.
⦁	Hydra-gtk displays the results of the password attack in real-time and allows users to save the results to a file for further analysis. It also provides a log file with detailed information about each request and response.
⦁	Like all online password attack tools, Hydra-gtk should only be used for ethical and legal purposes. Using Hydra-gtk to attack accounts without permission is illegal and can result in serious legal consequences. It's important to use the tool responsibly and to get permission from the owner of the system being tested.
iii.Patator:
⦁	 Patator is a versatile online password attack tool that supports many protocols, including HTTP, FTP, SSH, Telnet, and many others. It can also be used for brute-force attacks on other types of data, such as email addresses and file names.
⦁	Patator is highly customizable, allowing users to specify the target, username, password list, and other parameters for the attack. Users can also specify the number of threads, the delay between requests, and other performance settings.
⦁	Patator uses a modular architecture, with separate modules for each type of attack. This makes it easy to add new modules or customize existing ones to suit specific needs.
⦁	Patator supports both dictionary attacks and brute-force attacks. It can also perform hybrid attacks, which combine dictionary and brute-force methods to improve efficiency and accuracy.
⦁	Like other online password attack tools, Patator should only be used for ethical and legal purposes. It's important to obtain permission from the owner of the system being tested and to use the tool responsibly. Using Patator to attack accounts or systems without permission is illegal and can result in serious legal consequences.
C.passing the hash Tools:This package contains modified versions of Curl, Iceweasel, FreeTDS, Samba 4, WinEXE and WMI. They are installed as executables starting with the “pth-” string.
i.Mimikatz:
⦁	Is a powerful tool used for penetration testing and security research, specifically for extracting passwords and other credentials from Windows systems. Here are five key points to know about Mimikatz:
⦁	Mimikatz is a post-exploitation tool that can be used to extract credentials and perform other post-exploitation activities on Windows systems. It can bypass common defenses such as firewalls, antivirus software, and other security mechanisms.
⦁	Mimikatz can extract various types of credentials, including passwords, Kerberos tickets, and plaintext credentials stored in memory. It can also perform pass-the-hash attacks, which allow attackers to use stolen password hashes to authenticate to other systems.
⦁	Mimikatz has various built-in modules that can be used to perform different types of attacks, such as dumping passwords, keys, and certificates. It can also be used to perform various memory analysis and forensic activities.
⦁	Mimikatz is frequently updated to stay current with the latest security vulnerabilities and bypass techniques. It is widely used by security researchers and penetration testers to test the security of Windows systems and identify potential vulnerabilities.
⦁	It is important to use Mimikatz ethically and legally, with the explicit permission of the system owner. Using Mimikatz for unauthorized purposes is illegal and can result in serious legal consequences. Additionally, it is important to use best practices for securing Windows systems and preventing unauthorized access to credentials.
ii.pth-curl:
⦁	Is a command-line option in John the Ripper that enables it to perform password cracking attacks on HTTP-based authentication protocols such as NTLM and Kerberos.
⦁	pth-curl uses the curl utility to send authentication requests to the target server, and then uses John the Ripper to brute-force the password hashes returned by the server.
⦁	To use pth-curl in John the Ripper, users must first capture the NTLM or Kerberos hash from the target server. This can be done using a variety of network monitoring tools.
⦁	Once the hash is captured, the user can use pth-curl in John the Ripper to perform a brute-force attack on the hash, attempting to crack the password used by the target user.
⦁	Like all password cracking tools, it is important to use pth-curl ethically and legally, with the explicit permission of the system owner. Using pth-curl or other password cracking tools for unauthorized purposes is illegal and can result in serious legal consequences.
iii.pth-net tool :
⦁	pth-net is a command line option in John the Ripper that enables it to perform password cracking attacks on the Windows Authentication and Remote Desktop Protocol (RDP) protocols.
⦁	pth-net uses the NTLM protocol to authenticate to the target system and retrieve password hashes.
⦁	pth-net can be used with captured traffic files or with live traffic captured by a network sniffer.
⦁	Once the password hashes have been captured, pth-net can be used in John the Ripper to perform a brute-force attack on the hashes.
⦁	As with all password cracking tools, it is important to use pth-net ethically and legally, with the explicit permission of the system owner. Using pth-net or other password cracking tools for unauthorized purposes is illegal and can result in serious legal consequences.
⦁	D.cewl:
⦁	 Is a tool used for generating custom wordlists by spidering websites and extracting unique words and phrases from them.
⦁	cewl works by crawling a target website and extracting words and phrases that are likely to be used as passwords or other forms of authentication.
⦁	cewl can be used with various parameters to customize the spidering process, including specifying the depth of the spidering and the minimum and maximum word length.
⦁	Once cewl has generated a custom wordlist, it can be used in conjunction with other password cracking tools such as John the Ripper or Hashcat to attempt to crack passwords.
⦁	cewl is frequently used by penetration testers and security researchers to create custom wordlists that are more targeted and effective than traditional wordlists. However, it is important to use cewl ethically and with the explicit permission of the website owner, as unauthorized spidering and data harvesting can be illegal and unethical.
E.crunch :
⦁	Is a tool used for generating custom wordlists based on specified criteria, such as length, character set, and pattern.
⦁	crunch allows the user to generate wordlists with specific character sets, including uppercase and lowercase letters, numbers, and symbols.
⦁	The user can also specify the minimum and maximum length of the words to be generated, as well as patterns or masks for specific parts of the word.
⦁	crunch can be used with various parameters to customize the wordlist generation process, including specifying the output file format and the number of lines to generate.
⦁	Once a custom wordlist has been generated with crunch, it can be used in conjunction with other password cracking tools such as John the Ripper or Hashcat to attempt to crack passwords.
⦁	Crunch is a popular tool among penetration testers and security researchers for creating custom wordlists that are more targeted and effective than traditional wordlists. However, it is important to use crunch ethically and with the explicit permission of the system owner, as unauthorized use can be illegal and unethical.
F.Wordlist:
⦁	Is a collection of words or phrases used for password cracking and other security-related tasks.
⦁	Wordlists can be pre-made or custom-generated using tools such as cewl, crunch, and other tools.
⦁	Wordlists can be organized by topic or category, such as "sports teams," "movies," or "common phrases."
⦁	Wordlists can be used with various password cracking tools such as John the Ripper, Hashcat, Hydra, and others.
⦁	Wordlists are a critical component of password cracking and can greatly impact the success of password cracking attempts. It is important to use wordlists ethically and with the explicit permission of the system owner, as unauthorized use can be illegal and unethical. It is also important to keep wordlists updated and to use multiple wordlists and tools for best results.
G.cewl
H.crunch
I.hashcat
J.john:
⦁	John the Ripper is a popular password cracking tool that can crack many different types of passwords, including hashes generated by various operating systems and applications.
⦁	John the Ripper can use a variety of different attacks to crack passwords, including brute-force, dictionary, and hybrid attacks.
⦁	John the Ripper supports a wide range of hash types, including traditional Unix passwords, Windows LM and NTLM hashes, and many others.
⦁	John the Ripper can use custom wordlists generated with tools such as cewl, crunch, and others to improve the success rate of password cracking attempts.
⦁	John the Ripper is a command-line tool that can be used in various modes, including single-crack mode, wordlist mode, incremental mode, and others. It is a powerful tool that requires some knowledge and skill to use effectively. It is important to use John the Ripper ethically and with the explicit permission of the system owner, as unauthorized use can be illegal and unethical.
K.medusa
L.ncrack:
⦁	ncrack is a high-speed network authentication cracking tool that can be used to test the security of remote systems.
⦁	ncrack supports various authentication protocols, including SSH, FTP, Telnet, HTTP(S), SMB, RDP, and others.
⦁	ncrack uses a parallelized and asynchronous architecture to maximize efficiency and speed in password cracking.
⦁	ncrack can use custom wordlists and brute-force attacks to crack passwords, as well as other techniques such as username enumeration and service detection.
⦁	ncrack is a command-line tool that can be used with various parameters to customize the authentication cracking process. It is a powerful tool that requires some knowledge and skill to use effectively. It is important to use ncrack ethically and with the explicit permission of the system owner, as unauthorized use can be illegal and unethical.
M.ophcrack :
⦁	Is a free and open-source password cracking tool that is designed to crack Windows passwords.
⦁	ophcrack uses a rainbow table-based method to crack passwords, which involves precomputing the hashes of all possible combinations of characters and storing them in a table for quick lookup.
⦁	ophcrack can be used with live CDs or USBs, which contain a special operating system that can be booted from a computer to run ophcrack and crack Windows passwords.
⦁	ophcrack can be used to crack Windows NT/2000/XP/7/8/10 passwords, including those using NTLM and LM hash algorithms.
⦁	ophcrack is a relatively easy-to-use tool and can be useful for users who are not familiar with command-line password cracking tools. However, it is important to use ophcrack ethically and with the explicit permission of the system owner, as unauthorized use can be illegal and unethical.
N.wordlists
6.Wireless attacks:This tool is used to attack clients as opposed to the Access Point itself. It has the ability to act as an ad-hoc Access Point. It is an 802.11 WEP and WPA-PSK keys cracking tool, which is used to recover the keys once enough data packets have been captured.
A.802.11 Wireless Tools :The 802.11 Wireless Tools, also known as the Wireless Extension (WE) or Wireless Tools for Linux (WTL), are a set of utilities and drivers used for configuring and monitoring wireless networks on Linux systems.The 802.11 Wireless Tools can be used to monitor wireless networks, view network statistics, and perform various network-related tasks such as scanning for available networks, connecting to networks, and testing network performance.The tools can be used with various wireless interfaces, including PCI, USB, and PCMCIA wireless cards.Some of the most popular tools in the 802.11 Wireless Tools include iwconfig, iwlist, iwpriv, and iwspy, which can be used to manage wireless network settings, scan for available networks, view network statistics, and monitor network activity.The 802.11 Wireless Tools are widely used in the field of wireless networking and can be a useful tool for wireless network administrators, security professionals, and other users who need to configure or monitor wireless networks on Linux systems.
i.bully:
⦁	Is a command-line tool in Kali Linux that is used for performing brute-force attacks against WPS (Wi-Fi Protected Setup) enabled wireless access points.
⦁	WPS is a feature that allows users to easily connect to a wireless network without needing to enter a password, making it vulnerable to brute-force attacks.
⦁	bully uses a brute-force attack to guess the WPS PIN (Personal Identification Number) of a wireless access point, allowing an attacker to gain unauthorized access to the network.
⦁	bully uses a variety of techniques to perform the brute-force attack, including offline and online attacks, pixie dust attacks, and more.
⦁	While bully can be a powerful tool for testing the security of WPS-enabled wireless networks, it should only be used ethically and with the explicit permission of the network owner. Unauthorized use of bully or other brute-force tools can be illegal and unethical.
ii.Fern Wifi Cracker (root):
⦁	The Fern Wifi Cracker is a GUI (Graphical User Interface) based wireless security auditing tool that can be used to crack WEP, WPA, and WPA2 wireless networks.
⦁	The tool is designed to be used by security professionals, penetration testers, and other users who need to test the security of wireless networks.
⦁	Fern Wifi Cracker uses various techniques such as packet sniffing, brute-force attacks, and dictionary attacks to crack wireless network passwords.
⦁	The tool also includes features such as automatic WEP cracking, automatic WPA cracking, and automatic wireless interface detection, making it easier to use for non-experts.
⦁	While Fern Wifi Cracker can be a useful tool for testing the security of wireless networks, it should only be used ethically and with the explicit permission of the network owner. Unauthorized use of Fern Wifi Cracker or other wireless security tools can be illegal and unethical.
B.Bluetooth tools : Kali Linux comes with several Bluetooth tools built-in, which can be used for a variety of tasks, including discovering nearby Bluetooth devices, connecting to them, and even exploiting vulnerabilities in Bluetooth protocols.One of the most popular Bluetooth tools in Kali Linux is Bluelog, which is a Bluetooth scanner that can be used to detect and log nearby Bluetooth devices. It can also detect the manufacturer, device type, and signal strength of each device.Another popular Bluetooth tool in Kali Linux is BlueMaho, which is a Bluetooth reconnaissance tool that can be used to discover nearby Bluetooth devices and gather information about them. It can also be used to exploit vulnerabilities in Bluetooth protocols and perform man-in-the-middle attacks.Kali Linux also includes tools like BlueRanger, which can be used to test the security of Bluetooth-enabled devices by exploiting vulnerabilities in their firmware, and Spooftooph, which can be used to spoof the MAC address of a Bluetooth device to gain unauthorized access.Bluetooth tools in Kali Linux can be used by security professionals, penetration testers, and other users who need to test the security of Bluetooth-enabled devices or networks. However, it's important to use them ethically and with the explicit permission of the device or network owner, as unauthorized use of Bluetooth tools can be illegal and unethical.
i.Spooftooph :
⦁	Is a command-line tool in Kali Linux that is used for Bluetooth device spoofing. It can be used to change the MAC address of a Bluetooth device, allowing an attacker to impersonate a legitimate device and gain unauthorized access to Bluetooth-enabled networks or devices.
⦁	The tool can be used to spoof the MAC address of various Bluetooth devices, including headsets, phones, laptops, and more.
⦁	Spooftooph uses the L2CAP (Logical Link Control and Adaptation Protocol) layer of the Bluetooth protocol to perform the spoofing. It can send spoofed L2CAP packets to a target device, impersonating a legitimate Bluetooth device.
⦁	Spooftooph can be used for various purposes, including testing the security of Bluetooth-enabled devices and networks, bypassing Bluetooth authentication mechanisms, and gaining unauthorized access to Bluetooth devices.
⦁	It's important to use Spooftooph and other Bluetooth spoofing tools ethically and with the explicit permission of the device or network owner, as unauthorized use can be illegal and unethical.
C.aircrack-ng:
⦁	Aircrack-ng is a set of command-line tools in Kali Linux that is used for cracking wireless networks. It can be used to capture and analyze network traffic, crack WEP and WPA/WPA2-PSK encryption, and perform other wireless network attacks.
⦁	The tool is capable of sniffing wireless traffic, injecting packets, and performing dictionary attacks on captured traffic to crack passwords. It can also perform deauthentication attacks to force a client to reconnect to a network, allowing the attacker to capture the handshake and crack the password.
⦁	Aircrack-ng supports a wide range of wireless network interfaces, including USB, PCMCIA, and PCI adapters. It can also work with virtual interfaces created by tools like VirtualBox or VMWare.
⦁	Aircrack-ng is highly customizable, allowing users to tweak various parameters such as the number of threads to use, the size of the dictionary file to use, and the maximum number of attempts per second.
⦁	The tool can be used for ethical hacking purposes, such as testing the security of wireless networks and assessing their vulnerabilities. However, it's important to use Aircrack-ng ethically and with the explicit permission of the network owner, as unauthorized use can be illegal and unethical.
D.Fern Wifi Cracker (root)
E.Kismet :
⦁	Is a wireless network detector, sniffer, and intrusion detection system that is available in Kali Linux. It's designed to detect and analyze wireless networks and their traffic, and it can be used for a variety of purposes, including network monitoring, troubleshooting, and security auditing.
⦁	The tool can detect various types of wireless networks, including 802.11a/b/g/n/ac, Bluetooth, Zigbee, and more. It can also detect hidden SSIDs and rogue access points.
⦁	Kismet captures network traffic and analyzes it in real-time, providing detailed information about the networks and devices connected to them. It can display information such as SSIDs, MAC addresses, signal strengths, data rates, and more.
⦁	Kismet is highly customizable, allowing users to configure various parameters such as the capture channel, filter settings, and output format. It also supports plugins, which can be used to extend its functionality.
⦁	Kismet can be used for various purposes, including monitoring wireless networks for security threats, analyzing network performance, and troubleshooting connectivity issues. However, it's important to use Kismet and other network monitoring tools ethically and with the explicit permission of the network owner, as unauthorized use can be illegal and unethical.
F.Pixiewps:
⦁	Is a tool that can be used to exploit vulnerabilities in the WPS (Wi-Fi Protected Setup) protocol to recover the WPA/WPA2 passphrase of a wireless network. It's available in Kali Linux and is used for testing the security of wireless networks.
⦁	The tool uses a brute force attack to try all possible combinations of the eight-digit PIN used by the WPS protocol to authenticate devices to a wireless network. It also uses a technique called "Pixie Dust" to exploit a vulnerability in the WPS protocol that allows for the recovery of the passphrase in a short amount of time.
⦁	Pixiewps requires a wireless network interface that supports monitor mode and packet injection. The tool works by capturing packets exchanged between the target wireless access point and client devices and analyzing them for the WPS PIN.
⦁	Pixiewps is a command-line tool that requires some knowledge of the WPS protocol and wireless network security to use effectively. It can be run with various parameters to customize the attack and improve its chances of success.
⦁	Pixiewps can be used for ethical hacking purposes, such as testing the security of wireless networks and assessing their vulnerabilities. However, it's important to use the tool ethically and with the explicit permission of the network owner, as unauthorized use can be illegal and unethical.
G.Reaver:
⦁	Is a tool that can be used to exploit vulnerabilities in the WPS (Wi-Fi Protected Setup) protocol to recover the WPA/WPA2 passphrase of a wireless network. It's available in Kali Linux and is used for testing the security of wireless networks.
⦁	Reaver uses a brute force attack to try all possible combinations of the eight-digit PIN used by the WPS protocol to authenticate devices to a wireless network. It sends a series of requests to the access point, which provides an indication of whether the PIN is correct or not.
⦁	Reaver requires a wireless network interface that supports monitor mode and packet injection. The tool works by capturing packets exchanged between the target wireless access point and client devices and analyzing them for the WPS PIN.
⦁	Reaver is a command-line tool that requires some knowledge of the WPS protocol and wireless network security to use effectively. It can be run with various parameters to customize the attack and improve its chances of success.
⦁	Reaver can be used for ethical hacking purposes, such as testing the security of wireless networks and assessing their vulnerabilities. However, it's important to use the tool ethically and with the explicit permission of the network owner, as unauthorized use can be illegal and unethical. Additionally, Reaver has been known to cause some wireless access points to crash or lock up during an attack, so it's important to use it with caution and not on critical networks.
H.Wifite:
⦁	 Is a tool that can be used to automate wireless network attacks. It's designed to simplify the process of cracking WEP and WPA/WPA2 wireless networks and is available in Kali Linux.
⦁	Wifite uses a combination of tools such as Aircrack-ng, Pyrit, and Reaver to perform wireless attacks. It automates the process of capturing packets, deauthenticating clients, and cracking passwords.
⦁	Wifite supports a range of wireless network interfaces and can run on a variety of platforms, including Linux, macOS, and Windows. The tool is easy to use and doesn't require any advanced technical knowledge.
⦁	Wifite has a range of features, including automatic detection of wireless networks, automatic selection of attack methods, and support for custom attacks. It also has a variety of options for customizing attacks, such as setting a maximum number of deauthentication attempts.
⦁	Wifite can be used for ethical hacking purposes, such as testing the security of wireless networks and assessing their vulnerabilities. However, it's important to use the tool ethically and with the explicit permission of the network owner, as unauthorized use can be illegal and unethical. Additionally, Wifite is not foolproof and may not work on all networks, so it's important to use it as part of a larger toolkit for wireless network penetration testing.
7.Reverse Engineering :Reverse engineering refers to the process of analyzing and understanding how a piece of software or hardware works by breaking it down into its components and examining its inner workings. In the context of Kali Linux, reverse engineering can be a useful tool for security researchers, hackers, and developers who want to understand how a particular software or hardware system functions.
Kali Linux is a popular operating system used by security professionals and ethical hackers. It comes preloaded with a range of tools and applications that can be used for penetration testing, vulnerability assessment, and digital forensics. One of the tools available in Kali Linux for reverse engineering is Radare2, a powerful disassembler and debugger that can be used to analyze binary files.
To start reverse engineering a binary file in Kali Linux using Radare2, the first step is to open the file using the command "r2 filename". This will load the binary file into Radare2, and the user can then use various commands to analyze the file. For example, the command "aa" can be used to automatically analyze the binary and create a function database.
Once the binary file has been loaded into Radare2, the user can then start exploring its code by using commands such as "pd" (print disassembly) and "s" (seek to a specific address). The user can also set breakpoints and step through the code using the debugger.
Another tool available in Kali Linux for reverse engineering is Ghidra, a powerful reverse engineering framework developed by the National Security Agency (NSA). Ghidra can be used to analyze both binary and source code, and it comes with a range of features such as disassembly, decompilation, and debugging.
To use Ghidra in Kali Linux, the user first needs to download and install it from the official website. Once installed, Ghidra can be launched from the command line using the command "./ghidraRun". The user can then import the binary or source code they want to analyze and start exploring its code using Ghidra's range of tools and features.
In conclusion, Kali Linux provides a range of powerful tools and applications that can be used for reverse engineering. Radare2 and Ghidra are just two examples of the many tools available in Kali Linux for reverse engineering, and they can be used to analyze binary and source code to gain a better understanding of how a particular software or hardware system works.
i.Clang :
⦁	Is a powerful compiler front-end tool that is included in Kali Linux and is commonly used in reverse engineering tasks. It is designed to parse, analyze, and compile source code written in various programming languages, including C, C++, and Objective-C.
⦁	One of the main features of Clang is its ability to produce highly optimized and efficient code, making it a popular choice for reverse engineers who need to disassemble and analyze compiled binary code.
⦁	Clang can be used in conjunction with other reverse engineering tools, such as LLVM, to perform advanced code analysis and optimization. LLVM is a set of modular and reusable compiler and toolchain technologies that can be used to build various tools and applications for code analysis and transformation.
⦁	Clang's ability to produce highly optimized and efficient code makes it a valuable tool for reverse engineers who need to analyze complex and obfuscated binaries. By using Clang to analyze the code, reverse engineers can gain a deeper understanding of how the code works and identify potential vulnerabilities or security flaws.
⦁	Clang is also highly customizable, and users can modify its behavior by adding their own custom plugins and extensions. This flexibility makes Clang a powerful tool for reverse engineering in Kali Linux, allowing users to tailor its functionality to their specific needs and requirements.
ii.Clang++ :
⦁	Is a C++ compiler that is included in Kali Linux and is commonly used in reverse engineering tasks. It is a part of the Clang compiler family and provides support for C++14, C++17, and other modern C++ standards.
⦁	One of the main advantages of using Clang++ in reverse engineering tasks is its ability to produce highly optimized and efficient code. This is particularly important when dealing with large and complex codebases that need to be analyzed and disassembled.
⦁	Clang++ also provides a range of powerful debugging and profiling features that can be used to identify bugs and performance issues in the code. These features include support for sanitizers, profiling tools, and debuggers, making Clang++ a valuable tool for reverse engineers who need to understand the inner workings of complex software systems.
⦁	Another advantage of Clang++ is its compatibility with other tools and frameworks commonly used in reverse engineering, such as LLVM and Radare2. By using Clang++ in combination with these tools, reverse engineers can perform advanced code analysis and optimization, and gain a deeper understanding of how the code works.
⦁	Clang++ is highly customizable and can be configured to suit the specific needs and requirements of individual users. This flexibility makes it a powerful tool for reverse engineering in Kali Linux, allowing users to tailor its functionality to their specific tasks and goals.
iii.NASM (Netwide Assembler) :
⦁	Is a popular assembler used in Kali Linux for reverse engineering tasks. It is a lightweight and efficient tool that can be used to assemble and disassemble binary code written in various assembly languages, including x86, x64, and ARM.
⦁	NASM is particularly useful for reverse engineers who need to analyze and disassemble machine code generated by compilers such as GCC and Clang. By using NASM to disassemble the code, reverse engineers can gain a deeper understanding of how the code works and identify potential security vulnerabilities or flaws.
⦁	NASM provides a range of powerful features that can be used to analyze and modify the assembly code. These features include macros, conditional assembly, and various directives that can be used to customize the output.
⦁	NASM is also highly portable and can be run on various platforms, including Windows, Linux, and macOS. This makes it a valuable tool for reverse engineers who need to work on multiple platforms and need a tool that is compatible with all of them.
⦁	Finally, NASM is an open-source tool, and its source code is available for modification and customization. This flexibility makes it a powerful tool for reverse engineering in Kali Linux, allowing users to tailor its functionality to their specific needs and requirements.
8.Exploitation Tools :It is an OS command Injection and Exploitation Tool used to test web applications for bugs, errors, and vulnerabilities related to command injection attacks. It is a tool to crack and decrypt BLE encryption that allows an attacker to guess or brute force the Temporary Key.
A.CrackMapExec:
⦁	CrackMapExec (CME) is a powerful open-source tool designed for penetration testing, active directory reconnaissance, and credential harvesting. Here are five key points on using CME for reverse engineering in Kali Linux:
⦁	Active Directory reconnaissance: CME can be used to gather information about an Active Directory (AD) environment, including domain controllers, user accounts, groups, and computers. This information can be used for further attacks or to identify potential vulnerabilities.
⦁	Credential harvesting: CME can also be used to extract credentials from compromised systems or through password spraying attacks. These credentials can be used for lateral movement within the AD environment or to gain access to other systems.
⦁	Brute force attacks: CME can perform brute force attacks against SMB, SSH, and other services to crack passwords and gain access to systems. It supports a variety of protocols, including SMB, RDP, SSH, and WinRM.
⦁	Exploitation: CME can exploit known vulnerabilities in systems, such as the MS17-010 SMB vulnerability, to gain access to compromised systems. It can also run custom scripts and commands on compromised systems.
⦁	Reporting: CME generates comprehensive reports on the results of its scans and attacks, making it easier to identify vulnerabilities and plan future attacks. Reports can be saved in multiple formats, including HTML, JSON, and CSV.
B.metasploit framework :
⦁	The Metasploit Framework is an open source penetration testing and development platform 
⦁	It provides exploits for a variety of applications, operating systems and platforms.
⦁	 Metasploit is one of the most commonly used penetration testing tools and comes built-in to Kali Linux.
C.searchsploit :
⦁	SearchSploit is a command-line search tool for Exploit-DB that allows you to take a copy of the Exploit Database with you.
⦁	SearchSploit gives you the power to perform detailed off-line searches through your locally checked-out copy of the repository. 
⦁	This capability is particularly useful for security assessments on segregated or air-gapped networks without Internet access.
9.Sniffing & Spoofing:The network can be a valuable source of information and offers a variety of potential attack vectors for a penetration tester. Sniffing network traffic can offer access to valuable intelligence, and spoofing traffic can enable a penetration tester to identify and exploit potential attack vectors.
A.minicom:
⦁	Minicom is a clone of the MS-DOS “Telix” communication program. 
⦁	powerful tool for troubleshooting issues with serial devices.
⦁	Used to connectr modems,routers and serial devices in kali Linux.
⦁	Allow users to communicate real time.
⦁	Light weight and efficient tool.
B.mitmproxy:
⦁	MITMproxy is a powerful command-line tool that allows users to intercept, manipulate, and analyze HTTP(S) traffic on Kali Linux.
⦁	It is a popular tool for performing man-in-the-middle attacks and can be used to intercept traffic between clients and servers, allowing users to observe and manipulate the data being transmitted.
⦁	MITMproxy has a powerful scripting engine that allows users to automate tasks, such as modifying requests and responses, creating custom filters, and logging data to a file.
⦁	It provides an easy-to-use web interface that displays detailed information about the intercepted traffic, including the headers, body, and cookies.
⦁	Additionally, MITMproxy has plugins that extend its functionality, such as the ability to analyze SSL/TLS certificates, modify request headers, and decrypt HTTPS traffic, making it a versatile and powerful tool for network analysis and penetration testing on Kali Linux.
C.Responder:
⦁	Responder is an inbuilt Kali Linux tool for Link-Local Multicast Name Resolution (LLMNR) and NetBIOS Name Service (NBT-NS) that responds to specific NetBIOS queries based on the file server request.
10.Post Exploitation :Post-exploitation refers to any actions taken after a session is opened. A session is an open shell from a successful exploit or bruteforce attack. A shell can be a standard shell or Meterpreter.
A.weevely:Weevely is a stealth PHP web shell that simulate telnet-like connection. It is an essential tool for web application post exploitation.
B.powershell empire :
⦁	This package contains a post-exploitation framework that includes a pure-PowerShell2.0 Windows agent, and a pure Python Linux/OS X agent. 
⦁	It is the merge of the previous PowerShell Empire and Python EmPyre projects. The framework offers cryptologically-secure communications and a flexible architecture. 
⦁	On the PowerShell side, Empire implements the ability to run PowerShell agents without needing powershell.exe, rapidly deployable post-exploitation modules ranging from key loggers to Mimikatz, and adaptable communications to evade network detection, all wrapped up in a usability-focused framework.
C.Proxychains :
⦁	Is a UNIX program, that hooks network-related libc functions in dynamically linked programs via a preloaded DLL (dlsym(), LD_PRELOAD) and redirects the connections through SOCKS4a/5 or HTTP proxies. 
⦁	It supports TCP only (no UDP/ICMP etc).
11.Forensics:Forensic tools are valuable not only for acquiring disk images but also for automating much of the analysis process, such as: Identifying and recovering file fragments and hidden and deleted files and directories from any location.
A. Autopsy(root) : 
⦁	The Autopsy is a cyber forensic tool used for the analysis of Windows and UNIX file systems.
⦁	It can also be used to recover deleted files and also show various sectors of uploaded images making it easier to make an in-depth analysis of the image.
B.Binwalk:
⦁	Binwalk is a great tool when we have a binary image and have to extract embedded files and executable codes out of them.
⦁	 It is even used to identify the files and codes which are embedded inside the firmware images. 
⦁	Binwalk is compatible with magic signatures for UNIX file utility as it uses libmagic library.
C.Bulk-Extractor tool:
⦁	which is to be used when you have to extract features like E-Mail address, URLs, Confidential Document Numbers from files. 
⦁	This tool is used for Intrusion investigations, malware investigations, identity investigations, or any other kind of cyber investigation. 
⦁	The awesome feature of working with compressed or corrupt files makes it a great tool to work with those files. IT works on disk images, files, or a directory of files and finds out the useful information.
12.Reporting tool:Reporting is one of the very important means in Ethical hacking or pen-testing, you must have heard the term called POC which is proof of concept. when a hacker or pen tester checks a system for loopholes or vulnerabilities then they need to provide an end report to the organization which consists of all the processes of discovering a vulnerability and also fixing it. These reports include all the information about the testing process, Vulnerabilities discovered in the network or system, and with that countermeasures to make it secure/unreachable. reporting is the last step of the ethical hacking process. Linux offers multiple Reporting Tools which helps pen tester to make these reports and process all the steps for making a good pen test report. Tools like Dradis, Pipal, and Metagoofil. 
A.Pipal:
⦁	This tool is an Open Source Built Ruby for Password analysis. 
⦁	It can be used or come in handy when you are analyzing large password dumps that you used in the process of penetration testing activity.
⦁	 This tool also comes pre-installed with Kali Linux and is found under-reporting tools in the application menu.
B.Faraday start:
Is a GUI application that consists of a ZSH terminal and a sidebar with details about your workspaces and hosts.
C.CutyCapt:
 is a small cross-platform command-line utility to capture WebKit’s rendering of a web page into a variety of vector and bitmap formats, including SVG, PDF, PS, PNG, JPEG, TIFF, GIF, and BMP.
13.The Social-Engineer Toolkit (SET): is an open-source penetration testing framework designed for social engineering. SET has a number of custom attack vectors that allow you to make a believable attack in a fraction of time. These kind of tools use human behaviors to trick them to the attack vectors.
A.MSF Payload Creator (MSFPC) :
⦁	Is a wrapper that generates multiple types of payloads. MSFPC is simple to use, and it aims to use as few as one option to produce a payload. MSFC is used hand in hand with Metasploit.
⦁	MSFC help command can be launched using the following console as follows. To use MSFC, an attacker must only define the payload they want by either the platform or the file extension they want the payload to have.
⦁	MSFC can be used in the following scenarios:
• When you can’t remember your IP, use the interface name: eth0.
• When you don’t know what your external Ip is, MSFC will discover it: wan.
• If you want to generate one of each payload? Use a loop.
• If you want to mass create payloads. Try batch for everything, batch MSF for every Meterpreter option, batch staged for every staged payload, or batch cmd stageless for every stageless command prompt.
B.The Social-Engineer Toolkit (SET) (root):
is an open-source penetration testing framework designed for social engineering. SET has a number of custom attack vectors that allow you to make a believable attack in a fraction of time. These kind of tools use human behaviors to trick them to the attack vectors.


