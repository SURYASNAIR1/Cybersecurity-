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
