**Phishing Analysis Tools**

**INTRODUCTION**

In this room, we will look at various tools that will aid us in analyzing phishing emails. We will: 

Look at tools that will aid us in examining email header information.
Cover techniques to obtain hyperlinks in emails, expand the URLs if they're URL shortened.
Look into tools to give us information about potentially malicious links without directly interacting with a malicious link.
Cover techniques to obtain malicious attachments from phishing emails and use malware sandboxes to detonate the attachments to understand further what the attachment was designed to do.

Below is a checklist of the pertinent information an analyst (you) is to collect from the email header:

*Sender email address
*Sender IP address
*Reverse lookup of the sender IP address
*Email subject line
*Recipient email address (this information might be in the CC/BCC field)
*Reply-to email address (if any)
*Date/time

*Afterward, we draw our attention to the email body and attachment(s) (if any).

Below is a checklist of the artifacts an analyst (you) needs to collect from the email body:

*Any URL links (if an URL shortener service was used, then we'll need to obtain the real URL link)
*The name of the attachment
*The hash value of the attachment (hash type MD5 or SHA256, preferably the latter)


What is the official site name of the bank that capitai-one.com tried to resemble?

Ans : Google the website capitai-one.com so we can see the answer https://www.capitalone.com/

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/b5972a3e-2416-4b11-b462-ecb94c602148)

How can you manually get the location of a hyperlink?

Ans : copy link location

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/e5deef05-d56b-4939-9007-89119eb1454b)


Look at the Strings output. What is the name of the EXE file?

Ans : We can see the answer in the string section as  #454326_pdf.exe

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/4212456a-2d87-40e1-9a67-2170f898c52e)

**Phishing Case 1**

What brand was this email tailored to impersonate?

Ans : Netflix

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/c8a8d226-1d51-49e0-a1f6-c1899d1edf8a)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/43e20c8f-2c71-49ba-835e-7210edb4c80e)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/983c0094-802b-40a5-8e67-3aa411226f2b)

What is the From email address?

Ans : JGQ47wazXe1xYVBrkeDg-JOg7ODDQwWdR@JOg7ODDQwWdR-yVkCaBkTNp.gogolecloud.com

![Untitled](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/e20be4b1-c5a1-432e-aa38-ecb6cfb1f74e)

What is the originating IP? Defang the IP address. 

Ans : I used cyberchef to defang the IP adress

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/3da4a130-4a62-41bd-b30b-455a92f1f17c)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/27ee1f8e-350e-4f73-8de1-68d0a17ef398)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/f90eb1ee-009d-4b3d-b59d-6c78279c35cf)

209[.]85[.]167[.]226

From what you can gather, what do you think will be a domain of interest? Defang the domain.

Ans : Find this information in the Return-path of the mail.Defang it with cyberchef.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/154ebae2-24ad-4dec-a018-4d55c5da5b8e)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/44a98feb-9cac-4f49-9968-82de598f60c1)


What is the shortened URL? Defang the URL.

Ans : In the message URLs you have the link.Just defang it with cyberchef.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/23a3abb2-7ff3-47f3-8ac1-8007ae53118d)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/b3d208c9-aa15-4ef1-85ab-df2ee47f386b)

**phishing Case 2**

What does AnyRun classify this email as?

Ans: On the right of anyrun it's written as Suspicious activity.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/f60db480-2ef4-4b4f-82c0-130ab36947c6)

What is the name of the PDF file?

Ans: payment-updateid.pdf

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/bc7b5994-4f5a-4fdd-ae49-e8cc240d157b)

What is the SHA 256 hash for the PDF file?

Ans: cc6f1a04b10bcb168aeec8d870b97bd7c20fc161e8310b5bce1af8ed420e2c24

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/8960b4cb-d01a-4825-9ef6-ddf27d452e47)

What two IP addresses are classified as malicious? Defang the IP addresses. (answer: IP_ADDR,IP_ADDR)

Ans: 2[.]16[.]107[.]24,2[.]16[.]107[.]83

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/40791a23-b440-4bf3-a96e-a1f443f68915)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/2af4a689-9bfa-43f6-a21c-ff03dca65066)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/e585ddf0-1489-4f74-a224-9b06529ab76e)

What Windows process was flagged as Potentially Bad Traffic?

Ans : svchost.exe

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/3c34ec2f-39da-43c4-8402-2b5d89380dea)

**svchost.exe

