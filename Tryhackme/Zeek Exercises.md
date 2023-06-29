**Task 1  Introduction**

The room invites you a challenge to investigate a series of traffic data and stop malicious activity under different scenarios. 
Start working with Zeek to analyse the captured traffic.

**Task 2  Anomalous DNS**

Q : Investigate the dns-tunneling.pcap file. Investigate the dns.log file. What is the number of DNS records linked to the IPv6 address?

Ans: 320

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/5a6aa79e-ea76-407c-b695-25980708d6ff)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/bf6b217b-a882-4d18-9f10-1b950ec1b67b)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/1c912d12-b2df-4043-9484-b26486602ad1)

Q: Investigate the conn.log file. What is the longest connection duration?

A: 9.420791

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/e4121a6d-3351-47f6-9892-22d024b0854b)

Q: Investigate the dns.log file. Filter all unique DNS queries. What is the number of unique domain queries?

A: 6

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/39863489-3796-49e4-a86b-1b38958b1847)

There are a massive amount of DNS queries sent to the same domain. 
This is abnormal.
Let's find out which hosts are involved in this activity. 
Investigate the conn.log file.
What is the IP address of the source host?

A: 10.20.57.3

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/261a45ae-32f7-41c2-8100-0990f613bbb2)

**Task 3  Phishing**

Q: Investigate the logs. What is the suspicious source address? Enter your answer in defanged format.

Ans : 10[.]6[.]27[.]102

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/b76a67ff-cc5f-4d0c-bfd6-e4ae2faf560f)

Q: Investigate the http.log file. Which domain address were the malicious files downloaded from? Enter your answer in defanged format.

A: smart-fax[.]com

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/31597f44-b34d-4d46-8fa2-60d5e182d785)

Q: Investigate the malicious document in VirusTotal. What kind of file is associated with the malicious document?

A: vba

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/d1cf87c9-68d5-4504-8682-6e8d0d06afe9)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/b9667f37-2704-4606-8eb9-11755771fd8e)

Q: Investigate the extracted malicious .exe file. What is the given file name in Virustotal?

A: pleasewaitwindow.exe

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/dfa6abff-bcaf-43cd-abe8-69b6258a66e5)

Q: Investigate the malicious .exe file in VirusTotal. What is the contacted domain name? Enter your answer in defanged format.

A: hopto[.]org

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/40bf2d29-8d8c-43ce-871e-719f14d3fbed)
