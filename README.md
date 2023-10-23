<!-- osTicket Logo -->
<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<!-- Heading -->
<h1 align="center">osTicket - Prerequisites and Installation</h1>
<p>This tutorial provides a comprehensive guide to the prerequisites and installation process of osTicket, an open-source help desk ticketing system.</p>

<!-- Environments and Technologies Used -->
<h2 align="center">Environments and Technologies Used</h2>

<ul align="center">
  <li>Microsoft Azure (Virtual Machines/Compute)</li>
  <li>Remote Desktop</li>
  <li>Internet Information Services (IIS)</li>
</ul>

<!-- Operating Systems Used -->
<h2 align="center">Operating Systems Used</h2>

<p align="center"><b>Windows 10 (22H2)</b></p>

<!-- List of Prerequisites -->
<h2>List of Prerequisites</h2>

<ul>
  <li>Azure Virtual Machine</li>
  <li>Internet Information Services (IIS)</li>
  <li>PHP Manager</li>
  <li>Rewrite Module</li>
  <li>VC Redist</li>
  <li>MySQL</li>
  <li>Heidi SQL</li>
  <li>osTicket v1.15.8</li>
</ul>

<p>Link to downloads: [osTicket Downloads](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)</p>

<!-- Installation Steps -->
<h2>Installation Steps</h2>

<ol>
  <li>Create a virtual machine (VM) on Azure by visiting [Azure Portal](https://portal.azure.com/). Configure it with Windows 10 Pro, version 22H2, with a minimum of 2 vCPUs and 16GB of memory.</li>
  
  <li>Connect to the VM using the public IP address through Remote Desktop Connection.</li>
  
  <li>Go to 'Control Panel' -> 'Programs' -> 'Turn Windows features on and off' to install/enable IIS in Windows with CGI and Common HTTP Features.</li>
  
  <li>Install PHP Manager for IIS and the Rewrite Module.</li>
  
  <li>Create a folder named 'PHP' in the C drive and download PHP 7.3.8, extracting its contents into C:\PHP.</li>
  
  <li>Install VC_redist.x86.exe from the installation files.</li>
  
  <li>Download and install MySQL 5.5.62, configuring it with a root password (e.g., Password1).</li>
  
  <li>Search for IIS in the Windows search bar, open it as an administrator, and register PHP from within IIS.</li>
  
  <li>Download and install osTicket v1.15.8, placing its 'upload' folder in c:\inetpub\wwwroot and renaming it to 'osTicket'.</li>
  
  <li>In IIS, go to sites -> Default -> osTicket, click “Browse *:80”, and enable necessary PHP extensions.</li>
  
  <li>Rename 'ost-sampleconfig.php' to 'ost-config.php', set up permissions, and continue setting up osTicket in the browser.</li>
  
  <li>Download and install HeidiSQL, create a new session with root credentials (Username: root, Password: Password1), and create a new database named 'osTicket'.</li>
  
  <li>Delete the 'setup' folder in C:\inetpub\wwwroot\osTicket and set the permissions of 'ost-config.php' back to "Read" only.</li>
  
  <li>Login to osTicket in the browser, completing the installation and setup process.</li>
</ol>

<p align="center">Congratulations! osTicket is successfully installed and configured.</p>
