<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

[How to install osTicket with Prerequisites
](https://drive.google.com/file/d/1sQb3wwXHAow4GDiorqhS6ZO0xA02H3We/view?usp=share_link)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Microsoft Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create an Azure Virtual Machine Windows 10
- Install / Enable IIS in Windows WITH
CGI and Common HTTP Features
- download and install PHP Manager for IIS
- download and install Rewrite module
- download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) and unzip the contents into C:\PHP
- download and install VC_redist.x86.exe.
- download and install MySQL 5.5.62
- Install osTicket v1.15.8
- download and install HeidiSQL

<h2>Installation Steps</h2>

Create a resource group in Azure (named - RSG-1)

<img width="721" alt="Screenshot 2024-04-25 at 3 24 38 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/fd030a7f-9246-4b38-9390-13bc5199db8e"> 

Create a Virtual Machine (VM-osTicket) in Azure with Windows 10 and 2 VCPU.

<img width="766" alt="Screenshot 2024-04-25 at 3 30 35 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/be48264f-9fb9-4446-a503-d9efa8bc128e">

VM-osTicket and RSG-1 deployed and ready to go. 

<img width="489" alt="Screenshot 2024-04-25 at 3 36 43 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/81b102f4-d80f-46ab-8921-3ae0cd8d6b04">

Install / Enable IIS in Windows WITH CGI and Common HTTP Features
Open VM-osTicket in Microsoft Remote Desktop
<img width="396" alt="Screenshot 2024-04-25 at 3 44 00 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/09ce9560-00e3-4f16-892a-78d6e1961caf">

Open the control panel and click programs
<img width="396" alt="Screenshot 2024-04-25 at 3 48 47 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/8863c25f-d8df-4f2a-9a01-082b8a77404e">

Turn windows features on or off
<img width="324" alt="Screenshot 2024-04-25 at 3 50 59 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/7b542417-72ba-492c-9e37-44077d747ad9">

Check internet Information Services
<img width="324" alt="Screenshot 2024-04-25 at 3 53 07 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/54017e72-3f3e-4fc6-8695-c724ef3655b6">

Check CGI
<img width="293" alt="Screenshot 2024-04-25 at 3 55 22 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/aca7f61b-395a-4aa7-a604-da77d075610b">

Expand common HTTP features and check the HTTP Redirection box and the WebDAV publishing box.
<img width="220" alt="Screenshot 2024-04-25 at 4 01 48 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/b40703e0-ad5d-4b3b-b36c-cd07ebee2cb6">

download and install PHP Manager for IIS
<img width="270" alt="Screenshot 2024-04-25 at 4 12 44 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/a153e87d-4c43-4359-aeac-17b9df540681">

download and install Rewrite module
<img width="270" alt="Screenshot 2024-04-25 at 4 15 07 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/90d9d9c1-1dbc-4ed8-9da1-4f28422638fc">

Create a folder (PHP) in Drive C: and then from the Installation Files, download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) and unzip the contents into C:\PHP.
<img width="270" alt="Screenshot 2024-04-25 at 4 24 40 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/7b89c710-ab59-49ef-98f1-696b78dfd47c">

download and install VC_redist.x86.exe.
<img width="270" alt="Screenshot 2024-04-25 at 4 26 42 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/b699967f-c878-41c6-8f26-3df62e5fc6ce">

download and install MySQL 5.5.62 
<img width="270" alt="Screenshot 2024-04-25 at 4 31 23 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/3190b604-cb79-49cd-bd3a-222886bf0d56">

create a MySQL server password
<img width="296" alt="Screenshot 2024-04-25 at 4 34 28 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/c5548b1a-ee0c-4052-92a8-6b1aa6f35be5">

register new PHP version
<img width="296" alt="Screenshot 2024-04-25 at 4 43 14 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/a79e2d83-a49c-42a4-8e67-e3976ea2dfb6">

Install osTicket v1.15.8
Download osTicket from the Installation Files Folder
<img width="215" alt="Screenshot 2024-04-25 at 4 50 52 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/8394cf35-bd35-437d-bce6-8e6d1b1bb8b2">

Extract and copy “upload” folder to c:\inetpub\wwwroot
<img width="255" alt="Screenshot 2024-04-25 at 4 54 00 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/8b783e6c-73cb-4d06-9ffe-fd3dfc1aea09">

Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”
<img width="255" alt="Screenshot 2024-04-25 at 4 55 06 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/9439ca99-9e1b-4a1f-81da-376e0e54d204">

Go to sites -> Default -> osTicket On the right, click “Browse *:80”.
<img width="640" alt="Screenshot 2024-04-25 at 4 58 23 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/90e1f5d8-7e0f-4a28-8ce2-5890d6ff253a">

Go back to IIS, sites -> Default -> osTicket, double-click PHP Manager and Click “Enable or disable an extension”. Enable: php_imap.dll, Enable: php_intl.dll, and Enable: php_opcache.dll
<img width="485" alt="Screenshot 2024-04-25 at 5 58 59 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/c0fc38fb-4391-48bb-9fed-a6305a2291cc">

<img width="157" alt="Screenshot 2024-04-25 at 6 00 41 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/3cad1e71-aafe-4c6d-a404-41e031b72e4a">

<img width="157" alt="Screenshot 2024-04-25 at 6 03 50 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/7411fae7-c9b2-424e-9617-2fe0ecfd6040">

<img width="157" alt="Screenshot 2024-04-25 at 6 04 43 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/899bf3a1-0dfd-405f-9ffa-e5d2a5e29fcb">

Ensure they have been enabled
<img width="349" alt="Screenshot 2024-04-25 at 6 06 11 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/6bbe6852-0d05-44ec-89fb-222d8aa65731">

Rename: ost-sampleconfig.php to ost-config.php
<img width="288" alt="Screenshot 2024-04-25 at 6 24 41 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/a3c58db3-fe9a-4da3-b2e7-b5062b13aa60">

<img width="288" alt="Screenshot 2024-04-25 at 6 21 41 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/aaa4f41a-15d4-4deb-af81-16f39f3851c6">

Assign Permissions: ost-config.php, Disable inheritance -> Remove All, New Permissions -> Everyone -> All
<img width="259" alt="Screenshot 2024-04-25 at 6 27 09 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/0afb5511-d326-4efd-9d5d-54ffbc4863be">

Continue Setting up osTicket in the browser (click Continue). Name Helpdesk and Default email (receives email from customers)
<img width="342" alt="Screenshot 2024-04-25 at 6 32 37 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/cd230968-805f-4fa6-a9f1-115f5aec009f">

download and install HeidiSQL 
<img width="305" alt="Screenshot 2024-04-25 at 6 08 18 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/316149cf-0d5f-44ef-b292-171f8b989667">

Access MySQL Database through HeidiSQL 
<img width="265" alt="Screenshot 2024-04-25 at 6 11 23 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/8ffb7884-5848-41ed-9d09-78446847abbb">

Create a new database and name it osTicket
<img width="234" alt="Screenshot 2024-04-25 at 6 14 07 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/e97e7c3f-6fbf-4497-86e4-da1b79f61551">

<img width="159" alt="Screenshot 2024-04-25 at 6 16 10 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/4696cf0f-6777-4ed7-b095-5deeeb530566">

Continue Setting up osticket in the browser and click install now.
Successful Installation
<img width="482" alt="Screenshot 2024-04-25 at 6 44 15 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/c3056766-74d8-4f66-a274-a8244bea6f7a">

Clean up
delete Setup folder 
<img width="265" alt="Screenshot 2024-04-25 at 6 41 52 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/45edb621-a3da-4da4-87fb-81c62d242d40">

Set Permissions to “Read” only: 
<img width="342" alt="Screenshot 2024-04-25 at 6 38 11 PM" src="https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/2bc72cd4-b09c-45c6-94fe-dfa57e1e979e">







