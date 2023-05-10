<p align="center">
<img src="https://static.wixstatic.com/shapes/2ebf04_6ddec2f2c2eb4cd4ada9cef3f6ace924.svg" alt="osTicket Logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial provides an overview of the necessary prerequisites and installation procedures for deploying osTicket, an open-source platform for managing and resolving help desk support tickets.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://youtu.be/dEvGaxOgqf0)

[![YouTube](https://static.wixstatic.com/media/2ebf04_4ab570f6e52b411e9d743f591c649d73~mv2.png)](https://youtu.be/dEvGaxOgqf0)
</p>

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Internet Information Services (IIS)

<h2>Operating System Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enable Internet Information Services (IIS) and CGI.
- Install PHP Manager for IIS.
- Install URL Rewrite Module.
- Extract PHP into a new folder on Local Disk (C:) and register it in IIS.
- Install Microsoft Visual C++ Redistributable.
- Install MySQL and set up a password for root.
- Extract osTicket into the wwwroot folder.
- Enable php_imap.dll, php_opcache.dll, and php_intl.dll in IIS.
- Install HeidiSQL and create a new database.

<h2>Installation Steps</h2>

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_46fec3f74ebb4eaf803cb5cb612c6939~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 1: Create a resource group in Azure and name it "RG-osTicket."
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_77387910fc1a4be8b67ed724302d2e44~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 2: Create a virtual machine and select "RG-osTicket" as the resource group and "Windows 10 Pro, Version 21H2" as the image.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_05b52ea6778e40a090e17941939c969b~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 3: Use the Remote Desktop Connection to connect to the virtual machine (VM) using its public IP address.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_30bd0a8b94a14c9d8f1daa8eabefbf05~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 4: Navigate to "Turn Windows Features on or off" in the Control Panel menu.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_1ba15b5709a2434a9c676c21bd01ccf6~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_a6e5746c3bc44b529b5663237726fe20~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation">
</p>
<p>
Step 5: Enable Internet Information Services (IIS) and CGI.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_69ba87d49db24386a77890054495d507~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_ef74369fcc68481b9d6a42c04ba21362~mv2.png" height="50%" width="50%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 6: Download and install <a href="https://iis.net/downloads/community/2018/05/php-manager-150-for-iis-10">PHP Manager For IIS</a>. 
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_38c073f7680448e494baf97916f51593~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_6c6d0a55c7c24a81a52ed7cfa7fc9ea5~mv2.png" height="50%" width="50%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 7: Download and install <a href="https://iis.net/downloads/microsoft/url-rewrite">URL Rewrite Module</a>.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_25e7ed24bf1d4740a44e24084ec46bea~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 8: Navigate to Local Disk (C:) and create a new folder named "PHP."
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_a165a508089b4fc18ecc369532a80a4e~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 9: Download <a href="https://windows.php.net/download">PHP:</a> Hypertext Preprocessor. 
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_e1639b4d2eb04230b358191a83192074~mv2.png" height="50%" width="50%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 10: Unzip the downloaded PHP file into the "PHP" folder on Local Disk (C:).
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_5c7ade1560b74192afd51a8f539e2f41~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_6157427428c14221a9e41ab4cd6745f1~mv2.png" height="50%" width="50%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 11: Download and install <a href="https://learn.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist?view=msvc-170">Microsoft Visual C + + Redistributable</a>.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_4d4e5caedb364f3f87ab118b7eb7e831~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_414f33a46cc8409cbfd36e7c211617fb~mv2.png" height="50%" width="50%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 12: Download and install <a href="https://downloads.mysql.com/archives/community">MySQL</a>.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_5aef81d1038543ae87bf25a923554068~mv2.png" height="50%" width="50%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 13: Launch the MySQL Instance Configuration Wizard, select "standard configuration", install as Windows Service, set a password under "Modify Security Settings", and click "Execute."
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_340541966fd747b68875c02bf744f56e~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 14: Launch Internet Information Services as an administrator and navigate to the PHP Manager.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_74501320361645da9abc78cb89509097~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_670015e9b5b14932b4d9cea259ef32b3~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 15: Click on "Register new PHP version" and locate the "php-cgi" file in the PHP folder that was created in the Local Disk (C:).
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_ce7d6272c03f4f29a79c4253ff7795b1~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 16: Download and extract the latest version of <a href="https://osticket.com/download">osTicket</a>.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_2bd2b51d008640c98bb891c114fa4cb0~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 17: Open the "osTicket" folder and move the "upload folder" to the "wwwroot" folder in the "inetpub" folder of the Local Disk (C:).
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_81d6cf73e1904ae9bc188f4619b99155~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 18: Rename the "upload" folder to "osTicket."
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_aed8427d753b4b949e06064446aaab2a~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 19: Return to the PHP Manager and select "Enable or disable an extension."
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_39102b9e179446a4a774f5c635f3b6c1~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 20: Enable the following extensions in the PHP Manager:
- php_imap.dll
- php_opcache.dll
- php_intl.dll
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_6a8804c0450143969a82028bc0a0d38f~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 21: Navigate to the osTicket folder located in the wwwroot directory, open the "include" folder, and rename the file "ost-sampleconfig.php" to "ost-config.php."
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_22b6dbd0f8c24dfe964a170eaeb3c92b~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 22: Open the Properties of ost-config.php by right-clicking on it. Then, go to the Security tab and click on Advanced. Finally, click on "Disable Inheritance."
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_9f38a1f78c5f45c2806ac0024152a676~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 23: Click on "add", select "principle", type "everyone" and allow all basic permissions.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_f237c60e1dcb4ef49957ef886aa6e54d~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 24: Launch Microsoft Edge and navigate to https://localhost/osTicket/setup. Then, click on the "Continue" button located at the bottom of the page.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_5d2927f74cf44a24b9fed7eddeae24a9~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 25: Complete all the required fields for the "System" and "Admin User" settings.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_373f0f0c369c46d692ca831b96a0c5db~mv2.png" height="50%" width="50%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 26: Download and install <a href="https://www.heidisql.com/installers/HeidiSQL_12.3.0.6589_Setup.exe">HeidiSQL</a>.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_6d062cc7beeb45a5bdcdbc8a377af580~mv2.png" height="50%" width="50%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 27: Launch HeidiSQL, then click on "New" and enter the password for the root account that was set up earlier. Finally, click on "Open" to proceed.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_b589fb61255f4778b73871ffb880c6b5~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 28: Create a new database in HeidiSQL by right-clicking and selecting "Create new", then entering "osTicket" as the name.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_6cde76f0469745879219224cb9299254~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 29: Return to the osTicket setup page in Microsoft Edge and complete the remaining fields in the "Database Settings" section. After filling in all the required information, click on the "Install now" button.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_c05d50a19517450fac1b13f62d2e500c~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 30: Navigate back to the "wwwroot" folder and locate the "osTicket" folder. Delete the "setup" folder.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_656ded18f71e452cac05d4d2b4dc12ab~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 31: Access the include folder in osTicket, then navigate to ost-config.php. Right-click on ost-config.php, select Properties, then Security, Advanced, and modify the basic permissions by removing Full Control, Modify, and Write.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_8e7f7b6aece0475f8c5a5443207fd7d2~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 32: Log in to https://localhost/osTicket/scp/login.php.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_5f95f05113564d6ebf9f4615d146d2ce~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
Step 33: If everything was installed correctly, we should see this page.
</p>
<br />

<p align="center">🧠 <b><i>Being a student is easy. Learning requires actual work. ~ William Crawford</b></i> 📓</p>
<br />
<p align="right"> Next: <a href="https://github.com/stevennocent/post-install-config"
>osTicket: Post-Installation Configuration</a></p>
