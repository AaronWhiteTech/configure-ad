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


<H13>Configuration (Part 1)</h13>

![ad installed](https://github.com/AaronWhiteTech/configure-ad/assets/155200818/792b8791-f1c7-455d-991f-c64c35429ace)


<h4>Step 1</h4>
After installing Active Directory Domain Services, Configure the ip adrssing by going the newtok sharing center in the windows settings
Configure  IPV4 manually on Server 2022, configure ipv4 on windows 10, make sure the ip adress on windows 10 is the same as the dns on Server 2022
Ping the client to the server and vice versa to make sure a connection is established, you may need to disable firewall

![configure client dns to as server ip](https://github.com/user-attachments/assets/3cc745cb-e695-4b12-8b22-6a64a8e7204d)

<h11>Step 2 </h11>After establishing a connection, on the client, go to file explorer, click this pc, click reneame this pc(advanced) and type the domain of the server, Then type the administrator username and password, and you will be connected to the domain
![joined to domain](https://github.com/user-attachments/assets/774b65ad-e732-42fe-a8e7-9d66a068b7f2)

<h5>Step 3</h5>
Install Active Directory Domain Services go to tools-roles and features, add roles and features, choose active directory domain services, new forrest, create domain and password, hit next until finish
  Click the caution sign and install, after the computer restarts ad will show in the server window, click properties click rename this pc(advanced), Click change this computer's domain or workgroup
  

<h6>User Creation/Network Fileshare (Part 2)</h6>


<h7>Setp 1
</h7> After connecting client go the the server menu in server 2022 go to tools select users and computers, right click click new, select user, and create a user (Karen M) making a user name and password



![ad user creation screenshot 1](https://github.com/user-attachments/assets/90464548-e230-4bb3-812b-45180b9ca0db)

<h8>Step 2</h8> 
After creating the user i create the File and folder For (HR) i share out the file and folder by right clicking
going to properties, the share tab and click share
![Share out (HR)](https://github.com/user-attachments/assets/3264208d-6adf-42fd-a47c-06a5e622cc6f)

<h9>Step 3</h9>
Here I configure the security setting for the file making it that only those in the hr security group and administrators will have access to the HR file
![file security (HR)](https://github.com/user-attachments/assets/a057d82d-3c4f-4327-9606-173f3b9cb455)
<h10>Step 10</h10>
Next I will log into the client VM As Karen M go to file explorer type in the network path for the shared file 
and I am able to access the file due to me being signed in as a user who is within the security group "HR"
![screenshot of ad network filwsharing](https://github.com/user-attachments/assets/5f44aa8a-1eb8-4d07-a50e-b19afae91284)

