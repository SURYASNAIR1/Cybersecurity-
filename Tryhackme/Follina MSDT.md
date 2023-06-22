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

![WhatsApp Image 2023-06-22 at 08 06 21](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/d8115a23-6083-4f6b-93bc-f42d02dea0d9)

![WhatsApp Image 2023-06-22 at 08 07 30](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/524a239f-aff4-4d90-a396-984a1c737c3f)

![WhatsApp Image 2023-06-22 at 08 08 11](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/36196e1e-bd3b-46ae-b405-94a88b4d1e17)

![WhatsApp Image 2023-06-22 at 08 09 04](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/33a317be-805d-4103-b702-e98467136712)

![WhatsApp Image 2023-06-22 at 08 10 40](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/7a0e7bcb-b497-4273-b529-159840026f09)

![WhatsApp Image 2023-06-22 at 08 11 34](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/46fd4afe-0877-46f8-9b88-a631b0d52302)

![WhatsApp Image 2023-06-22 at 08 13 34](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/f5ae82e4-c559-40c6-a05f-274ebc340109)

![WhatsApp Image 2023-06-22 at 08 15 19](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/7a78106b-ddeb-4be3-be1f-9277f3c6e681)

![WhatsApp Image 2023-06-22 at 08 16 28](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/334897aa-42e0-4fbd-98c9-9929b73a3bca)

![WhatsApp Image 2023-06-22 at 08 18 24](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/886cc6bf-6b34-431d-9c9a-7c73b8872115)

**Detection**

![WhatsApp Image 2023-06-22 at 08 19 19](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/1e9eed6a-9586-47f4-ab08-49ea68e28634)

![WhatsApp Image 2023-06-22 at 08 20 05](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/17188433-12b6-4314-87a4-353c745eba19)


![WhatsApp Image 2023-06-22 at 08 25 02](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/9c3dd7af-538b-45b0-921e-c6db1581ace6)

![WhatsApp Image 2023-06-22 at 08 23 21](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/06836187-6745-437c-8e03-1bb96d527db6)


![WhatsApp Image 2023-06-22 at 08 24 17](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/5ff1f2cf-831e-4c09-94f7-b421b977a2b6)

![WhatsApp Image 2023-06-22 at 08 27 12](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/855446a2-5284-4ec0-a28e-c1888bae9d37)

**Remediation**

* The patch for this vulnerability is in the June 2022 cumulative Windows Updates.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/0f223e54-093d-4466-bbd2-1836368c2f6e)

* Disable MSDT URL Protocol.

By disabling the MSDT URL Protocol, troubleshooters will not be launched as links and so ms-msdt won’t be able to be called by Office.
We're always changing our working directory to the Desktop - it's so we can immediately see the changes that our commands are introducing to the environment.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/34da30a6-381c-4ee8-a637-751174f5dcfa)

* reg query command quick check that the key exists.
* reg export that exports our key into a file so we may be able to reintegrate it in our system later on when Microsoft comes up with a more permanent fix to this vulnerability. The exported file is saved in the current working directory - in our case the Desktop.
* The reg delete command disables the MSDT URL Protocol mainly because it essentially removes it altogether from the system.
* The final reg query command is a confirmatory check that the key no longer exists.


*Attack Surface Reduction (ASR)

If you’re using Microsoft Defender for Endpoint in your environment, enable the ASR rule Block all Office applications from creating a child.
