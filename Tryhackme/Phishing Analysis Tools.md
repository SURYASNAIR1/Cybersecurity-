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

