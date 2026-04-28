<h1>Active Directory Lab - Promote Server</h1>

<h2>Description</h2>
This project demonstrates the process of deploying and configuring an Active Directory Domain Service (AD DS) environment on a Windows Server 2022 virtual machine hosted in Oracle VirtualBox. This lab includes promoting a standalone server to a domain controller and adding Active Directory roles and features preparing the foundation for enterprise-level identity and access management. 

<br />

<h2>Purpose:</h2>
This lab was created to simulate a real-world enterprise envionment using Windows Server 2022 and Active Directory. The goal is to develop pratical experience in identity and access management, including organizing resources with Organizational Units, enforcing policies with Group Policy, and managing user permissions in a controlled domain environment. 

<br />

<h2>Lab Tasl:</h2>
- <b>Promote server to domain controller</b>
<br />
- <b>Add Active Directory role</b>

<h2>Promote server to Domain Controller:</h2>
<br />
- <b>Login to Virtual Machine</b>
<br />
- <b>Within Server Manager, select the flag with the alert notification</b>
<br />
<br />
<p align="center">
- <b>Click "Promote this server to a domain controller"</b>
<img src="PromoteDC.PNG" height="80%" width="80%" alt="Promote server to DC"/>
</p>
<br />
- <b>Domain Controller Wizard Window will open</b>
<br />
<br />
<p align="center">
- <b>Select options and set password for adminstrator account</b>
<img src="DCOptions.PNG" height="80%" width="80%" alt="DC Wizard Window"/>
</p>

<br />
- <b>VM will require a reboot in order to save configurations</b>
<br />
<br />
<p align="center">
- <b>After reboot, login using Administrator username and password created during the Domain Controller Wizard</b>
<img src="DCLogin.PNG" height="80%" width="80%" alt="DC Login"/>
</p>
<br />
<br />
<h2>Add Active Directory roles and features:</h2>
<br />
- <b>After logging into admin account, select "Manage"</b>
<br />
- <b>Select "Add Roles and Features", wizard window will prompt</b>
<p align="center">
  <img src="AddRoles.PNG" height="80%" width="80%" alt="Add Roles"/>
</p>
<br />
- <b>Select "Active Directory Domain Services"</b>
<br />
- <b>Finish Install, will require a reboot</b>
<p align="center">
<img src="InstallRoles.PNG" height="80%" width="80%" alt="Install Roles"/>
</p>



