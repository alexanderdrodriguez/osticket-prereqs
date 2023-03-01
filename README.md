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
<img src="https://i.imgur.com/aCVH5Sq.png" alt="Disk Sanitization Steps"/>
</p>
<p>
Our first step is going to be to open your Microsoft Azure Windows 10 virtual machine via "Remote Desktop Connection" so we can start installing osTicket on it! 
Simply grab your virtual machines public IP address and login using the username and password you provided Azure.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open the Installation Files and download the required files for osTicket installation.

Install and enable IIS in Windows with CGI. To do this, open the Server Manager, navigate to "World Wide Web Services" -> "Application Development Features" -> check "CGI".
</p>
<br />
