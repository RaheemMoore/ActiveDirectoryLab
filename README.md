<h1>Active Directory Home Lab</h1>

<h2>Description</h2>
<h3>What is Directory Service</h3>
Before explaining “Active Directory”, let’s first discuss what is Directory Services. Directory Services is the software system that is used to store and locate data within a network. Prior to directory services, to locate a file, a user would need to know the files name, which server it is stored on, and the folder path. This may be acceptable in some small network, but organizations possess large amounts of data that needs to be easily accessible at any time. Active Directory is Microsoft answer this problem.

<h3>What is Active Directory</h3>
Active Directory does more than just store and locate data within the network, it also provides the method for making the information available to network users and administrators. Security is integrated into Active Directory, which uses Kerberos Authentication and SSO services. Users can use one set of credentials to gain access certain resources and services. In summary, Active Directory serves as a centralized security management solution that houses all network resources.

<h3>What is Stored in Active Directory?</h3>
There are two types of objects stored within the AD. The first is Container objects which are objects that store other objects. The second is Leaf objects which are individual objects that do not contain other objects. Common information stored in the AD includes:
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


<h2>Goals</h2>

- <b>PowerShell</b> 
- <b>Diskpart</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>
- <b>Windows Server 2019</b>

<h2>Lab walk-through:</h2>

<p align="center">
Configure the network adapters with information from the network diagram: <br/>
<img src="https://imgur.com/HM4f17B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
