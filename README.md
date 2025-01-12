# configure-ad

<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h2>Video Demonstration</h2>


Configuration- https://youtu.be/XbnsOEeY2PA



User Creation and Network File Share- https://youtu.be/Xr1UQ-xrPlE


Objective: Conduct Overview of Active Directroy administrative responsibilites simulating live environemnt


Preequisites : 
 Download Iso File from Microsoft
 Configure VMwae

 Configuration Steps
 Create Accounts For Windows 10 and Server 2022 

 Configure IPv4 settings on Both Virtual Machines

<h1>On-premises Active Directory Deployed On Vmware


<h2>Environments and Technologies Used</h2>
-VMWare
- Active Directory Domain Services


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



![ad user creation screenshot 1](https://github.com/user-attachments/assets/90464548-e230-4bb3-812b-45180b9ca0db)
