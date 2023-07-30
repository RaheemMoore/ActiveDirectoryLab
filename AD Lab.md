<h1>Active Directory: Domain and User Configuration</h1>

<h2>Description</h2>
<h3>What is Directory Service?</h3>
Before explaining “Active Directory”, let’s first explain what is Directory Services. Directory Services is the software system that is used to store and locate data within a network. Prior to directory services, to locate a file, a user would need to know the files name, which server it is stored on, and the folder path. This may be acceptable in some small networks, but organizations possess large amounts of data that needs to be easily accessible at any time. Active Directory is Microsoft's answer to this problem.

<h3>What is Active Directory?</h3>
Active Directory does more than just store and locate data within the network, it also provides the method for making the information available to network users and administrators. Security is integrated into Active Directory, which uses Kerberos Authentication and SSO services. Users can use one set of credentials to gain access certain resources and services. In summary, Active Directory serves as a centralized security management solution that houses all network resources.

<h3>What is Stored in Active Directory or AD?</h3>
There are two types of objects stored within the AD. The first is Container objects, which are objects that store other objects. The second is Leaf objects, which are individual objects that do not contain other objects. Common objects stored in the AD include:
<br />
<br />

- User accounts and their passwords 
- Computers
- Printers
- File Shares
- Applications
- Security Groups

Active Directory enables administrators to centrally manage an organizations network. A few of the most common uses of AD include changing the hierarchy of objects, overseeing the access control list, and setting permissions for specific groups.

<br />


<h2>Primary Skills</h2>

- <b>PowerShell</b>
- <b>Windows OS</b>
- <b>VMware</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>
- <b>Windows Server 2019</b>
- <b>VMware Workstation</b>

<h2>Lab walk-through:</h2>

<p align="center">
Network Diagram:  <br/>
<img src="https://imgur.com/sq3VIaY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure the network adapters with information from the network diagram. The server will use itself as a DNS. <br/>
<img src="https://imgur.com/HM4f17B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install Active Directory Domain Service.  <br/>
<img src="https://imgur.com/NIMmfLm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create the domain. For example, this project uses companydomain.com. <br/>
<img src="https://imgur.com/bOZH4kn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Within the domain, create an Organizational Unit named _ADMIN. Then create your first admin and give it privileges.  <br/>
<img src="https://imgur.com/3FPrjRY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install RAS/NAT services and enable IPv4 routing. This will allow clients on the private network to access the internet using the Domain Controller. <br/>
<img src="https://imgur.com/nHY5hYM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install DHCP services and configure the scope of IP addresses that will leased. This will allow users that join the domain to automatically be assigned private IP addresses.<br/>
<img src="https://imgur.com/DO7ajS7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Use PowerShell to create 1000 users to imitate a corporate environment. You will need to disable security features to enable the use of the script provided in this lab.   <br/>
<img src="https://imgur.com/Vc7zryN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Log onto one of the generated users. Ping www.google.com to make sure the user can access the internet. Ping the domain created earlier in the lab to make sure it can be accessed. Run ipconfig and make sure the IP address is within the specified scope. <br/>
<img src="https://imgur.com/zCAf6xL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Add the user to the domain using the credential of the admin account created earlier in the lab.  <br/>
<img src="https://imgur.com/Vg2LDbC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Check the DHCP server and make sure there is a lease for the user that was just added to the domain.  <br/>
<img src="https://imgur.com/xMkzHT9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
