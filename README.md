<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Installation Files https://drive.google.com/drive/u/1/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/ADUIJNc.png" width="80%" alt="Searching for VM"/>
</p>
<p>
Look up Vitural Machines and click on the result.  
</p>
<br />

<p>
<img src="https://i.imgur.com/vb5bYkr.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Since we havent created the resouce group for the VM yet, we will let it create one for us. Memorize or (not the best pratice but its only for this )write down the username and password. We will choose a windows OS , with 4vpc(so you can run the VM quicker)  leave the default setttings for the Network, Disk and create the VM.
</p>
<br />

<p>
<img src="https://i.imgur.com/nhLMOla.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Remote in to the VM via remote desktop connection with the VM's public adress as shown above. And enter the user and password when prompted. </p>
<br />

<p>
<img src="https://i.imgur.com/CbbxR07.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once in the VM, go to control panel>"uninstall a program"> "turn windows fetures on or off">Highlight Internet Information Services>"OK". This creates a webserrver on the VM which be used to server osTiket.
</p>
<br />

<p>
<img src="https://i.imgur.com/T3ijOTG.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install Web Platform Installer download from the "Installation Files" above.

Open WPI and Add MySQL 5.5 and all simple versions of x86 PHP up until 7.3 but not 7.4

Click Intsall.

Name: root

Password: Password1(can be whatever but be sure to remember or write it down).
    
A screen similar to the one above might appear in which download the things needed so I would download the PHP manger and Microscof Visuall C++(ignore the php5.3.28).Find the links in Insallation Files. And might as well download osticket while you are there.
</p>
<br />


<p>
<img src="https://i.imgur.com/M8aNb0r.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open File Exopler go to downloads and "extract all" the osticket Folder.
    
Open the extracted osTicket folder .
    
Extract and copy the “upload” folder INTO c:\inetpub\wwwroot.
    
Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”
</p>
<br />


<p>
<img src="https://i.imgur.com/YbinGos.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/NL0ZEl1.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Restart IIS as shown above.
    
Go to sites > Default > osTicket

On the right tab, click “Browse *:80”
    
And a similar page should open up in the browser as shown below.
</p>
<br />
<p>
<img src="https://i.imgur.com/kFyMmkE.png" width="80%" alt="Disk Sanitization Steps"/>
============================================================================================


<img src="https://i.imgur.com/WkXDPsw.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go back to IIS, sites > Default > osTicket
    
Double-click PHP Manager
    
Click “Enable or disable an extension”
    
Enable: php_imap.dll , php_intl.dll , php_opcache.dll

Refreash the page and changes above should be seen.
</p>
<br />


<p>
<img src="https://i.imgur.com/YEATvTz.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Change C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php to "ost-config.php"
</p>
<br />


<p>
<img src="https://i.imgur.com/snv80yb.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Assigning Permissions: ost-config.php
    
ost-config.php>right click>properties>security> 

Disable inheritance > Remove All
    
New Permissions > Everyone > Full access
</p>
<br />


<p>
<img src="https://i.imgur.com/KnXMxq6.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go back to the page and you will similar page as show above. Just fill the emails as you like. The important part is the username and password for the admin.Remember them or write it down for now.
</p>
<br />

<p>
<img src="https://i.imgur.com/O0tNcUA.png" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/jfphMDu.png" width="80%" alt="Disk Sanitization Steps"/> 
</p>
<p>
    
Download and Install HeidiSQL (from the installation files)

Rember the MySQL database we made at the start. Well HeidiSQL is a client that allows us to connect to that database
    
Create a new session, root/Password1 which is the credentails we made for the SQL at the start.

Connect to the session and create a database called “osTicket” by right clicking on "unnamed">create new.
</p>
<br />


<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />


<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />


<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />


<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />

<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />


<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />


<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />


<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />


<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />


<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />


<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />

<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />

<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />


<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />


<p>
<img src="" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start here bozo
</p>
<br />

