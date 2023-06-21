**LOCAL POTATO (CVE-2023-21746)**

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

so we can accomplish with local potato **we can have write or read privileges on the system it means we can resize the files and we can write the files**.

**Storsvc and DLL Hijacking**

Exploiting the storage services by DLL Hijacking.
What we can do here : We can edit or we can create our own DLL then given that  with local potato we can write files as system .We can write DLL or modify an existing DLL then achieve remote code execution through StorSvc and DLL Hijacking.
We need 2 items to make this work :
* We need a DLL name SprintCSP.dll .
This DLL is very much needed if we want to make calls to or by using the storage service.
So storage service by default when it is used or invokedit uses this DLL.
If that DLL is missing we can write our own DLLand replace it.
SprintCSP.dll exists under windows/system32 .
When we invoke storage service it loads that DLL .

* Remote Procedural Call Client.exe this will invoke call to the storage service which in turn load the DLL.

**With Local potato we can write files as system we can write our own DLL an then make RPC so when we invoke that service so we invoke SprintCSP.dll .
