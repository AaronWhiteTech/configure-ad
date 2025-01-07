# configure-ad

<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>
https://youtu.be/XbnsOEeY2PA
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
- (Step 1)Install Sever 2022(Server) and Windows 10(client)
-Configure Network Settings (Make sure client server are on the ame vnet, make server IP static, and configure The Client DNS to match the Server IP, Test connection)





![ad installed](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/792b8791-f1c7-455d-991f-c64c35429ace)



- (step 2) Install Active Directory Domain Services go to tools-roles and features, add roles and features, choose active directory domain services, new forrest, create domain and password, hit next until finish
  Click the caution sign and install, after the computer restarts ad will show in the server window


Part 2

[user admin config](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/e9d44fcf-dc04-4009-a94d-bbd14d3262bd)

-(Step 3) Configure administrator account "Jane Doe" go to active directory users and computers, ccreate new user, go to properties-security, then join the user to domain administrators




![alternate account logged in on client](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/bdd2d59a-78b3-45fe-9c30-86d48ed465e8)

- (Step 4)Log into client as created admin "Jane Doe" Log into the client machine with the user "aaron.com/janedoe"




![connect client to domain](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/0c46cc4f-deaa-4b9a-9503-6f05232bec5f)

-(Step 5) Connect client to Domain, go to pc-properties-rename this computer advanced, change domain, type in "aaron.com, a welcome to aaron.com pop up appears






![creating users i AD 1000](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/e0275595-1580-43a7-a3b3-e835c730754f)

-(Step 6)  Go to server and open powershell ISE as admin to create multiple users










   ![Log in with created user ](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/1ea0e335-a9bb-4195-a47a-1cdfbfc50fd0)


(Step 7)Log into client as created user "tvp.bul" to prove mas user creation successful log into client machine with user name "aaron.com/tvp.bul"

