**Task 1 : Introduction**

Microsoft's Active Directory is the backbone of the corporate world. 
It simplifies the management of devices and users within a corporate environment.

**Task 2 : Windows Domains**

1. Initially, managing a small business network with five computers and five employees is relatively simple, with the ability to configure each computer separately.
2. As the business grows to 157 computers and 320 users across multiple offices, manual management becomes impractical and inefficient.
3. To overcome these limitations, a Windows domain is used, which is a group of users and computers under the administration of a business.
4. The main component of a Windows domain is Active Directory (AD), which serves as a central repository for network administration.
5. A Domain Controller (DC) is the server that runs Active Directory services.
6. Benefits of a configured Windows domain include centralised identity management and the ability to manage security policies across the network.
7. A real-world example of a Windows domain is seen in school or university networks, where users can access any computer using their credentials, which are verified by Active Directory.
8. Active Directory allows for the enforcement of policies, such as restricting access to certain features or granting administrative privileges.
9. The task at hand is to review and make additional configurations to the "THM.local" domain as the new IT admin at THM Inc. Administrative credentials will be provided for a pre-configured Domain Controller (DC) to perform the tasks.

Q: In a Windows domain, credentials are stored in a centralised repository called…

Ans: Active Directory

Q: The server in charge of running the Active Directory services is called…

Ans:Domain Controller

**Task 3 : Active Directory**

1. The Active Directory Domain Service (AD DS) is the core of a Windows Domain, functioning as a catalog that stores information about all objects in the network.
2. AD supports various types of objects, including users, groups, machines, printers, shares, and more.
3. Users are one of the most common object types in Active Directory and are considered security principals.
4. Users can be authenticated by the domain and assigned privileges over network resources like files or printers.
5. Security principals are objects that can act upon network resources.
6. Users in Active Directory can represent two types of entities: people (such as employees) and services (used by applications like IIS or MSSQL).
7. Service users are different from regular users as they have privileges specific to running their respective services.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/437870ba-3aa5-4519-b796-fdd74edf7d11)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/3c19c0ae-54d9-45b6-b32e-3709314e59a7)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/9570235e-ea38-4624-a49b-51d4582bab69)

Q: Which group normally administrates all computers and resources in a domain?

Ans :Domain Admins

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/f37abdf9-b2f6-4636-82ef-646144471561)

Q: What would be the name of the machine account associated with a machine named TOM-PC?

Ans : TOM-PC$

Suppose our company creates a new department for Quality Assurance. What type of containers should we use to group all Quality Assurance users so that policies can be applied consistently to them?

Ans : Organizational Units.

**Task 4: Managing Users in AD**

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/e8748cdd-1d49-442f-9829-8b5e712abae3)

**Delegation**

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/1c7117a5-918c-4cca-b384-668704d6a6af)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/e3a0960f-550f-4a66-8928-409d301b1f81)

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/2c63a917-ec5a-4954-94ca-a56f4a94841c)


![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/4f1ae61f-ca36-4b62-864f-97b77d54cb31)

Q : What was the flag found on Sophie's desktop?

Ans : THM{thanks_for_contacting_support}

Enter account of sophie with new password.

![image](https://github.com/SURYASNAIR1/Cybersecurity-/assets/123303806/e0942f40-1cea-4e5e-b638-19a0de884a36)

Q : The process of granting privileges to a user over some OU or other AD Object is called...

Ans : Delegation

**Task 5 : Managing Computers in AD**

Q : After organising the available computers, how many ended up in the Workstations OU?

Ans : 7

Q : Is it recommendable to create separate OUs for Servers and Workstations? (yay/nay)

Ans : yay

**Task 6 : Group Policies**

Q : What is the name of the network share used to distribute GPOs to domain machines?

Ans : sysvol

Q: Can a GPO be used to apply settings to users and computers? (yay/nay)

Ans : yay

**Task 7 : Authentication Methods**

Q: Will a current version of Windows use NetNTLM as the preferred authentication protocol by default? (yay/nay)

Ans :nay

Q: When referring to Kerberos, what type of ticket allows us to request further tickets known as TGS?

Ans : Ticket Granting Ticket

Q: When using NetNTLM, is a user's password transmitted over the network at any point? (yay/nay)

Ans : nay

**Task 8 : Trees, Forests and Trusts**

Q: What is a group of Windows domains that share the same namespace called?

Ans :tree

Q: What should be configured between two domains for a user in Domain A to access a resource in Domain B?

Ans : a  trust relationship

**Task 9 : Conclusion**

In this room, we have shown the basic components and concepts related to Active Directories and Windows Domains.
