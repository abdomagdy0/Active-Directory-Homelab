<h1>Active Directory homelab</h1>

<h2>Description</h2>
In this lab, we will  walk through how you can create an active Directory home lab Environment using Virtual Box. Configuring and running this lab will definetly help develop your understanding of how active directory and widnows networking works, so i'd highly suggest creating your own AD home lab.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Oracle Virtual Box</b>


<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Windows Server 2019</b>

<h2> walk-through:</h2>
<p align="center">
our goal is to create the windows server Virtual Machine which will become our domain controller, give it two network adapters one of which is going to be used to connect to the internal network, and the other one will be used to connect to the outside network (internet), once that's done were going to sign IP Adressing for the internal network, Configure NAT, Routing, and DHCP on the Domain controller so the clients on the private network can get automatic IP Adressesing and browse the internet through the Domain Controller.step two is to rename the server and Setup Active Directory, and lastly create multiple users with a Powershell script.
 
Here is a diagram of how the lab should look like

 ![image](https://github.com/abdomagdy0/Active-Directory-Homelab/assets/91535529/1e703464-f594-4157-8592-cf152fe0438e)

</p>
Virtual Box:
go to https://www.virtualbox.org/wiki/Downloads and select the latest version for your Operating system

![image](https://github.com/abdomagdy0/Active-Directory-Homelab/assets/91535529/4c298c27-72bc-4fc1-abab-18c2fc6c2142)

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
