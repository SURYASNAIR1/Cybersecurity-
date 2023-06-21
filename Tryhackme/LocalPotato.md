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
