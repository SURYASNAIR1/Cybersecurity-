**Follina MSDT (CVE-2022-30190)**

**Intro to MSDT**

* Microsoft Support Diagnostic Tool (MSDT) is a service in Windows 11/10/8.1/7 and windows server.
* The tool enables Microsoft support representatives to analyze diagnostic data and find a resolution for the problems experienced by users.

**What is Follina MSDT 0-day vulnerability?**

* Follina is the nickname given to a new vulnerability discovered as a zero-day and identified as CVE-2022-30190.
* It is a Remote Code Execution Vulnerability in the Microsoft Windows Support Diagnostic Tool (MSDT).
* Affected Platforms: Microsoft Windows
* Affected Parties: Microsoft Windows users
* Impact : Full control of the affected machine
* Severity level: Critical

**Who detected and working of Follina**

*Individual security researcher nao_sec found this vulnerability.
He checked the virus Total where one of the file was uploaded.This Vulnerability existed long year back but nobody detected it .

**Working and Flow of Follina Vulnerability**

1. A Microsoft Office.DOC file crafted by an attacker is sent to a target.
2. The word document contain some link of HTML file.
   The .DOC file references a HTTPS:link leading to an HTML file containing obfuscated Java script.
   That contain secret information.
3. The JavaScript code references another link with an identifier MS-MSDT.

When we click on the HTML link then when we check the URL bar of that browser there will be some HTTP or HTTPS.
But here it is redirecting or we can say calling this msdt.exe.

4. Windows OS open the MSDT and run code contained in the provided link.

So whatever is present in that link is going to execute.

5. Depending on the coed executed on the targeted system,the attacker might facilitate further compromise or take control of the affected system.

**Exploit of Follina MSDT Vulnerability**

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/202e895a-26a4-4ebb-9698-cb793fbf5cb7)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/2426c195-58f4-4d9e-9bb2-3e82ee6527d1)

**Detection and Mitigation**
