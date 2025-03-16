
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites([https://www.youtube.com/watch?v=LOzmM5ZjKi0])

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enable INternet Infromation Services
- Install Web PLatform Installer
- Install My SQL
- Install C++
- Configure Permissions and Install osTicket

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/jZnQUuD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 1: Create a Windows 10 Azure Vitual Machine with 10 vCPU's, then login to that VM with Remote Desktop. Within the VM, download the osTicket-Installation-Files.zip and unzip it onto your desktop. The folder should be called “osTicket-Installation-Files”.

</p>
<br />

<p>
<img src="https://i.imgur.com/UrKtQWF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 2:*IN THIS ORDER* Install / Enable IIS in Windows WITH CGI. From the “osTicket-Installation-Files” folder, install PHP Manager for IIS, install the Rewrite Module, Create the directory C:\PHP, unzip PHP 7.3.8 into the “C:\PHP” folder, install VC_redist.x86.exe, and install MySQL then setup from there.


</p>
<br />

<p>
<img src="https://i.imgur.com/3IlT68w.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 3: Open IIS as an Admin
Register PHP from within IIS, Reload IIS , Install osTicket v1.15.8, Reload IIS again, Go to sites -> Default -> osTicket, Enable: php_imap.dll, php_intl.dll, php_opcache.dll. Refresh the osTicket site in your browser, observe the changes. Rename: ost-config.php, Assign Permissions: ost-config.php, Continue Setting up osTicket in the browser (click Continue).





</p>
<br />

<p>
<img src="https://i.imgur.com/Wdvegtd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 4: 
From the “osTicket-Installation-Files” folder, install HeidiSQL.
Open Heidi SQL
Create a new session, root/root
Connect to the session
Create a database called “osTicket”

Continue Setting up osTicket in the browser
MySQL Database: osTicket
MySQL Username: root
MySQL Password: root
Click “Install Now!”

</p>
<br />
