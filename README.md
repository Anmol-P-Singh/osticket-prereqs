<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>

<p>This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system (<strong>osTicket</strong>).</p>

<h2>Environments and Technologies Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machines/Compute)</li>
  <li>Remote Desktop</li>
  <li>Internet Information Services (IIS)</li>
</ul>

<h2>Operating Systems Used</h2>
<ul>
  <li>Windows 10 (21H2)</li>
</ul>

<h2>List of Prerequisites</h2>
<ul>
  <li>IIS</li>
  <li>PHP Manager</li>
  <li>VC_redistx86</li>
  <li>MySQL 5.5.62</li>
  <li>Rewrite Module</li>
  <li>Heidi SQL</li>
</ul>

<h2>Installation Steps</h2>
<h3>1. Within the Virtual Machine in Azure, Download the <code>osTicket-installation-Files.zip</code></h3>

<p>
  Inside your VM, <a href="https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD" target="_blank">download the osTicket installation files</a> and unzip them onto your desktop. These files will be used to install osTicket.
</p>

<ul>
  <li>
    <img width="505" height="127" alt="Download Prompt" src="https://github.com/user-attachments/assets/940b7b32-1348-4b5d-9b9f-a79a834e043b" />
    <p>Download prompt showing zip file.</p>
  </li>
  <li>
    <img width="345" height="147" alt="Unzipping Files" src="https://github.com/user-attachments/assets/094e5297-25bb-45c0-89e3-4eb967c224d5" />
    <p>Unzipping the installation files to the desktop.</p>
  </li>
  <li>
    <img width="445" height="47" alt="Folder Name" src="https://github.com/user-attachments/assets/0d8a0de8-65f9-46e2-8b12-09d46fc28ec0" />
    <p>Ensure the folder is named <code>osTicket-Installation-Files</code>.</p>
  </li>
</ul>


<p>



</p>


### ✅ Step: Turn On IIS and CGI

1. Open the **Control Panel**.  
   ![Open Control Panel](https://github.com/user-attachments/assets/9372d57a-9618-49f1-9dac-7addec1b014b)

2. Go to **Programs > Turn Windows features on or off**.  
   ![Windows Features](https://github.com/user-attachments/assets/c0b8daf1-a523-4a7a-b0fa-cddade52a7ca)

3. In the list, find **Internet Information Services (IIS)** and expand it.

4. Under **Application Development Features**, check the box for **CGI**.  
   ![Enable IIS with CGI](https://github.com/user-attachments/assets/a3559bef-dafb-4513-8ad5-6e9757c71a4d)

5. Click **OK** to apply the changes.This will allow your system to support PHP applications like osTicket.


