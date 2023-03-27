<p align="center">
<img src="https://static.wixstatic.com/shapes/2ebf04_6ddec2f2c2eb4cd4ada9cef3f6ace924.svg" alt="osTicket Logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial provides a technical overview of the necessary conditions and installation procedures for deploying osTicket, an open-source platform for managing and resolving help desk support tickets.<br />


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
1. Create a resource group within Azure and name it “RG-osTicket.”
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_77387910fc1a4be8b67ed724302d2e44~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
2. Create a virtual machine and choose “RG-osTicket” as the resource group and Windows 10 Pro, Version 21H2 as the image.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_05b52ea6778e40a090e17941939c969b~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
3. Remote Desktop Connection into the virtual machine (VM) via the VM’s public IP Address.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_30bd0a8b94a14c9d8f1daa8eabefbf05~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
4. Go to “Turn Windows Features on or off” in the control panel menu.
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
5. Enable Internet Information Services (IIS) and CGI.
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
6. Download and Install PHP Manager For IIS version 1.5.0 by going to https://iis.net/downloads/community/2018/05/php-manager-150-for-iis-10. 
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
7. Download and Install URL Rewrite Module 2.1 by going to https://iis.net/downloads/microsoft/url-rewrite.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_25e7ed24bf1d4740a44e24084ec46bea~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
8. Go to the Local Disk (C:) and create a new folder called “PHP.”
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_a165a508089b4fc18ecc369532a80a4e~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
9. Download PHP 7.4.33 by going to https://windows.php.net/downloads/release and click php-7.4.33-nts-Win32-vc15-x64.zip.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_e1639b4d2eb04230b358191a83192074~mv2.png" height="50%" width="50%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
10. Extract PHP 7.4.33 into the PHP folder created in Local Disk (C:).
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
11. Download and Install Microsoft Visual C + + Redistributable by going to https://learn.microsoft.com/en-US/cpp/windows/lastest-supported-vc-redist?view=msvc-170, scroll down and click the link for the x86 version.
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
12. Download and Install MySQL 5.5.62 by going to https://downloads.mysql.com/archives/community/ and for product version choose 5.5.62 and download the 32-bit, MSI Installer.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_5aef81d1038543ae87bf25a923554068~mv2.png" height="50%" width="50%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
13. Launch the MySQL Instance Configuration Wizard → choose “standard configuration” → Install as Windows Service → Enter a password under Modify Security Settings → Then click Execute.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_340541966fd747b68875c02bf744f56e~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
14. Run Internet Information Services as an administrator and go to the PHP Manager.
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
15. Click register new PHP version → Search for the PHP folder created in Local Disk (C:) and select the “php-cgi” file.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_ce7d6272c03f4f29a79c4253ff7795b1~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
16. Go to https://osticket.com/download/ and download the latest version of osTicket and extract the folder.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_2bd2b51d008640c98bb891c114fa4cb0~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
17. Open the “osTicket” folder and drag the “upload folder” to the “wwwroot” folder found by going to the Local Disk (C:) → “inetpub” folder → wwwroot.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_81d6cf73e1904ae9bc188f4619b99155~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
18. Rename the “upload folder” to “osTicket.”
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_aed8427d753b4b949e06064446aaab2a~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
19. Go back to the PHP Manager and click “Enable or disable an extension.”
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_39102b9e179446a4a774f5c635f3b6c1~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
20. Enable the following extension:
-php_imap.dll
-php_opcache.dll
-php_intl.dll
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_6a8804c0450143969a82028bc0a0d38f~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
21. Go to the osTicket folder in wwwroot → Then click the “include” folder → Find and rename ost-sampleconfig.php file to ost-config.php.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_22b6dbd0f8c24dfe964a170eaeb3c92b~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
22. Right-click on ost-config.php → Properties → Security → Advanced → Click “Disable Inheritance.”
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_9f38a1f78c5f45c2806ac0024152a676~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
23. Click add → Select principle → Type “everyone” and allow all basic permissions.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_f237c60e1dcb4ef49957ef886aa6e54d~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
24. Open Microsoft Edge and go to https://localhost/osTicket/setup/ and click continue at the bottom.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_5d2927f74cf44a24b9fed7eddeae24a9~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
25. Fill out all the “System” and “Admin User” settings.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_373f0f0c369c46d692ca831b96a0c5db~mv2.png" height="50%" width="50%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
26. Download and Install HeidiSQL by going to https://heidisql.com/instalers/HeidiSQL_12.3.0.6589_setup.exe.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_6d062cc7beeb45a5bdcdbc8a377af580~mv2.png" height="50%" width="50%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
27. Launch HeidiSQL → Click new and enter in the password we created earlier for root and click open. 
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_b589fb61255f4778b73871ffb880c6b5~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
28. Right-Click on HeidiSQL → Create new → Database and for the name type “osTicket.”
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_6cde76f0469745879219224cb9299254~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
29. Go back to osTicket in Microsoft Edge to finish the “Database Settings” section and fill out the rest of the information and click Install now.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_c05d50a19517450fac1b13f62d2e500c~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
30. Go back to wwwroot folder → osTicket and delete the setup folder.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_656ded18f71e452cac05d4d2b4dc12ab~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
31. Click the include folder and go down to ost-config.php → Properties → Security → Advanced → and edit the basic permissions by removing:
- Full Control
- Modify
- Write
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_8e7f7b6aece0475f8c5a5443207fd7d2~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
32. Go to https://localhost/osTicket/scp/login.php and login.
</p>
<br />

<p>
<p align="center"> 
<img src="https://static.wixstatic.com/media/2ebf04_5f95f05113564d6ebf9f4615d146d2ce~mv2.png" height="80%" width="80%" alt="osTicket: Prerequisites and Installation"/>
</p>
<p>
33. We should this page if everything was installed correctly. :)
</p>
<br />
<p align="center"><b><i>🙌💥People may hear your words, but they feel your attitude. ~ John C. Maxwell🙌💥</b></i></p>
<p align="right"> Next up, <a href="https://github.com/stevennocent/post-install-config"
>osTicket: Post-Installation Configuration</a></p>
