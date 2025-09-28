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

<h1>Downloads</h1>

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
  <img width="797" height="603" alt="Creating PHP Folder in C Drive"
       src="https://github.com/user-attachments/assets/e89b0709-a7d1-46e0-90e8-5b8637e3f2ee" />
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
  <img width="538" height="138" alt="Right-click to Extract PHP Zip"
       src="https://github.com/user-attachments/assets/b1bbc98e-94ac-49a2-a275-2da719d7fb39" />
</p>

<ul>
  <li>
    When prompted, browse to locate the <strong>PHP</strong> folder, or simply type
    <code>C:\PHP</code> in the destination path.
  </li>
</ul>

<p>
  <img width="577" height="337" alt="Browse to PHP Folder Location"
       src="https://github.com/user-attachments/assets/7097cb1e-8080-4c5d-a1ea-c930337eb5ae" />
</p>

<br />

<h3>🔧 Install the VC_redist.x86.exe from the osTicket-Installation-Files folder</h3>

<p>
  <img width="635" height="402" alt="Installing VC_redist"
       src="https://github.com/user-attachments/assets/7b80f405-ace6-4ec2-860f-60ba3d3ec710" />
</p>

<h3>🗄️ Steps to install MySQL 5.5.62 from the osTicket-Installation-Files folder</h3>

<p>
  <img width="720" height="365" alt="Installing MySQL"
       src="https://github.com/user-attachments/assets/4fba33f7-38f0-4ed5-8e24-fee6f98d50a7" />
</p>

<ol>
  <li>
    Choose the <strong>Typical</strong> setup type when prompted, then go ahead and complete the installation. Once it's done, launch the application.
  </li>
</ol>

<p>
  <img width="491" height="380" alt="Setup Type - Typical"
       src="https://github.com/user-attachments/assets/b4fae87b-3537-4639-962b-918b3684b09a" />
</p>

<ol start="2">
  <li>
    Choose the <strong>Standard configuration</strong>.
  </li>
</ol>

<p>
  <img width="524" height="461" alt="Screenshot 2025-09-26 070023"
       src="https://github.com/user-attachments/assets/db95f5e6-a443-471b-b536-2ffdb6d09a3a" />
</p>

<ol start="3">
  <li>
    Click <strong>Next</strong>, and when you reach the security settings, enter <strong>root</strong> for the passwords. Then click <strong>Next</strong>, followed by <strong>Execute</strong>, and finally, <strong>Finish</strong> to complete the setup.
  </li>
</ol>

<p>
  <img width="497" height="372" alt="Screenshot 2025-09-26 071300"
       src="https://github.com/user-attachments/assets/111410e4-42af-41c0-a200-aab236316de2" />
</p>

<h3>🚀 Run <strong>IIS</strong> as Administrator to register PHP from within IIS</h3>

<p>
  Open the Start menu, search for <strong>IIS</strong>, right-click on it, and choose <strong>Run as administrator</strong>.
</p>

<p>
  <img width="426" height="280" alt="Run IIS as Administrator"
       src="https://github.com/user-attachments/assets/41f4bfcf-a3d7-4d67-9bfc-49aa6f36bf68" />
</p>

<ol>
  <li>
    Open the <strong>PHP Manager</strong> from within <strong>IIS</strong>.
  </li>
</ol>

<p>
  <img width="426" height="158" alt="Open PHP Manager"
       src="https://github.com/user-attachments/assets/43798a6d-b3ea-4e60-8e43-93f0764ba989" />
</p>

<ol start="2">
  <li>
    Click on <strong>Register new PHP version</strong>.
  </li>
</ol>

<p>
  <img width="468" height="191" alt="Register new PHP version"
       src="https://github.com/user-attachments/assets/7d9164a9-c4f8-4875-9505-0a7be64361cf" />
</p>

<ol start="3">
  <li>
    Click the <strong>three dots</strong> to browse, then navigate to the <strong>PHP</strong> folder.
  </li>
</ol>

<p>
  <img width="819" height="650" alt="Browse to PHP folder"
       src="https://github.com/user-attachments/assets/712f3fa2-e30d-4a97-b1f8-25db799c13ca" />
</p>

<ol start="4">
  <li>
    Inside the <strong>PHP</strong> folder, select the <strong>php-cgi.exe</strong> file, then click <strong>OK</strong> to register it.
  </li>
</ol>

<p>
  <img width="634" height="174" alt="Select php-cgi.exe"
       src="https://github.com/user-attachments/assets/daf50e17-577e-4f02-9ca6-ddfa946f8c21" />
</p>

<ol start="5">
  <li>
    Restart <strong>IIS</strong> to apply the changes. You can do this by clicking <strong>Restart</strong>, or by <strong>stopping</strong> and then <strong>starting</strong> the service manually.
  </li>
</ol>

<p>
  <img width="1420" height="342" alt="Restart IIS Screenshot"
       src="https://github.com/user-attachments/assets/7c92bd6d-6a72-4ef2-ae7a-b0f6e842f84f" />
</p>

<h3>📦 Install osTicket v1.15.8</h3>

<ol start="1">
  <li>
    Go to the <strong>osTicket-Installation-Files</strong> folder, right-click on <strong>osTicket-v1.15.8.zip</strong>, and select <strong>Extract All</strong>.
  </li>
</ol>

<p>
  <img width="423" height="128" alt="Extract osTicket"
       src="https://github.com/user-attachments/assets/2ba6fdf8-4e26-4e9e-b59b-7cc50d80cc06" />
</p>

<p>
  <img width="577" height="411" alt="Extract location"
       src="https://github.com/user-attachments/assets/0c586350-4569-48b3-9ff5-f126d353b085" />
</p>

<ol start="2">
  <li>
    After the extraction is complete, open the <strong>osTicket-v1.15.8</strong> folder. Copy the <strong>upload</strong> folder to <strong>wwwroot</strong> by opening another File Explorer window and navigating to <strong>Windows C: ➜ inetpub ➜ wwwroot</strong>.
    <br>You can do this by dragging the folder from one window to the other.
  </li>
</ol>

<p>
  <img width="793" height="593" alt="Copy to wwwroot"
       src="https://github.com/user-attachments/assets/013843f1-864e-4e70-ad15-5680ab010b38" />
</p>

<p>
  <img width="668" height="129" alt="Upload in wwwroot"
       src="https://github.com/user-attachments/assets/7fb7e92d-c5b3-4351-b07f-cd045946c48e" />
</p>

<ol start="3">
  <li>
    Change the name of the <strong>upload</strong> folder to <strong>osTicket</strong>. Make sure to copy it exactly — capitalization matters.
  </li>
</ol>
<p><img width="133" height="93" alt="Screenshot 2025-09-26 110926" src="https://github.com/user-attachments/assets/354ac4c6-e546-4dab-8110-c4cfb764f6dc" />
</p>

<ol start="4">
  <li>
    Go back to <strong>IIS</strong> and restart the to apply changes.
  </li>
</ol>
<p><img width="991" height="341" alt="Screenshot 2025-09-27 091241" src="https://github.com/user-attachments/assets/e786046f-6a5a-41fd-a07f-9c703cdfff44" />
</p>

<ol start="5">
  <li>
    In <strong>IIS Manager</strong>, expand <code>[Your VM Name] &gt; Sites &gt; Default Web Site &gt; osTicket</code>, then click <strong>Browse *:80 (http)</strong> in the right-hand panel to launch osTicket.
    <br /><br />
  </li>
</ol>

<p>
  <img width="1424" height="748" alt="Screenshot 2025-09-27 092329" src="https://github.com/user-attachments/assets/78a20005-11e0-405b-aa01-e8251dfd77e6" />
</p>

<ul>
  <li>
    This will lead to your browser opening osTicket. If you notice that some extensions are disabled.
  </li>
</ul>

<p>
  <img width="808" height="729" alt="Screenshot 2025-09-27 102300" src="https://github.com/user-attachments/assets/5d57adc0-0f1a-4811-af48-c6432ffd57b0" />



</p>

<ol start="6">
  <li>
    Go back to <strong>IIS Manager</strong> and open <strong>PHP Manager</strong> under the <code>osTicket</code> site.
    <br /><br />
    In PHP Manager, follow these steps to enable the required extensions:
  </li>
</ol>

<!-- Step-by-step images in sequence -->
<div style="display: flex; flex-wrap: wrap; gap: 20px; margin-top: 10px;">
  <div style="text-align: center;">
    <img width="92" height="78" alt="Open PHP Manager" src="https://github.com/user-attachments/assets/31394f15-bc22-4243-9fd8-92292338ee6c" />
    <p><em>1. Open PHP Manager</em></p>
  </div>
  <div style="text-align: center;">
    <img width="350" height="166" alt="Enable or disable an extension" src="https://github.com/user-attachments/assets/7dd8924b-a4ca-41aa-bb5f-abe8e8f080df" />
    <p><em>2. Click "Enable or disable an extension"</em></p>
  </div>
  <div style="text-align: center;">
    <img width="606" height="654" alt="Enable PHP Extensions" src="https://github.com/user-attachments/assets/25204d94-8db0-49b6-b7b2-be524f03e627" />
    <p><em>3. Enable the following extensions:</em><br />
      <code>php_imap.dll</code>, <code>php_intl.dll</code>, <code>php_opcache.dll</code>
    </p>
  </div>
</div>

<ul>
  <li>
    Right-click on each of the required extensions and choose <strong>Enable</strong>.
  </li>
  <li>
    Refresh the <code>osTicket</code> site in your browser; enabled extensions will now be seen as active.
  </li>
</ul>
<p><img width="820" height="740" alt="Screenshot 2025-09-27 102409" src="https://github.com/user-attachments/assets/89cc9c39-1768-4c2f-bf22-c37ab15c2500" />
</p>

<h2>📝 Rename: <code>ost-sampleconfig.php</code> to <code>ost-config.php</code></h2>

<ol start="1">
  <li>
    Navigate to <strong>Local Disk (C:)</strong> &rarr; <strong>inetpub</strong> &rarr; <strong>wwwroot</strong> &rarr; <strong>osTicket</strong> &rarr; <strong>include</strong>.<br />
    Locate the file named <code>ost-sampleconfig.php</code>.
  </li>
</ol>
<p><img width="1122" height="630" alt="Screenshot 2025-09-27 110222" src="https://github.com/user-attachments/assets/418425c0-b5c7-4c0b-9d9e-649ae8f73fe2" />
</p>
<p>
  ✅ Rename the file <code>ost-sampleconfig.php</code> to <code>ost-config.php</code>.
</p>
<p><img width="601" height="153" alt="image" src="https://github.com/user-attachments/assets/ce3dca44-458d-419f-bba2-c3c39780d526" />
</p>

<h2>🔐 Assign and change Permissions in <code>ost-config.php</code></h2>
<ol start="1">
  <li>
    Right-click <code>ost-config.php</code> and select:<br />
    <strong>Properties</strong> &rarr; <strong>Security</strong> &rarr; <strong>Advanced</strong> &rarr; <strong>Disable inheritance</strong>.
  </li>
</ol>

<ul>
  <li>Click on <strong>Remove all</strong> to clear inherited permissions.</li>
</ul>
<P><img width="761" height="529" alt="image" src="https://github.com/user-attachments/assets/324bdd68-058c-42c4-8389-9e811a8b8ea4" />
</P>

<ol start="2">
  <li>
    Add new permissions by clicking <strong>Add</strong> &rarr; <strong>Select a principal</strong>, then type <code>Everyone</code> in the <em>Enter the object name</em> field.
    <br /><br />
    <img width="760" height="535" src="https://github.com/user-attachments/assets/73936358-2c70-4ee0-9d70-46e1436aeeee" alt="Add permissions dialog" />
    <ul>
      <li>Click <strong>Add</strong>.</li>
      <li>Click <strong>Select a principal</strong>.</li>
      <li>Type <code>Everyone</code> in the object name box.</li>
      <li>Click <strong>OK</strong>.</li>
    </ul>
  </li>
  <li>
    Set permissions for <code>Everyone</code> as needed (e.g., Full control) and click OK to apply.
    <br /><br />
    <img width="899" height="513" src="https://github.com/user-attachments/assets/f4c064d6-9999-41f8-a3c6-eebf8cede0fd" alt="Permission settings dialog" />
    <ul>
      <li>Check the <strong>Full control</strong> box.</li>
      <li>Click <strong>Ok</strong>.</li>
    </ul>
  </li>
</ol>

<p>
  <img width="893" height="457" src="https://github.com/user-attachments/assets/172ff0b9-5604-4b98-8dcb-530c4d425b33" alt="Permissions applied confirmation" />
</p>
<ul>
  <li>Click <strong>Ok</strong>.</li>
  <li>Click <strong>Apply</strong>.</li>
</ul>
<p>
  <img width="768" height="518" alt="Screenshot 2025-09-27 115749" src="https://github.com/user-attachments/assets/3c1bcab2-afb5-4e88-ab19-b2a1f586d515" />
</p>
<ul>
  <li>Click <strong>Ok</strong> to complete.</li>
</ul>
<h2 style="color: red; text-align: center;">
  Go osTicket installer brower tab click continue and fill out the highlighted sections. keep note of the passwords and ubersnames.
</h2>
<p><img width="622" height="306" alt="Screenshot 2025-09-28 073130" src="https://github.com/user-attachments/assets/2b78773a-7ef2-4c50-be63-1858bdbad4ad" />
</p>
<p><img width="736" height="625" alt="Screenshot 2025-09-28 073244" src="https://github.com/user-attachments/assets/78479a29-edc0-435a-b95f-df6896890f6c" />
</p>

<h2 style="color: red; text-align: center;">
<h2 style="color: red; text-align: center;">
 <h2 style="color: red; text-align: center;">
  📥 From osTicket-Installation-Files Download and install Heidi SQL
</h2>

<p>
  <img width="614" height="521" alt="HeidiSQL Installer Screenshot"
       src="https://github.com/user-attachments/assets/1774456d-2446-4cb0-af03-1be49c048fe2" />
</p>

<ol>
  <li>
    Just click <strong>Next</strong> until you reach <strong>Install</strong>, then click <strong>Finish</strong>.
  </li>
</ol>
<ol start="2">
  <li>
    Click <strong>Skip</strong> to open the HeidiSQL session manager. Press <strong>New</strong>, type password <code>root</code>, then click <strong>Open</strong>.
  </li>
</ol>

<p><img width="681" height="477" alt="Screenshot 2025-09-28 075609" src="https://github.com/user-attachments/assets/0052436b-bd75-4bc4-af79-5a10735ec47f" />
</p>

<ol start="3">
  <li>
    We're now creating a database called <code>osTicket</code>. Right-click the <strong>Unnamed</strong> tab, select <strong>Create new</strong> → <strong>Database</strong>.
  </li>
</ol>
<p><img width="749" height="528" alt="Screenshot 2025-09-28 080315" src="https://github.com/user-attachments/assets/578d9854-0940-40aa-8683-e5a6be931b31" />
</p>
<ul>
  <li>Enter <code>osTicket</code> as the name and click <strong>OK</strong>.</li>
</ul>
<p><img width="320" height="255" alt="Screenshot 2025-09-28 080817" src="https://github.com/user-attachments/assets/aa122c57-7598-41ee-804c-12ea7eb39e6c" />
</p>
<h3>➡️ Database set up! Return to the osTicket browser to complete the form and install.</h3>
<ul>
  <li>MySQL Database: <code>osTicket</code></li>
  <li>MySQL Username: <code>root</code></li>
  <li>MySQL Password: <code>root</code></li>
  <li>Click <strong>Install Now!</strong></li>
</ul>

<p><img width="708" height="337" alt="Screenshot 2025-09-28 081937" src="https://github.com/user-attachments/assets/13356c00-2f07-45a8-8316-2f334790962b" />
</p>
<h2 style="color: green; text-align: center;">🎉 osTicket has been installed successfully!</h2>
<p><img width="736" height="570" alt="Screenshot 2025-09-28 082255" src="https://github.com/user-attachments/assets/5959d270-cbd1-4e26-942a-7b7c4f724eae" />
</p>
