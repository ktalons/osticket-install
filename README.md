<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

## osTicket - Prerequisites and Installation ##
> This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.
- ⚠️ ost-config.php permission settings only used for demonstration purposes ⚠️
- ⚠️ SQL database root login credentials only used for demonstration purposes ⚠️
<br />

<h2>Video Demonstration</h2>

- ### [<img src="https://img.icons8.com/?size=100&id=19318&format=png&color=000000" align="center" width="40" height="40">](https://www.youtube.com/channel/UC9YvuJxKB94ByhwCfZQ_5Kg) [How To Install osTicket](https://youtu.be/_0zx2qOCJ9k)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10

<h2>List of Prerequisites</h2>

- Create an Azure Virtual Machine Windows 10 - 4 vCPUs 
- Install / Enable IIS in Windows with CGI
  > Windows Features -> IIS -> World Wide Web Service -> Application Development Features -> check CGI box.  
- Install PHP Manager / IIS URL Rewrite Module
- Create PHP directory and unzip PHP package into directory
- Install Microsoft Visual C++ Redistributable
- Install / Configure MySQL
- Open IIS as Admin
- Register PHP within IIS
  > PHP Manager -> C:\PHP\php-cgi.exe


<h2>Installation Steps</h2>

<img src="https://github.com/user-attachments/assets/f77bff26-45dd-4c25-82c4-5528a94464b5"/> <br />

1️⃣ Install osTicket ⤵️
> 1. Unzip osTicket-v1.15.8.zip.
> 2. Copy __upload__ folder into __c:\inetpub\wwwroot__. Within __c:\inetpub\wwwroot__ rename __upload__ folder to __osTicket__. <br />
> 3. Reload IIS. Go to sites -> Default -> osTicket -> click Browse *:80".
> 4. Enable extensions within PHP Manager.
> 5. Rename ost-config.php and assign permissions.
> 6. Continue configuration of osTicket in browser.
---
<img src="https://github.com/user-attachments/assets/60676b0c-d786-424d-815b-fa30ebc9f980"/> <br />

2️⃣ Install HeidiSQL ⤵️
> 1. Open HeidiSQL. Create a new session. Connect to the session. Create a database called **osTicket**.
> 2. Continue configuration of osTicket in browser.
> 3. Click Install Now.
---
<img src="https://github.com/user-attachments/assets/87353174-dba7-44ff-8bb1-ffee16e240c6"/> <br />

3️⃣ Login osTicket and Cleanup 🏁
> 1. Browse to help desk login URL
> 2. Browse to end user URL
> 3. Optional Cleanup. Delete: C:\inetpub\wwwroot\osTicket\setup
---
