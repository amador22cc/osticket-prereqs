<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

-  Windowd Azuer
-  Micrsoft Remmote Desktop
-  PHP Manger
-  VC Redist
-  MySQL
-  Heidi SQL
-  osTicket
-  Download links https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6

-  
<h2>Installation Steps</h2>
1)Open Windows Azure and create a virtual machine that we will set up with Windows 10 Pro, 22H2. with DS1 v2 with 16 GB of memory.
2)Once your virtual machine has been created, locate the pulbic IP address and copy it. 
<p>
<img width="1710" alt="Screenshot 2024-09-03 at 9 43 16 PM" src="https://github.com/user-attachments/assets/d4c3a101-24d2-4066-9001-abb1689ab8c8">

</p>3) Open Microsoft Remote Desktop and add a PC. Copy the IP address from your virtual machine. and login with your username and password.
<p>
To create a resource group in Windows Azure, click the Resources Groups icon, name the group "RG", place it in WST 3, and crate the group, then name the virtual machine "VM".
</p>
<br />

<p>
<img <img width="1470" alt="Screenshot 2024-09-03 at 8 05 26 PM copy" src="https://github.com/user-attachments/assets/c487e81a-407c-418d-b086-347443a5a9d5">

</p>
<p>
To log in to Microsoft Remote Desktop, add the VM's IP address and navigate to the control panel. Change settings, click on programs, and enable CGI and HTTP common features.
</p>
<br />
<img width="1470" alt="Screenshot 2024-09-03 at 8 02 52 PM 2" src="https://github.com/user-attachments/assets/0494c697-8b89-4e2b-be92-cda3c1201be8">


To install IIS in Windows, follow these steps:

1. Download and install PHP Manager for IIS, Rewrite Module, and C:\PHP.
2. Download PHP 7.3.8 and unzip the contents into C:\PHP.
3. Install VC_redist.x86.exe and MySQL 5.5.62.
4. Open IIS as an Admin, register PHP from within IIS, and reload the server.
5. Install osTicket v1.15.8 and reload IIS.
6. Enable or disable extensions like php_imap.dll, php_intl.dll, and php_opcache.dll.
7. Refresh the osTicket site and assign permissions.
8. Set up osTicket in the browser and name the helpdesk.
9. Download and install HeidiSQL and create a new session.
10. Install osTicket in the browser.
</p>
<br />
<img 

To open OSTicket, return to PHP. On the left-hand side, click the drop-down bar label OSTicket, then open Bowers 80*. Afterwares login with your selected username and password. which will allow you access to an admission page on OSTicket.
