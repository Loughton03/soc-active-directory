<p align="center">

![image](https://github.com/Loughton03/soc-active-directory/assets/78968473/64f88fee-1609-404f-af0f-0506064577d4)

</p>

<h1>Azure Active Directory Overview (Users, Groups, and Access Management)</h1>
In this part, we will explore Azure Active Directory (AAD) and observe different access levels..<br />

<h2>What is Azure Active Directory?</h2>

- Azure Active Directory is a cloud based identity and access management service.

<h2>Actions and Observations</h2>

<p>
 Create a user in AAD named "globalreaderjohn" and use the auto-generated password.
</p>

<p>
<img src="https://i.imgur.com/1e4MhZW.png" height="80%" width="80%" alt="New User"/>
</p>

<p>
<img src="https://i.imgur.com/ZOtqZBn.png" height="80%" width="80%" alt="create new user"/>
</p>


<p>
Assign "Tenant-Level Global Reader" to the user.
</p>

<p>
<img src="https://i.imgur.com/PY27CLa.png" height="80%" width="80%" alt="asssign global reader"/>
</p>

<p>
Log in as "globalreaderjohn" in an incognito window and observe the access the pressioned granted as a "Global Reader."

Be sure to copy your user's "User Principal Name"

</p>

<p>
<img src="https://i.imgur.com/6jQMw6K.png" height="80%" width="80%" alt="account overview"/>
</p>

<h2>
<a href="http://portal.azure.com/">Login to Azure</a>
</h2>

<p>
<img src="https://i.imgur.com/SR1wUf3.png" height="80%" width="80%" alt="Azure Log-in"/>
</p>

<p>
 Azure will ask you to change the auto-generated password

 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now that we are connected, let us enable IIS (Internet Information Services ). ISS is a Microsoft web server that runs on the Windows operating system and is used to exchange static and dynamic web content with internet users. IIS can host, deploy, and manage web applications using technologies such as ASP.NET and PHP. 

Start Menu > Windows Feature > Internet Information Services > World Wide Web Services > Application Development Features > CGI.
</p>
<br />


<p>
<img src="https://i.imgur.com/YmpTa7K.png" height="80%" width="80%" alt="Internet Installation Services installation"/>
</p>
<p>
Now that we have this installed, let's download the installation files needed for osTicket and HeidiSQL.
</p>
<br />

<p>
<img src="https://i.imgur.com/n9NDKgB.png" height="80%" width="80%" alt="Internet Installation Services installation"/>
</p>
<p>
Now head to the installation folders.

•	From the Installation Files, download and install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi) 
•	From the Installation Files, download and install the Rewrite Module (rewrite_amd64_en-US.msi).

Create a directory C:\PHP.
</p>
<br />

<p>
<img src="https://i.imgur.com/BsYhvqG.png" height="80%" width="80%" alt="Create a PHP Folder in the C directory"/>
</p>
<p>
Download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) from the Installation Files and unzip the contents into C:\PHP 

•	From the Installation Files, download and install VC_redist.x86.exe. 
•	From the Installation Files, download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi). 

Next, download osTicket, and extract the content to the folder c:\inetpub\wwwroot. Rename the folder "Upload" to "osTicket."
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS Manager as an Admin, Register the PHP using the PHP folder.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In IIS Manager, open PHP Manager. We need to enable three extensions named php_imap.dll, php_intl.dll, php_opcache.dll Now reload IIS manager and make your way to "Sites > Default > osTickets. Click " Browse *:80" on the right to open the osTicket web interface.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
It should look like this.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Perfect. Now let's return to c:\inetpub\wwwroot\osticket\include. Look for the file named "ost-sampleconfig.php" We will rename it to "ost-config.php." Once completed, right-click the file, and open properties, under the security tab, "Disable Inheritance." Then Remove all new permissions, and give everyone permissions.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
HeidiSQL From the Installation Files, download and install HeidiSQL.

 •	Open Heidi SQL 
•	Create a new session, root/Password1 
•	Connect to the session 
•	Create a database called "osTicket" 

Let's return to osTicket in the web interface. Name the Helpdesk and remember your login credentials. 

##Continue Setting up osticket in the browser 

•	MySQL Database: osTicket 
•	MySQL Username: root 
•	MySQL Password: Password1 
•	Click "Install Now!"
</p>
<p>
<img src="https://i.imgur.com/cPxyIZe.png" height="80%" width="80%" alt="osTicket Installer"/>
</p>

<p>
<img src="https://i.imgur.com/TGmrZnu.png" alt="osTicket Installer Complete"/>
</p>
<br />

<p>
osTicket should be up and running with no issues. We will now move on the Post Installation Config.
</p>
<br />

