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

-  Crate resoures group and virual machines
-  Open VM and configure IIS 
-  configure and ajdust protories of php
-  OSTicket installion and configure


<h2>Installation Steps</h2>

<p>
<img !
<img width="1340" alt="Screenshot 2024-09-02 at 8 21 26 PM" src="https://github.com/user-attachments/assets/052d05f5-a8b7-49af-a428-3edcea94410a">



</p>
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

tTo open OSTicket, return to PHP. On the left-hand side, click the drop-down bar label OSTicket, then open Bowers 80*. Afterwares login with your selected username and password. which will allow you access to an admission page on OSTicket.
