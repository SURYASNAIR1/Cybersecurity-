**LOCAL POTATO (CVE-2023-21746)**


**TASK 1**

**INTRODUCTION**

Local potato is one of the very recently disclosed public vulnerabilities.
It was reported to Microsoft on September 9, 2022.
As we can see the identifier CVE 2023.
It works only on *windows*.
This vulnerability exploits a mechanism in *NTLM authentication*.
NTLM authentication is used widely in windows operating systems.  *So the major problem lies in NTLM authentication*.
Once there is flaw in NTLM authentication then local potato will work on any system.
When there is a flaw in internal authentication, when we run the local potato exploit its going to use a privileged process.
Privileged process is any process that runs under system user.
Local potato use a privileged process into launching a session against the available local server.
Here we are going to take an example of a SMB server.Because SMB server is the least challenging protocol.
We can use SMB,HTTP or DNS,FTP.
Once this is done the attacker will be able to connect with that server here it is SMB server to list all the shares and have admin privilege.

**IMPACTS**

Once the vulnerability is exploited the attacker will be able to:
* Write files as the system user.
* Read Files as the system user.

Microsoft has released a patch for this vulnerability  by making sure our windows is up to date to avoid being hacked.
Microsoft released a fix for the vulnerability in the January 2023 patch Tuesday.

so we can accomplish with local potato *we can have write or read privileges on the system it means we can resize the files and we can write the files*.

**Storsvc and DLL Hijacking**

Storsvc is the storage service .
Is a windows storage service which provide service for storage settings and extern extension storage .  
DLL means Dynamic Link Library is the library that contain code and data that can be used by more than one program at the same time.


*Exploiting the storage services by DLL Hijacking.*

What we can do here : We can edit or we can create our own DLL then given that  with local potato we can write files as system .We can write DLL or modify an existing DLL then achieve remote code execution through StorSvc and DLL Hijacking.

We need 2 items to make this work :
* We need a DLL name SprintCSP.dll .
This DLL is very much needed if we want to make calls to or by using the storage service.
So storage service by default when it is used or invoked it uses this DLL.
If that DLL is missing we can write our own DLL and replace it.
SprintCSP.dll exists under windows/system32 .
When we invoke storage service it loads that DLL .

* Remote Procedural Call Client.exe this will invoke call to the storage service which in turn load the DLL.

*With Local potato we can write files as system we can write our own DLL an then make RPC so when we invoke that service so we invoke SprintCSP.dll.*

**TASK 2**

**NTLM Authentication**

NTLM : New Technology LAN Manager
Is a suite of Microsoft security protocols intended to provide authentication , Integrity and Confidentiality to users.
NTLM is more secure and requires multiple exchange  between client and server.
The usual case of NTLM authentication involves a user trying to authenticate to a remote server. Three packets are involved in the authentication process:

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/d77d0bc7-4c03-45b4-914b-4f3eeea90d83)

*Type 1 Message: The client sends a packet to negotiate the terms of the authentication.
The packet contains the name of the client machine and its domain.
The server receives the packet and can check that authentication was started from a different machine.

*Type 2 Message: The "challenge" is a random number used to authenticate the client without having to pass their credentials through the network.

*Type 3 Message: The client uses the challenge and combines it with the user's password hash to generate a response to the challenge. 
The server can check if the client knows the correct user's password hash without transferring it through the network. 

**NTLM Local Authentication**

User tries to log into a service running on the same machine. 
Since both the client and server applications reside on the same machine, there is no need for the challenge-response process.
So here the authentication is done by setting up a Security Context which a set of security parameters associated with a connection, including the session key and the user whose privileges will be used for the connection.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/4c173d2e-5084-47e7-9334-365c02f51dbb)

*Type 1 Message: I f the crdedntial matches then only the process will began.

*Type 2 Message: The server creates a Security Context and sends back its ID to the client in this message. The client can then use the Security Context ID to associate itself with the connection.

*Type 3 Message: If the security context ID success then empty message is send to signal that the local authentication process succeeded.

**Task 3** 

**LocalPotato**

Take advantages of flaw in NTLM local authentication.
This attacker get access to privileges.
Attacker will start local SMB server authentication.
SMB means Server Message Block.Is a network file sharing protocol that allows applications on a computer to read or write to files to requires services from server programs in a computer network.
The attacker ends up having a connection that grants him access to special shares like C$ (Default drive share) or ADMIN$ (Remote admin).

*Process*

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/9c8eea1d-c36b-441a-a98f-cc0314b6f02c)

*The attacker will trigger a privileged process to connect to a rogue server under his control.
*The rogue server will instantiate a Security Context A for the privileged connection but won't send it back immediately.
attacker will launch a rogue client that simultaneously initiates a connection against the local SMB Server (Windows File Sharing) with its current unprivileged credentials. The client will send the Type1 message to initiate the connection, and the server will reply by sending a Type2 message with the ID for a new Security Context B.
*The attacker will swap the Context IDs from both connections so that the privileged process receives the context of the SMB server connection instead of its own. As a result, the Privileged client will associate its user (SYSTEM) with Security Context B of the SMB connection created by the attacker. As a result, the attacker's client can now access any network share with SYSTEM privileges.

By having a privileged connection to SMB shares, the attacker can read or write files to the target machine in any location. 

**Task 4**

**Abusing StorSvc to Execute Commands**

Attacker would need to write DLL into systems path to trigger it.
By default ,windows PATH will only include directories that only privileged accounts can write.
We can find machines where the installation of specific applications has altered the PATH variable and made the machine vulnerable.

**TASK 5**

**Elevating Your Privileges**


**WHAT I DID**

* By opening the attack box I can see a folder named Tools .

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/7f277955-0514-46c6-aa4d-2c1d40120a36)

*Open the main.c in notepad.And change how the DLL works.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/24a09ae9-7a81-44b0-bfe5-eb6ccae27c12)

* The below line says the the command prompt will run execute whoami and then store the output under program data under whoami.txt.

![WhatsApp Image 2023-06-21 at 18 32 16](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/541343b2-bf67-420e-bbc7-d1df836a5f23)

* Add the existing user into administratory group .The username is userSo in a set of issuing whoami we're going to actually  add the user into administrator group thus elevating the privileges.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/063780fa-6948-4839-a9f2-547f71e60819)

* Changes are made in the Create process area then save it.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/677472d8-0547-4a72-a76a-8b38cac18fa5)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/60c8455d-d308-434b-b00e-03900a049d3e)

Here we have main.c 

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/b7ca890b-f644-4b62-b74a-d98446bff363)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/27fa0144-b876-4c58-8f33-b9529ebe0a2e)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/4e55021f-7ed7-4ba4-a843-477caecc2042)

![WhatsApp Image 2023-06-21 at 18 58 26](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/e579cfd2-a9ff-4127-833f-dcc27af14e4a)

![WhatsApp Image 2023-06-21 at 18 59 14](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/9649de36-5397-4c94-917c-d8e795ae92d3)

![WhatsApp Image 2023-06-21 at 19 00 13](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/2d655ad2-0f17-486b-afd7-299386b93013)

![WhatsApp Image 2023-06-21 at 19 01 04](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/26e2a970-53e3-4906-9d71-10140ca21f1c)

![WhatsApp Image 2023-06-21 at 19 02 10](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/4ffa982d-96dc-4880-adcd-855306a0c93c)

![WhatsApp Image 2023-06-21 at 19 03 39](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/f26853e3-4ae1-431c-a4e3-479cf0e2b141)

![WhatsApp Image 2023-06-21 at 19 04 40](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/e386dd37-3772-4ea3-90cb-6822ffc58e72)

![WhatsApp Image 2023-06-21 at 19 06 25](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/968e9990-7c6a-4cd6-b6c2-a41942a1d5b6)

![WhatsApp Image 2023-06-21 at 19 06 25](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/19566817-90eb-4b74-9326-77f54c6b5613)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/bcb80910-3703-4b32-9bad-942a0e212ddc)

![WhatsApp Image 2023-06-21 at 19 12 49](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/dd8a74dd-187a-477b-a942-63157745ac86)

![WhatsApp Image 2023-06-21 at 19 12 49](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/b978a346-3ba2-402a-a988-3b23a48841a5)

![WhatsApp Image 2023-06-21 at 19 15 08](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/ddb0641f-ae2b-426b-8d86-7002ab2a0ff7)

![WhatsApp Image 2023-06-21 at 19 15 57](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/29292c48-20d9-4d89-830d-187333f37456)

![WhatsApp Image 2023-06-21 at 19 18 03](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/e950b0ad-88a0-4694-87da-9ac5554491f9)

![WhatsApp Image 2023-06-21 at 19 18 50](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/1b75b9c5-7b49-4181-a6c4-63d2fc0374b7)

![WhatsApp Image 2023-06-21 at 19 20 56](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/a5c3bbab-8533-4630-9853-5c83c7940512)


![WhatsApp Image 2023-06-21 at 19 25 55](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/7ea942d6-3795-437e-8c41-1066ebe4b73e)


![WhatsApp Image 2023-06-21 at 19 27 49](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/8cffa3e0-8f69-4a30-b633-f0845ba65754)

**Task 6**

**Detection/Mitigation**

*Detect* by using the pattern matching tool YARA.To detect the file patterns and examine the events generated by the execution of this hack tool localpotato.exe.

*YARA Rule*

Identifying and classifying malware samples.
Detect the presence of localpotato.exe hack tool, within the system.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/a564f096-8220-4d07-a263-0e3bb57c320e)

The code is a function that detects the local potato exploit.

The condition is all of them. The function will only run if all of the following conditions are met.

 $CLSID = "854A20FB-2D44-457D-992F-EF13785D2B51"   means the name of the exploit.

 CLSID is a globally unique identifier that identifies a COM class object. It is either 32 continuous hexadecimal digits or groups of 8,4,4,4 and 12 hexadecimal digits separated by hyphens.

 $localpotato = {6c 6f 63 61 6c 70 6f 74 61 74 6f}   is looking for an exploit with this string in its name and it's expecting to find one with this value.

 $function = "NtQueryInformationProcess"  to detect local potato exploit present on system or not.

 *Mitigation*

 * Ensure all systems are stay updated with the latest security patches.
 *  Least privilege principle : User access to only the resources they need to perform their job functions.
 *  Monitor suspicious activities using Splunk.
   
