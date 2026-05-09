<h1>Promote Server to Domain Controller (VirtualBox Lab) </h2>
<br /> 
<h2>Objective:</h2> 
This lab demonstrates the process of promoting a Windows Server virtual machine to a Domain Controller using Active Directory Domain Services (AD DS). The environment is built and tested inside VirtualBox to simulate a real enterprise Active Directory setup.

<h2>Lab Task 1:</h2>
<h3>Install Active Directory Domain Services (AD DS)</h3>

- **Open Server Manager**
- **Click Add Roles and Features**
- **Select:**
    - Role-based installation
- **Choose server**
- **Select:**
    - Active Directory Domain Services
- **Install and complete wizard**

<h2>Lab Task 2:</h2>
<h3>Promote Server to Domain Controller</h3>

After installation:
<br /> 
- **Click Promote this server to a domain controller**
- **Select:**
    - Add a new forest
- **Enter domain name**
    - Example: corp.local 
- **Set DSRM**
- **Leave DNS option checked**
- **Continue through prerequisites check**
- **Click Install**

VM will reboot automatically 

<h2>Lab Task 3:</h2>
<h3>Verify Domain Controller Setup</h3>

After reboot: 
<br /> 
- **Log in using domain**
    - CORP\Administrator:
    - Password ( Set up in Lab Task 2 ) 
- **Open Tools**
    - Active Directory
    - DNS Manager
- **Confirm**
    - Domain exists 
    - DNS zone created
