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
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To create a resource group in Windows Azure, click the Resources Groups icon, name the group "RG", place it in WST 3, and crate the group, then name the virtual machine "VM".
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To log in to Microsoft Remote Desktop, add the VM's IP address and navigate to the control panel. Change settings, click on programs, and enable CGI and HTTP common features.
</p>
<br />

<p>
<img> [Uploading Untitled 2.pdf…]

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
