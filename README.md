# configure-ad

<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>
Part 1
- Install Sever 2022(Server) and Windows 10(client)
-Configure Network Settings (Make sure client server are on the ame vnet, make server IP static, and configure The Client DNS to match the Server IP, Test connection)

- Install Active Directory Domain Services
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Part 2
- Configure administrator account
- <img src="![user admin config](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/e9d44fcf-dc04-4009-a94d-bbd14d3262bd)
" alt="Disk Sanitization Steps"/>
- Log into client as created admin
- <img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
- Connect client to Domain
- <img src="![Screenshot 2024-06-28 193624](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/c9ac231a-2118-43e2-951e-491e3f94f6a6)
" alt="Disk Sanitization Steps"/>
-  Go to server and open powershell ISE as admin
-   to create multiple users
-   <img src="![Screenshot 2024-06-28 220203](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/01522db1-a3ba-49f4-99f7-effcac95c444)
" width="80%" alt="Disk Sanitization Steps"/>
<img src="![users created in ad](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/17e96434-bd7d-42a4-ae39-d2e99e039373)
" alt="Disk Sanitization Steps"/>
- Log into client as created user
<img src="![Log in with created user ](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/5d64b378-03ec-4e8d-8f9e-5e0debeec44f)
" alt="Disk Sanitization Steps"/>

