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

- Create a Resource Group in Azure
- Create a Windows 10 Virtual Machine (VM) with 2-4 Virtual CPUs
- Make sure that when you are creating the Virtual Machine you allow it to create a new Virtual Network (Vnet)
- Have these [osTicket Installation Files](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6) open and ready to install within your Windows 10 Virtual Machine.

<h2>Installation Steps</h2>

<p>
Our first step is going to be to open your Microsoft Azure Windows 10 virtual machine via "Remote Desktop Connection" so we can start installing osTicket on it! 
Simply copy and paste your virtual machines public IP address and login using the username and password you provided Azure.
</p>
<p>
<img src="https://i.imgur.com/aCVH5Sq.png">
</p>
<br />

<p>
Next we have to install and enable Internet Information Services (IIS) in Windows with CGI. To do this, open the Control panel and click "Programs", then click "Turn Windows features on or off". Next check each of the features exactly like in one of the images below, in the order of "World Wide Web Services" -> "Application Development Features" -> check "CGI", and then press "OK". 

Once the installation is finished open Microsoft Edge and type and enter 127.0.0.1 into the search bar, if the IIS page appears that means that everything was installed correctly.
</p>
<p>
<img src="https://i.imgur.com/IQH33cf.png">
<img src="https://i.imgur.com/p7TsqoH.png">
<img src="https://camo.githubusercontent.com/27dacaaa327beb3d34eba9fefa06ee647f5340d4289770b3bde0c042d8233440/68747470733a2f2f692e696d6775722e636f6d2f37475646734d4e2e706e67"/>
<img src="https://i.imgur.com/syVKVO4.png">
</p>

<p>
Now within the VM open this link (https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6). This is going to provide all of the installation files we need in order to install osTicket.
  
Download and install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi) from the Installation Files.
<img src="https://i.imgur.com/b4K90DP.png">

Download and install the Rewrite Module (rewrite_amd64_en-US.msi) from the Installation Files.
<img src="https://i.gyazo.com/a0e9c68340ab1e7e6c046d9030d76db9.png">
  
Create a folder named "PHP" in the location C:\PHP
<img src="https://i.gyazo.com/029bcb938fb400c7b03836cab8d63150.png">
  
Download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) from the Installation Files and unzip the contents into C:\PHP.
<img src="https://i.gyazo.com/14855f2802e4a90b0d7e18c057bb4c29.png">
<img src="https://i.gyazo.com/9c9c967a17559e45a8134e6435259a7e.png">
<img src="https://i.gyazo.com/912b26f2e87cf1627f2e3a23d1d92e3a.png">
  
Download and install VC_redist.x86.exe from the Installation Files.
<img src="https://i.gyazo.com/be0375247a2c0e5aa9215fc50fe5c64a.png">

Download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi) from the Installation Files. During the installation process, select "Typical Setup", then launch the Configuration Wizard (after installation) and select "Standard Configuration" with password "Password1".
<img src="https://i.gyazo.com/943c13b4805569234fbaae63156748eb.png">
<img src="https://i.gyazo.com/07a7de5cf1ce3efa83d95b9168eed72d.png">
<img src="https://i.gyazo.com/4578a4201546941acfab6ce3923631d4.png">
<img src="https://i.gyazo.com/f7857f33a399c5492eedaa644e4ae6a0.png">
<img src="https://i.gyazo.com/e6721a1a99ee461c50ba94520a3e4e3a.png">  
  
Open IIS as an Admin and register PHP from within IIS.
<img src="https://i.gyazo.com/93c4a3ec8a09046039bb007b0aa9d588.png">
<img src="https://i.gyazo.com/f6c789ca23a21e99af894c6e85b3e128.png">
<img src="https://i.gyazo.com/fd6c837a883ed1b17abb00af4892e0bb.png">

<p>Reload IIS (Open IIS, Stop and Start the server).</p>
<img src="https://i.gyazo.com/86285f2b8b2d653c687f3b4b4ff5ed40.png">
</p>
