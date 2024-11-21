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

- An active Azure account with permissions to create resources.
- A Windows Virtual Machine (VM) deployed in Azure.
- Remote Desktop Connection (RDC) enabled to access the VM.
- Installed software:
     - IIS (Internet Information Services)
     - PHP (Version 8.1 or 8.2)
     - MySQL (Version 8.0 or higher)
- Firewall rules allowing HTTP (port 80) and HTTPS (port 443).

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To install osTicket, begin by setting up your server environment. If you're using Microsoft Azure, create a Windows Virtual Machine (VM) with sufficient resources (e.g., 2 vCPUs, 8 GB RAM, and 128 GB SSD storage) and ensure it runs Windows 10 or a compatible server OS. Enable Remote Desktop Protocol (RDP) to connect to the VM and configure firewall rules to allow HTTP (port 80) and HTTPS (port 443) traffic. Once connected to the VM, install Internet Information Services (IIS) via the Control Panel and enable essential features like CGI and URL Rewrite. This forms the foundation for hosting the osTicket application.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, install PHP and MySQL, which are required to run osTicket. Download PHP (version 8.1 or 8.2) and extract it to a directory like C:\PHP. Configure the php.ini file to enable necessary extensions, such as mysqli, pdo_mysql, gd, and mbstring, and add PHP to the system PATH for global accessibility. Install MySQL Community Server, create a database named osticket, and set up a user with full privileges to manage it. Ensure both PHP and MySQL are properly configured and working by testing them with basic scripts or connection checks.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finally, download osTicket from its official site and extract the files into the IIS web root directory (e.g., C:\inetpub\wwwroot\osTicket). Navigate to http://<your-vm-ip>/osTicket/setup in your browser to begin the web-based installer. During the setup, provide database credentials, set up an admin account, and configure basic settings. After installation, remove or secure the setup/ directory as per the instructions, log in to the admin panel, and customize osTicket by defining departments, adding agents, and configuring email notifications. Your osTicket helpdesk system is now ready to use!
</p>
<br />
