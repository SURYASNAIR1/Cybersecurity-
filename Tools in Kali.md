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

**a.CMS (Content Management System) and Framework identification**:

This tool is designed to help security professionals and ethical hackers identify the CMS and Frameworks used by a website or web application, which can be helpful in identifying potential vulnerabilities and attack vectors.The CMS and Framework identification tool in Kali Linux works by scanning a website or web application and analyzing its source code and HTTP response headers to determine the CMS and Frameworks used.

*i.wpscan* :

⦁	WPScan is a popular security tool in Kali Linux that is designed to scan WordPress websites for vulnerabilities and security issues.

⦁	The tool uses various techniques to identify potential vulnerabilities, including scanning for vulnerable plugins and themes, checking for weak passwords, and identifying common misconfigurations.

⦁	WPScan can be used to enumerate WordPress usernames, version numbers, installed plugins and themes, and other important information that can be useful for security testing and vulnerability assessment.

⦁	The tool can also be used to perform brute force attacks on WordPress login pages in order to identify weak passwords and gain unauthorized access to a website.

⦁	WPScan is a powerful and versatile tool that can be used by security professionals and ethical hackers to identify and exploit vulnerabilities in WordPress websites, and it is a valuable addition to any security testing toolkit. 

**b.Web Application Proxies** :

The main objective of a web application hacker is to gain deep insight into the inner workings of the application, and this is best accomplished by acting as a man in the middle and intercepting every request and response.

*i.burpsuite*:

⦁	Burp Suite is a popular web application testing tool that is included in the Kali Linux distribution. 

⦁ It provides a wide range of features that allow security testers and developers to identify vulnerabilities and security issues in web applications.

⦁	Burp Suite is designed to be highly customizable and flexible, allowing users to configure it to meet their specific testing needs.

⦁ It includes a proxy server, scanner, intruder, repeater, sequencer, and many other modules that can be used for a variety of testing tasks.

⦁	One of the key features of Burp Suite is its ability to intercept and modify HTTP and HTTPS traffic between the browser and web application. 

⦁ This allows security testers to analyze and manipulate the application's behavior.

**c.Web crawlers and Directory Brute Force** :

Web crawling is the process of getting specific information from websites using a bot or automated script. Kali provides the inbuilt applications to perform this activity. The benefit of web crawling is that it lets you import data without having to perform attacks manually, one by one.

*i.CuteCapt*:

⦁	 Is a command-line utility tool in Kali Linux that can be used to capture screenshots of web pages.

⦁	CuteCapt allows you to capture screenshots of web pages, either the entire page or just a selected region. This can be useful for capturing evidence or documenting the appearance of a website.

⦁	CuteCapt is a command-line tool, but it's simple and easy to use. You can specify the URL of the webpage you want to capture, the output file format, and the size of the screenshot.

⦁	Customizable Screenshot Size.

⦁	Supports Multiple Image Formats.

⦁	CuteCapt is open-source software and is available for free on the Kali Linux repository. This means that you can modify and distribute the software as you see fit, and you can also contribute to its development.

**4.Database assessment** :

A database security assessment examines the IT environment and identifies security vulnerabilities in databases, and examines the security controls implemented.It determines how successful security policies and procedures are.It enables a proactive security approach.It evaluates and verifies the security measures and mechanisms already implemented.It identifies security flaws and vulnerabilities in configurations and IT environments that can lead to data breaches, malicious infiltration, etc.It helps organizations to meet legal, regulatory, and compliance requirements such as It identifies security flaws and vulnerabilities in configurations and IT infrastructures, resulting in data breaches, hostile infiltration, and other problems.

*i.SQLite database browser*:

⦁	SQLite is a lightweight, file-based database system that is commonly used in small-scale applications. 

⦁	The SQLite database browser tool in Kali Linux is a graphical user interface (GUI) that allows you to view and edit SQLite databases.

⦁	It provides a visual representation of the database structure and allows you to execute SQL queries.

⦁	The SQLite database browser tool in Kali Linux supports a variety of features, including the ability to create new tables, modify existing tables, and import/export data.

⦁	The tool is easy to use and provides a simple interface for managing SQLite databases. It can be accessed from the Kali Linux menu or by typing "sqlitebrowser" in the terminal.

⦁	The SQLite database browser tool in Kali Linux is an essential tool for developers and system administrators who need to manage SQLite databases. 

**5.Password Attacks** :

**a..Offline Attacks** :

Offline password attacks involve attempting to crack password hashes that have been obtained through methods such as stealing a database of hashed passwords.Kali Linux provides a variety of tools for offline password attacks, including John the Ripper, Hashcat, and Hydra.These tools use various techniques such as brute-force attacks, dictionary attacks, and rule-based attacks to crack passwords.	Offline password attacks can be time-consuming and resource-intensive, especially for complex passwords or hashed passwords that use strong encryption algorithms.To protect against offline password attacks, it's important to use strong passwords that are difficult to crack and to use secure hashing algorithms that make it more difficult for attackers to crack password hashes.Multi-factor authentication can provide an additional layer of protection against password attacks.

*i.Hashcat* :

⦁	Is a popular password cracking tool that is included in the Kali Linux distribution.

⦁	The tool is designed to crack passwords by using brute-force attacks, dictionary attacks, rule-based attacks, and mask attacks.

⦁	Hashcat can crack password hashes for a wide variety of encryption algorithms, including MD5, SHA-1, SHA-2, and bcrypt.

⦁	The tool supports both CPU and GPU acceleration, making it a fast and efficient password cracking tool.

⦁	Hashcat can also be used to perform other tasks related to password cracking.

**b.Online Attacks**:

*i.Hydra*:

⦁	Is a popular online password attack tool that is available in Kali Linux, a powerful operating system used for penetration testing and ethical hacking.

⦁	Hydra is a command-line tool used for brute-force attacks on online passwords. 

⦁	It supports a wide range of protocols, including HTTP, FTP, SMTP, SSH, Telnet, and many others.

⦁	Hydra can also be customized with various options to improve its performance and accuracy.

⦁	Hydra is an effective tool for testing the security of online accounts.

⦁	Hydra works by guessing passwords based on a list of possible options.

**c.passing the hash Tools**:

*i.Mimikatz*:

⦁	Is a powerful tool used for penetration testing and security research, specifically for extracting passwords and other credentials from Windows systems.

⦁	Mimikatz is a post-exploitation tool that can be used to extract credentials and perform other post-exploitation activities on Windows systems. 

⦁	It can bypass common defenses such as firewalls, antivirus software, and other security mechanisms.

⦁	Mimikatz can extract various types of credentials, including passwords, Kerberos tickets, and plaintext credentials stored in memory. 

⦁	It can also perform pass-the-hash attacks, which allow attackers to use stolen password hashes to authenticate to other systems.

⦁	Mimikatz is frequently updated to stay current with the latest security vulnerabilities and bypass techniques.

**6.Wireless attacks**:

This tool is used to attack clients as opposed to the Access Point itself. It has the ability to act as an ad-hoc Access Point. It is an 802.11 WEP and WPA-PSK keys cracking tool, which is used to recover the keys once enough data packets have been captured.

**a..802.11 Wireless Tools** : The 802.11 Wireless Tools, also known as the Wireless Extension  are a set of utilities and drivers used for configuring and monitoring wireless networks on Linux systems.The 802.11 Wireless Tools can be used to monitor wireless networks, view network statistics, and perform various network-related tasks such as scanning for available networks, connecting to networks, and testing network performance.The tools can be used with various wireless interfaces, which can be used to manage wireless network settings, scan for available networks, view network statistics, and monitor network activity.The 802.11 Wireless Tools are widely used in the field of wireless networking and can be a useful tool for wireless network administrators, security professionals, and other users who need to configure or monitor wireless networks on Linux systems.

*i.bully*:

⦁	Is a command-line tool in Kali Linux that is used for performing brute-force attacks against Wi-Fi Protected Setup enabled wireless access points.

⦁	WPS is a feature that allows users to easily connect to a wireless network without needing to enter a password, making it vulnerable to brute-force attacks.

⦁	Bully uses a brute-force attack to guess the WPS PIN (Personal Identification Number) of a wireless access point, allowing an attacker to gain unauthorized access to the network.

⦁	Bully uses a variety of techniques to perform the brute-force attack, including offline and online attacks, pixie dust attacks, and more.

⦁	Bully can be a powerful tool for testing the security of WPS-enabled wireless networks.

**b.Bluetooth tools** : Kali Linux comes with several Bluetooth tools built-in, which can be used for a variety of tasks, including discovering nearby Bluetooth devices, connecting to them, and even exploiting vulnerabilities in Bluetooth protocols.It can also be used to exploit vulnerabilities in Bluetooth protocols and perform man-in-the-middle attacks.Bluetooth tools in Kali Linux can be used by security professionals, penetration testers, and other users who need to test the security of Bluetooth-enabled devices or networks.

*i.Spooftooph* :

⦁	It can be used to change the MAC address of a Bluetooth device, allowing an attacker to impersonate a legitimate device and gain unauthorized access to Bluetooth-enabled networks or devices.

⦁	The tool can be used to spoof the MAC address of various Bluetooth devices, including headsets, phones, laptops, and more.

⦁	Spooftooph uses the Logical Link Control and Adaptation Protocol layer of the Bluetooth protocol to perform the spoofing. 

⦁	It can send spoofed L2CAP packets to a target device, impersonating a legitimate Bluetooth device.

⦁	Spooftooph can be used for various purposes, including testing the security of Bluetooth-enabled devices and networks, bypassing Bluetooth authentication mechanisms, and gaining unauthorized access to Bluetooth devices.

**c.aircrack-ng**:

⦁	Aircrack-ng can be used to capture and analyze network traffic, crack WEP and WPA/WPA2-PSK encryption, and perform other wireless network attacks.

⦁	The tool is capable of sniffing wireless traffic, injecting packets, and performing dictionary attacks on captured traffic to crack passwords.

⦁	It can also perform deauthentication attacks to force a client to reconnect to a network, allowing the attacker to capture the handshake and crack the password.

⦁	Aircrack-ng supports a wide range of wireless network interfaces, including USB, PCMCIA, and PCI adapters.

⦁	It can also work with virtual interfaces created by tools like VirtualBox or VMWare.

⦁	Aircrack-ng is highly customizable.

⦁	The tool can be used for ethical hacking purposes.

**7.Reverse Engineering** :

Reverse engineering can be a useful tool for security researchers, hackers, and developers who want to understand how a particular software or hardware system functions.Kali Linux is a popular operating system used by security professionals and ethical hackers. It comes preloaded with a range of tools and applications that can be used for penetration testing, vulnerability assessment, and digital forensics. One of the tools available in Kali Linux for reverse engineering is Radare2, a powerful disassembler and debugger that can be used to analyze binary files.

*i.Clang* :

⦁	Is a powerful compiler front-end tool that is included in Kali Linux and is commonly used in reverse engineering tasks.

⦁	It is designed to parse, analyze, and compile source code written in various programming languages, including C, C++, and Objective-C.

⦁	One of the main features of Clang is its ability to produce highly optimized and efficient code.

⦁	Clang can be used in conjunction with other reverse engineering tools.

⦁	Clang's ability to produce highly optimized and efficient code makes it a valuable tool for reverse engineers who need to analyze complex and obfuscated binaries.

⦁	Clang is also highly customizable.

*ii.Clang++*:

⦁	Is a C++ compiler that is included in Kali Linux and is commonly used in reverse engineering tasks. It is a part of the Clang compiler family and provides support for C++14, C++17, and other modern C++ standards.

⦁	Has ability to produce highly optimized and efficient code. 

⦁	Clang++ also provides a range of powerful debugging and profiling features that can be used to identify bugs and performance issues in the code. 

⦁Is compatible with other tools and frameworks commonly used in reverse engineering.

⦁	Clang++ is highly customizable and can be configured to suit the specific needs and requirements of individual users.

*iii.NASM (Netwide Assembler)*:

⦁	Is a popular assembler used in Kali Linux for reverse engineering tasks. 

⦁It is a lightweight and efficient tool that can be used to assemble and disassemble binary code written in various assembly languages.

⦁	NASM is particularly useful for reverse engineers who need to analyze and disassemble machine code generated by compilers such as GCC and Clang.

⦁By using NASM to disassemble the code, reverse engineers can gain a deeper understanding of how the code works and identify potential security vulnerabilities or flaws.

⦁	NASM provides a range of powerful features that can be used to analyze and modify the assembly code.

⦁	NASM is also highly portable and can be run on various platforms.

⦁ NASM is an open-source tool, and its source code is available for modification and customization. 

**8.Exploitation Tools** :

It is an OS command Injection and Exploitation Tool used to test web applications for bugs, errors, and vulnerabilities related to command injection attacks. It is a tool to crack and decrypt BLE encryption that allows an attacker to guess or brute force the Temporary Key.

**a.CrackMapExec**:

⦁	CrackMapExec (CME) is a powerful open-source tool designed for penetration testing, active directory reconnaissance, and credential harvesting.

⦁	CME can be used to gather information about an Active Directory (AD) environment, including domain controllers, user accounts, groups, and computers.

⦁	CME can also be used to extract credentials from compromised systems or through password spraying attacks. 

⦁	CME can perform brute force attacks against SMB, SSH, and other services to crack passwords and gain access to systems.

⦁CME can exploit known vulnerabilities in systems.

**b.metasploit framework** :

⦁	The Metasploit Framework is an open source penetration testing and development platform.

⦁	It provides exploits for a variety of applications, operating systems and platforms.

⦁	 Metasploit is one of the most commonly used penetration testing tools and comes built-in to Kali Linux.

**c.searchsploit** :

⦁	SearchSploit is a command-line search tool for Exploit-DB that allows you to take a copy of the Exploit Database with you.

⦁	SearchSploit gives you the power to perform detailed off-line searches through your locally checked-out copy of the repository. 

⦁	This capability is particularly useful for security assessments on segregated or air-gapped networks without Internet access.

**9.Sniffing & Spoofing**:

The network can be a valuable source of information and offers a variety of potential attack vectors for a penetration tester. Sniffing network traffic can offer access to valuable intelligence, and spoofing traffic can enable a penetration tester to identify and exploit potential attack vectors.

**a.minicom**:

⦁	Minicom is a clone of the MS-DOS Telix communication program. 

⦁	Powerful tool for troubleshooting issues with serial devices.

⦁	Used to connectr modems,routers and serial devices in kali Linux.

⦁	Allow users to communicate real time.

⦁	Light weight and efficient tool.

**b.mitmproxy**:

⦁	MITMproxy is a powerful command-line tool that allows users to intercept, manipulate, and analyze HTTP(S) traffic on Kali Linux.

⦁	It is a popular tool for performing man-in-the-middle attacks and can be used to intercept traffic between clients and servers, allowing users to observe and manipulate the data being transmitted.

⦁	MITMproxy has a powerful scripting engine that allows users to automate tasks, such as modifying requests and responses, creating custom filters, and logging data to a file.

⦁	It provides an easy-to-use web interface that displays detailed information about the intercepted traffic, including the headers, body, and cookies.

⦁	MITMproxy has plugins that extend its functionality.

**c.Responder**:

⦁	Responder is an inbuilt Kali Linux tool for Link-Local Multicast Name Resolution (LLMNR) and NetBIOS Name Service (NBT-NS) that responds to specific NetBIOS queries based on the file server request.

**10.Post Exploitation** :

⦁ Post-exploitation refers to any actions taken after a session is opened.

⦁ A session is an open shell from a successful exploit or bruteforce attack. A shell can be a standard shell or Meterpreter.

**a.weevely**:

⦁ Weevely is a stealth PHP web shell that simulate telnet-like connection. 

⦁ It is an essential tool for web application post exploitation.

**b.powershell empire** :
⦁	This package contains a post-exploitation framework that includes a pure-PowerShell2.0 Windows agent, and a pure Python Linux/OS X agent. 

⦁	It is the merge of the previous PowerShell Empire and Python EmPyre projects. The framework offers cryptologically-secure communications and a flexible architecture.

⦁	On the PowerShell side, Empire implements the ability to run PowerShell agents without needing powershell.exe, rapidly deployable post-exploitation modules ranging from key loggers to Mimikatz, and adaptable communications to evade network detection, all wrapped up in a usability-focused framework.

**c.Proxychains** :

⦁	Is a UNIX program, that hooks network-related libc functions in dynamically linked programs via a preloaded DLL (dlsym(), LD_PRELOAD) and redirects the connections through SOCKS4a/5 or HTTP proxies. 

⦁	It supports TCP only (no UDP/ICMP etc).

**11.Forensics**:

Forensic tools are valuable not only for acquiring disk images but also for automating much of the analysis process, such as Identifying and recovering file fragments and hidden and deleted files and directories from any location.

**a. Autopsy(root)**: 

⦁	The Autopsy is a cyber forensic tool used for the analysis of Windows and UNIX file systems.

⦁	It can also be used to recover deleted files and also show various sectors of uploaded images making it easier to make an in-depth analysis of the image.

**b.Binwalk**:

⦁	Binwalk is a great tool when we have a binary image and have to extract embedded files and executable codes out of them.

⦁	 It is even used to identify the files and codes which are embedded inside the firmware images. 

⦁	Binwalk is compatible with magic signatures for UNIX file utility as it uses libmagic library.

**c.Bulk-Extractor tool**:

⦁	which is to be used when you have to extract features like E-Mail address, URLs, Confidential Document Numbers from files. 

⦁	This tool is used for Intrusion investigations, malware investigations, identity investigations, or any other kind of cyber investigation. 

⦁	The awesome feature of working with compressed or corrupt files makes it a great tool to work with those files. IT works on disk images, files, or a directory of files and finds out the useful information.

**12.Reporting tool**:

Reporting is one of the very important means in Ethical hacking or pen-testing. When a hacker or pen tester checks a system for loopholes or vulnerabilities then they need to provide an end report to the organization which consists of all the processes of discovering a vulnerability and also fixing it.

**a.Pipal**:

⦁	This tool is an Open Source Built Ruby for Password analysis. 

⦁	It can be used or come in handy when you are analyzing large password dumps that you used in the process of penetration testing activity.

⦁	This tool also comes pre-installed with Kali Linux and is found under-reporting tools in the application menu.

**b.Faraday start**:

⦁	Is a GUI application that consists of a ZSH terminal and a sidebar with details about your workspaces and hosts.

**c.CutyCapt**:

Is a small cross-platform command-line utility to capture WebKit’s rendering of a web page into a variety of vector and bitmap formats, including SVG, PDF, PS, PNG, JPEG, TIFF, GIF, and BMP.

**13.The Social-Engineer Toolkit (SET)**:

⦁	Is an open-source penetration testing framework designed for social engineering. 

⦁	SET has a number of custom attack vectors that allow you to make a believable attack in a fraction of time. 

**a.MSF Payload Creator (MSFPC)**:

⦁	Is a wrapper that generates multiple types of payloads. MSFPC is simple to use, and it aims to use as few as one option to produce a payload.

⦁	MSFC is used hand in hand with Metasploit.

⦁	To use MSFC, an attacker must only define the payload they want by either the platform or the file extension they want the payload to have.

**b.The Social-Engineer Toolkit (SET) (root)**:

Is an open-source penetration testing framework designed for social engineering.

⦁	SET has a number of custom attack vectors that allow you to make a believable attack in a fraction of time. These kind of tools use human behaviors to trick them to the attack vectors.


