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

- Enable IIS (Internet Information Server) with CGI 
- Install PHP Manager for IIS
- Install a few separate programs from the installation files
- Create a folder for the PHP files directly into the C drive.
- Configure Settings in My SQL
- Install OSticket

<h2>Installation Steps</h2>

<p>


</p>
<p>
-On a Windows computer, Click Start and go to the Control Panel>Programs & Features> Turn Windows Features on or off
 From the list, enable "Internet Information Services" Next, expand that section, then expand "World Wide Web Services"> 'Application Development Features" and enable CGI


-Next, install PHP manager from the download files of osticket opensource. Go throught the installation steps as the installation wizard prompts

-Install the Rewrite Module

-Create a directory in the C drive named "C:/PHP"

-From the installation files, unzip php-7.3.8-nts-Win32-VC15-x86.zip directly into the folder C:/PHP that was recently created

- Next, install VC_redist.x86.exe

- Next install My SQL. (Use standard configuation when prompted)

- Open IIS as an admin and register PHP by going to PHP Manager>C:\PHP\php-cgi.exe

- Be sure to start and stop the server to ensure the server recognizes these settings by clicking these buttons on the right side of the screen

- From the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip” and copy the “upload” folder into “c:\inetpub\wwwroot”
Within “c:\inetpub\wwwroot”, Rename “upload” to “osTicket” ***This step is very important as you will run into error if this file is named incorrectly. This is case-sensitive.

- Again, start and stop the server
  
- Navigate to IIS and go to the Sites section. Locate the Default site and select osTicket.

-Next, open PHP Manager by double-clicking on it. Within PHP Manager, find the option to enable or disable an extension and select it. Then, enable the following extensions: php_imap.dll, php_intl.dll, and php_opcache.dll. Once you've made these changes, refresh the osTicket site in your browser to observe the effects.

-Now, you need to rename the configuration file for osTicket. Locate the file ost-sampleconfig.php in C:\inetpub\wwwroot\osTicket\include\ and rename it to ost-config.php.

-After renaming the file, update its permissions. Disable inheritance, remove all existing permissions, and then assign new permissions to Everyone, granting full access.

-Continue with the osTicket setup in the browser by clicking Continue. At this stage, name your helpdesk and provide a default email address that will receive emails from customers.

-Next, install HeidiSQL from the “osTicket-Installation-Files” folder. Open HeidiSQL and create a new session using the credentials root/root. After successfully connecting to the session, create a new database named osTicket.

-Finally, return to the osTicket browser setup. Enter the database information: MySQL Database: osTicket, MySQL Username: root, and MySQL Password: root. Click Install Now! to complete the installation process.
  



</p>
<br />

<p>

</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
