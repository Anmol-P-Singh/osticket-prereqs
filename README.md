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
<h3> Within the Virtual Machine in Azure, Download the <code>osTicket-installation-Files.zip</code></h3>

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


### ✅Next Step: Turn On IIS and CGI

1. Open the **Control Panel**.  
   ![Open Control Panel](https://github.com/user-attachments/assets/9372d57a-9618-49f1-9dac-7addec1b014b)

2. Go to **Programs > Turn Windows features on or off**.  
   ![Windows Features](https://github.com/user-attachments/assets/c0b8daf1-a523-4a7a-b0fa-cddade52a7ca)

3. In the list, find **Internet Information Services (IIS)** and expand it.

4. Under **Application Development Features**, check the box for **CGI**.  
   ![Enable IIS with CGI](https://github.com/user-attachments/assets/a3559bef-dafb-4513-8ad5-6e9757c71a4d)

5. Click **OK** to apply the changes.This will allow your system to support PHP applications like osTicket.


<h3>📦 Open the <strong>osTicket-Installation-Files</strong> Folder and Install <strong>PHP Manager for IIS</strong></h3>

<p>
  <img width="760" height="385" alt="PHP Manager Installation" src="https://github.com/user-attachments/assets/d740c8ff-2387-48c4-9ea6-ef9ef935ebfe" />
</p>

<h3>🔄 Install the <strong>Rewrite Module</strong> from the same <strong>osTicket-Installation-Files</strong> Folder</h3>


<p>
  <img width="753" height="415" alt="Rewrite Module Installation" src="https://github.com/user-attachments/assets/993f802f-6d58-468a-9fc7-46102f2335c8" />
</p>

<br />





<h3>📁 Open File Explorer, go to the <strong>C:\</strong> drive, and create a new folder named <strong>PHP</strong></h3>

<p>
  <img width="797" height="603" alt="Creating PHP Folder in C Drive" src="https://github.com/user-attachments/assets/e89b0709-a7d1-46e0-90e8-5b8637e3f2ee" />
</p>

<br />

<h3>📦 Extract <code>php-7.3.8-nts-Win32-VC15-x86.zip</code> into the <strong>PHP</strong> Folder</h3>

<ul>
  <li>
    From the <strong>osTicket-Installation-Files</strong> folder, right-click on 
    <code>php-7.3.8-nts-Win32-VC15-x86.zip</code> and select <strong>Extract All</strong>.
  </li>
</ul>

<p>
  <img width="538" height="138" alt="Right-click to Extract PHP Zip" src="https://github.com/user-attachments/assets/b1bbc98e-94ac-49a2-a275-2da719d7fb39" />
</p>

<ul>
  <li>
    When prompted, browse to locate the <strong>PHP</strong> folder, or simply type 
    <code>C:\PHP</code> in the destination path.
  </li>
</ul>

<p>
  <img width="577" height="337" alt="Browse to PHP Folder Location" src="https://github.com/user-attachments/assets/7097cb1e-8080-4c5d-a1ea-c930337eb5ae" />
</p>

<br />
