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
Search the internet for the installation files you will need to insatll. Find and install Web Platform Installer: open Web Platform Installer and search to add "MySQL 5.5" & search to add all simple versions of PHP (x86) up until 7.3. Create username and password when asked to finish installation. Web installer will attempt to finish installing all of the prerequistes that are checked (some of the downloads will fail, just manually download C++ redis & PHP Manager via files found online). Continue to finish with installation. Find and install PHP Manager version 7.3.8 & version 1.5.0. 
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
<img src="https://imgur.com/AKPxXsc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After IIS restart, click on "OsTicket" within IIS under "Default Website" and lastly, click "Browse*:80" on the right hand side of the menu. 
</p>
<br />

<p>
<img src="https://imgur.com/OdzWcn5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
If you have installed all prerequisites and followed all steps up to this point correctly, then you should the OS Ticketing system open in the browser*:80 port when clicked. 
</p>
<br />

<p>
<img src="https://imgur.com/kjIMvoQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/Yw6c5gd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click the "PHP Manager" option in ISS. If the option does not show then restart ISS. Next, click "Enable or disable an extension" option at the bottom. On the next window enable the following extensins: "php_imap.dll, php_intl.dll, php_opcahe.dll" and refresh OsTicket in the browser window.
</p>
<br />

<p>
<img src="https://imgur.com/e0Qis8c.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/INrk5kt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Rename C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php to C:\inetpub\wwwroot\osTicket\include\ost-config.php. Assign permissions: under security tab security click advanced, click disable inheritance: remove all inheritance. Next allow all permisions, on the same screen click "add", select a "principal", enter "everyone" in object name field, lastly allow full control permissions. This will allow full control for everyone. 
</p>
<br />

<p>
<img src="https://imgur.com/4SxPW2u.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After all previous steps are complete, the OsTicketing system should be fully functional and you should be allowed to continue forward to start being able to create acual helpdesk tickets. Please see test ticket above. You have to fill out most, if not all, of the information for this setup. The email addresses must be different for the system settings and the admin user to not create conflict. 
</p>
<br />

<p>
<img src="https://imgur.com/iecoXP0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install a program called HeidiSQl (can be searched online) that OsTicketing System uses to connect with Databases. Then you must create a new database to be used with the new ticketing setup titled "OsTicket". Now, finish filling out the information in the OsTicket browser (MySQL will be the new database's name) and use the same user name and passwork from throughout the lab. 
</p>
<br />

<p>
<img src="https://imgur.com/Dm38qAa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
You should see a congratulations screen in the browser window if everything was done correctly. Clients are now able to successfully create help desk tickets. That concludes the lab. Once again, thank you very much for viewing! 
</p>
<br />
