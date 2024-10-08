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
<img width="711" alt="Screenshot 2024-09-03 at 9 43 35 PM" src="https://github.com/user-attachments/assets/193e82b5-6775-4dbf-b6d3-9776c4bf8991">

<br />
4) Once PC is connected, open the control panel. form control panel open programs to get to programs and features. Look for the run window features on and off.

You will want to install / enable IIS in Windows with CGI and Common HTTP Features

World Wide Web Services -> Application Development Features -> [X] CGI [X] Common HTTP Features
<p>
<img <img width="1470" alt="Screenshot 2024-09-03 at 8 05 26 PM copy" src="https://github.com/user-attachments/assets/c487e81a-407c-418d-b086-347443a5a9d5">

</p>* To ensure IIS is enabled, open the internet browser and enter 127.0.0.1. You should get this page. 
<p> copy and paste https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6 into your browser 

</p>5) Crate a floder in c: and name it PHP.

</P>6) Download PHP 7.3.8 and unzip the contents into C:\PHP. Exact the fold when finished downloading 


<img width="1252" alt="Screenshot 2024-09-04 at 6 33 21 PM" src="https://github.com/user-attachments/assets/ae27d156-2055-4922-b792-dc5a58b4219d">

</p>7) Open IIS as an Admin,
<img width="1470" alt="Screenshot 2024-09-03 at 8 02 52 PM 2" src="https://github.com/user-attachments/assets/0494c697-8b89-4e2b-be92-cda3c1201be8">

</p>8)register PHP from within IIS.uthe the PHP folder you crated as the file to load after reload the the sever

<img width="1252" alt="Screenshot 2024-09-04 at 7 22 29 PM" src="https://github.com/user-attachments/assets/4da0b8ef-aa2d-4751-8b30-5455f48cbbed">

</p>9) Install VC_redist.x86.exe and MySQL 5.5.62.
   
<img width="1252" alt="Screenshot 2024-09-04 at 6 42 13 PM" src="https://github.com/user-attachments/assets/cb61191c-5e29-4e15-be53-ed16fed646f4">

<img width="1208" alt="Screenshot 2024-09-04 at 6 49 01 PM" src="https://github.com/user-attachments/assets/3eaf6d3f-cfb4-47c5-8f49-76b6276636de">

</p>10)Download php-7.3.8-nts-Win32-VC15-x86.zip once it have has finshed Extract copy the upload folder to c:\inetpub\wwwroot -Within c:\inetpub\root, Rename "upload" to "osTicket" 
reload IIS

</p>11)on IIS go to site click on site and go down to OSTick on the right side the screen look for “Browse *:80” and open it 

<img width="1470" alt="Screenshot 2024-09-03 at 8 02 52 PM" src="https://github.com/user-attachments/assets/1b9530a6-21a6-4f2b-8c6d-5a45320a4a4f">

</p> some extions will not be enable on OSTicket browser
<img width="1710" alt="Screenshot 2024-09-04 at 7 21 12 PM" src="https://github.com/user-attachments/assets/c332cfb5-6a05-4071-92ce-7fffc4a3ac3d">

</P>12)Return to IIS sites to PHP manager. Click "Enable or disable an extension." Enable or disable extensions.

You want to enable PHP_imap.dll, PHP_intl.dll, and PHP_opcache.dll.

<img width="1252" alt="Screenshot 2024-09-04 at 7 22 29 PM" src="https://github.com/user-attachments/assets/1ab6476e-2561-4d21-95ef-591b65530993">

</p>13) Once you have enabled the extensions, return to your inetpub folder to rename C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php. You will rename ost-sampleconfig.php to ost-config.php.

<img width="1252" alt="Screenshot 2024-09-04 at 7 05 51 PM" src="https://github.com/user-attachments/assets/b895d171-becf-4c7a-8025-a0f5f31e4b58">

</P>14)Now that we have renamed the files, right click on the file and go to properties. From there click security, click on advance, and disable the inheritance. We will select Remove all inherited permissions from this object.

<img width="1252" alt="Screenshot 2024-09-04 at 7 25 54 PM" src="https://github.com/user-attachments/assets/6b09fe9d-5042-4920-81c6-97aa648ca9b6">

to send new permissions 

Click added, at the top, select a principal, type everyone in the box, check the box labeled full control, click okay, and apply. 

</p>14) Download and install HeidiSQL from the Installation Files. 

<img width="1252" alt="Screenshot 2024-09-04 at 7 28 07 PM" src="https://github.com/user-attachments/assets/aa9cc003-b940-4b32-998c-79aed4f7d0e7">

Download and install HeidiSQL from the installation files. Create a new session. Your username will be root, and the password is password1.

<img width="1208" alt="Screenshot 2024-09-04 at 7 35 55 PM" src="https://github.com/user-attachments/assets/e67bceeb-17ca-4722-9da8-b9ed196d6d0a">

</p>15)create a new database within HeidiSQL. In Heidi right click on the left side where is says "Unnamed", select "create new", and then select "database". Name the new database osTicket. Once we have the new database setup go back to the osTicket browser and under MySQL Database type in osTicket.
</p> You will want to delete the setup folder in our system. -Delete: C:\inetpub\wwwroot\osTicket\setup Only delete the setup folder and nothing else.

We then will want to set the permissions back to "Read" only in the ost-config.php file.

</p>16)Login to osticket on the browser

<img width="1252" alt="Screenshot 2024-09-04 at 7 39 40 PM" src="https://github.com/user-attachments/assets/f8ca2440-dc6a-4b8f-9bd0-416ee83e8c56">




