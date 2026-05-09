<h1>Promote Server to Domain Controller (VirtualBox Lab) </h2>
<br /> 
<h2>Overview:</h2> 
This lab demonstrates the process of promoting a Windows Server virtual machine to a Domain Controller using Active Directory Domain Services (AD DS). The environment is built and tested inside VirtualBox to simulate a real enterprise Active Directory setup.
<br />

<h2>Objective</h2>
<br />

- **Promote Windows Server VM to Domain Controller**
- **Create a new Active Directory forest and domain**
- **Install and configure AD DS role**
- **Configure DNS integration for domain services**
- **Verify successful domain controller deployment**
<br /> 

<h2>Environment:</h2>
- **Virtualization: VirtualBox**
- **Windows Server 2022**
- **Role Services: Active Directory Domain Services, DNS**
<br />

<h2>Lab Task 1:</h2>
<h3>VM Setup in Windows</h3>
- **Open VirtualBox**
- **Click New**
- **Set:**
    - Name: Windows Server 
    - Type: Microsoft Windows Server
    - Version: Windows 2022 (64-bit) (or 2019)
- **Allocate:**
    - RAM: 4–8 GB (recommended)
    - CPU: 2 cores minimum
- **Create virtual hard disk:**
    - Size: 60 GB+ (dynamic allocation)

# insert screenshot of vm creation in virtualbox 
<br />

<h2>Lab Task 2:</h2>
<h3>Install Windows Server</h3>
- **Attach Windows Server ISO to VM**
- **Boot VM**
- **Install:**
    - “Windows Server with Desktop Experience”
- **Complete installation and login as Administrator**

# insert screenshot of os install 
<br />


<h2>Lab Task 3:</h2>
<h3>Static IP Configuration </h3>

Inside Windows Server:
- **Open Network Settings**
- **Assign:**
    - IP Address: 192.168.10.10 (example)
    - Subnet: 255.255.255.0
    - Gateway: optional
    - DNS: point to itself (same as the IP)

</h2>

<h2>Lab Task 4:</h2>
<h3>Rename the Server</h3>
- **Open System Properties on Desktop**
- **Change computer name to**
    - DC1
- **Restart VM**


<h2>Lab Task 5:</h2>
<h3>Install Active Directory Domain Services (AD DS)</h3>

- **Open Server Manager**
- **Click Add Roles and Features**
- **Select:**
    - Role-based installation
- **Choose server**
- **Select:**
    - Active Directory Domain Services
- **Install and complete wizard**

<h2>Lab Task 6:</h2>
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

<h2>Lab Task 7:</h2>
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
