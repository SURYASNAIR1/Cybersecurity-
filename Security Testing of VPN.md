


1.Create anIPsec-basedVPN with the help of the Strongswan tool.
a.Configure it with IKE version 1, performthe pen-testingprocedures,and make it to IKE version 2 and follow the same. Add your observations tothe report.
![WhatsApp Image 2023-04-23 at 23 08 53](https://user-images.githubusercontent.com/123303806/233855947-5174d01f-65ac-4be8-b0fe-7593f6647e86.jpg)
![WhatsApp Image 2023-04-23 at 23 07 39](https://user-images.githubusercontent.com/123303806/233855977-fadfbfc7-d8bf-4231-a43c-ba510b2ab52e.jpg)
![WhatsApp Image 2023-04-23 at 23 10 21](https://user-images.githubusercontent.com/123303806/233855989-b8e584ba-db76-4542-804f-b4e3552a9a58.jpg)

b.Configure your PSK to your own key phrase,then try to crack it offline. Then followthe same by creating a random auto-generatedPSK and try the same. 

2.Pen testingparametersfor VPN:
a.Scanning or identifying the VPN gateway.
b.Fingerprinting the VPN gateway for guessing implementation.
c.PSK mode assessment and PSK sniffing.
d.Offline PSK cracking.
e.Checking for default user accounts.
f.Testing the VPN gateway for vendor-specificvulnerabilities.
g.Check is there any firewall is present in this networkbefore VPN.
+h.Perform necessaryIKEscans
