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
Preequisites
- (Step 1)Install Sever 2022(Server) and Windows 10(client)




![ad installed](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/792b8791-f1c7-455d-991f-c64c35429ace)
After installing Active Directory Domain Services, Configure the ip adrssing by going the newtok sharing center in the windows settings
Configure  IPV4 manually on Server 2022, configure ipv4 on windows 10, make sure the ip adress on windows 10 is the same as the dns on Server 2022
Ping the client to the server and vice versa to make sure a connection is established, you may need to disable firewall
![configure client dns to as server ip](https://github.com/user-attachments/assets/3cc745cb-e695-4b12-8b22-6a64a8e7204d)

After establishing a connection, on the client, go to file explorer, click this pc 
![joined to domain](https://github.com/user-attachments/assets/774b65ad-e732-42fe-a8e7-9d66a068b7f2)

- (step 2) Install Active Directory Domain Services go to tools-roles and features, add roles and features, choose active directory domain services, new forrest, create domain and password, hit next until finish
  Click the caution sign and install, after the computer restarts ad will show in the server window, click properties click renmae thois pc(advanced
  

Part 2
After connecting client go the the server menu in server 2022 go to tools select users and computers, right click click new, select user, and create a user (Karen M)



![ad user creation screenshot 1](https://github.com/user-attachments/assets/90464548-e230-4bb3-812b-45180b9ca0db)
![Share out (HR)](https://github.com/user-attachments/assets/3264208d-6adf-42fd-a47c-06a5e622cc6f)
![file security (HR)](https://github.com/user-attachments/assets/a057d82d-3c4f-4327-9606-173f3b9cb455)

![screenshot of ad network filwsharing](https://github.com/user-attachments/assets/5f44aa8a-1eb8-4d07-a50e-b19afae91284)

