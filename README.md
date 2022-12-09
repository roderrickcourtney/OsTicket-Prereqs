<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket through an Azure VM. The installation instructions written in this guide came directly from OsTicket. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used</h2>

- Windows 10 (21H2)

<h2>List of Prerequisites</h2>

- Internet Information Services (IIS)
- Microsoft Web Platform Installer
- PHP Manager
- My SQL
- C++ 2008 Redistributable

<h2>Installation Steps</h2>

<p>
<img src="https://imgur.com/qXWOfvq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/egJMdgS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a Virtual Machine with Azure to run this lab. Remote Desktop into the created VM. 
</p>
<br />

<p>
<img src="https://imgur.com/n9ibcLa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install/Enable Internet Information Services in windows. This is done by going to "control panel","programs", "Turn Windows features on or off", lastly check box titled "Internet Information Services".  IIS is a windows server in which OsTicket requires to be enabled in order to run properly, even though OsTicket runs through the web browser.
</p>
<br />

<p>
<img src="https://imgur.com/YBPThz1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/OjPupsw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Search the internet for the installation files you will need to insatll. Find and install Web Platform Installer: open Web Platform Installer and search to add "MySQL 5.5" & search to add all simple versions of PHP (x86) up until 7.3. Create username and password when asked to finish installation. Web installer will attempt to finish installing all of the prerequistes that are checked. Continue to finish with installation. Find and install PHP Manager version 7.3.8 & version 1.5.0. 
</p>
<br />

<p>
<img src="https://imgur.com/t2OkA7p.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Search the internet for "osTicket-v1.15.8" and download it. Next, copy the upload folder from inside the OsTicket installation files to c:\inetpub\wwwroot. Within c:\inetput\wwwroot folder, rename "upload" folder to "OsTicket". Open ISS, click "osTicket", next click Browse*80 then restart ISS
</p>
<br />

<p>
<img src="https://imgur.com/KL5FPaL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Search and open IIS program via windows search bar. Next, restart IIS server client for changes to take effect.  
</p>
<br />

<p>
<img src="https://imgur.com/zWbAuXn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Search the internet for the installation files you will need to insatll. Find and install Web Platform Installer: Add SQL & All PHP (x86) versions during install up until 7.3, Find and install OsTicket. 
</p>
<br />

<p>
<img src="https://imgur.com/zWbAuXn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Search the internet for the installation files you will need to insatll. Find and install Web Platform Installer: Add SQL & All PHP (x86) versions during install up until 7.3, Find and install OsTicket. 
</p>
<br />

<p>
<img src="https://imgur.com/zWbAuXn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Search the internet for the installation files you will need to insatll. Find and install Web Platform Installer: Add SQL & All PHP (x86) versions during install up until 7.3, Find and install OsTicket. 
</p>
<br />

<p>
<img src="https://imgur.com/zWbAuXn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Search the internet for the installation files you will need to insatll. Find and install Web Platform Installer: Add SQL & All PHP (x86) versions during install up until 7.3, Find and install OsTicket. 
</p>
<br />

<p>
<img src="https://imgur.com/zWbAuXn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Search the internet for the installation files you will need to insatll. Find and install Web Platform Installer: Add SQL & All PHP (x86) versions during install up until 7.3, Find and install OsTicket. 
</p>
<br />
