![image](https://github.com/abdomagdy0/Active-Directory-Homelab/assets/91535529/183552bd-4928-4b1e-9cff-7413cb0632bb)![image](https://github.com/abdomagdy0/Active-Directory-Homelab/assets/91535529/e3b9d113-f832-4284-89a0-c7c9e6519fb2)<h1>Active Directory homelab</h1>
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
![image](https://github.com/abdomagdy0/Active-Directory-Homelab/assets/91535529/d411822f-46d0-4d85-b417-0072864e7c00)
</p>
<b>Virtual Box:</b>
<p>go to https://www.virtualbox.org/wiki/Downloads ,and choose the latest version for your Operating system.
 <p>Install and open VB, then click on the add icon and select the server iso. </p>
 </p
once you install virtualbox, create a new machine.

![image](https://github.com/abdomagdy0/Active-Directory-Homelab/assets/91535529/84115a56-a759-47a0-a16a-68c88567f271)
<p>make sure to set around 2gbs of ram at minimum for Windows server as anything less would not run, I prefer 4-8gbs, and set max cpu cores for your cpu to make the installation process faster. </p>

you need to select the one with desktop environment, create custom install and click next, let it install.
![image](https://github.com/abdomagdy0/Active-Directory-Homelab/assets/91535529/d0068d2f-c345-4fb6-a6ea-77b012f17921)

<p> repeat the process for the windows 10 VM</p>

<P> Install Guest Additions to make the experience more fluid</P>
let it install and reboot your machine.



 
 

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
