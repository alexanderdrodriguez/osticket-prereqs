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
Simply grab your virtual machines public IP address and login using the username and password you provided Azure.
</p>
<p>
<img src="https://i.imgur.com/aCVH5Sq.png">
</p>
<br />

<p>
Next we have to install and enable Internet Information Services (IIS) in Windows with CGI. To do this, open the Control panel and click "Programs", then click "Turn Windows features on or off". Next check each of the features exactly like in one of the images below, in the order of "World Wide Web Services" -> "Application Development Features" -> check "CGI". Press "OK" and once the installation is finished open Microsoft Edge and type 127.0.0.1 to see if Internet Information Services is working correctly.
</p>
<p>
<img src="https://i.imgur.com/IQH33cf.png">
<img src="https://i.imgur.com/p7TsqoH.png">
<img src="https://camo.githubusercontent.com/27dacaaa327beb3d34eba9fefa06ee647f5340d4289770b3bde0c042d8233440/68747470733a2f2f692e696d6775722e636f6d2f37475646734d4e2e706e67"/>
<img src="https://i.gyazo.com/32e1749f2d29f450e53461ed1b6c06e5.png">
</p>
