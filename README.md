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
- download and install MySQL 5.5.62
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


Once the virtual machine is up and running, to install/enable IIS in windows the CGI has to be checked and make sure all features in the common HTTP features are highlighted. To confirm if the IIS has installed, go to the web browser and type 127.0.0.1 and once it opens up like the image above then IIS has successfully been installed/enabled.

![image](https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/20eff0eb-256c-4395-ad41-c3b254d46343)

Download and install PHP manager (helps in running osTicket by providing a convenient way to manage PHP settings and ensure that the server meets the necessary requirements for running osTicket smoothly), rewrite module (this plays a crucial role in running osTicket by providing URL manipulation capabilities, improving user experience, and facilitating better SEO practices), VC_redist (provides the necessary runtime components and dependencies required by osTicket and its associated libraries or extensions that were built with Visual C++..), MySQL (provides the robust data storage, management, scalability, performance, reliability, security, and integration capabilities required for a ticketing system to operate effectively) AND HeidiSQL (It provides a convenient and efficient way to interact with the database, perform database management tasks, and troubleshoot database-related issues, ultimately helping to ensure the smooth operation of osTicket).

![image](https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/13acbfc9-5d03-430d-9156-5c420c0c74c7)

Once OsTicket has been properly installed, it will show the image above. Then a cleanup has to be done by Deleting: C:\inetpub\wwwroot\osTicket\setup and Set Permissions to “Read” only: C:\inetpub\wwwroot\osTicket\include\ost-config.php
</p>
<br />

