 <u>OCAL POTATO (CVE-2023-21746)

**INTRODUCTION**

Local potato is one of the very recently disclosed public vulnerabilities. As we can see the identifier CVE 2023.
It works only on windows.
This vulnerability exploits a mechanism in NTLM authentication.
NTLM authentication is used widelyin windows operating systems.  So the major problem lies in NTLM authentication.
Once there is flaw in NTLM authentication then local potato will work on any system.
When there is a flaw in internal authentication, when we run the local potato exploit its going to use a privileged process.
Privileged process is any process that runs under system user.
Local potato use a privileged process into launching a session against the available local server.
Here we are going to take an example of a SMB server.Because SMB serveris the least challenging protocol.
We can use SMB,HTTP or DNS,FTP.
Once this is done the attacker will be able to connect with that server here it is SMB server to list all the shares and have admin privilege.

**IMPACTS**

Once the vulnerability is exploited the attacker will be able to:
* Write files as the system user.
* Read Files as the system user.

Microsoft has released a patch for this vulnerability  by making sure our windows is up to date to avoid being hacked.

so we can accomplish with local potato **we can have write or read privileges on the system it means we can resize the filesand we can write the files**.
