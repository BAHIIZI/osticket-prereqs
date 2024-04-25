<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

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

![image](https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/477df87e-ca3b-4012-a377-d1e8cbce32d6)

Once the virtual machine is up and running, to install/enable IIS in windows the CGI has to be checked and make sure all features in the common HTTP features are highlighted. To confirm if the IIS has installed, go to the web browser and type 127.0.0.1 and once it opens up like the image above then IIS has successfully been installed/enabled.

![image](https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/20eff0eb-256c-4395-ad41-c3b254d46343)

Download and install PHP manager (helps in running osTicket by providing a convenient way to manage PHP settings and ensure that the server meets the necessary requirements for running osTicket smoothly), rewrite module (this plays a crucial role in running osTicket by providing URL manipulation capabilities, improving user experience, and facilitating better SEO practices), VC_redist (provides the necessary runtime components and dependencies required by osTicket and its associated libraries or extensions that were built with Visual C++..), MySQL (provides the robust data storage, management, scalability, performance, reliability, security, and integration capabilities required for a ticketing system to operate effectively) AND HeidiSQL (It provides a convenient and efficient way to interact with the database, perform database management tasks, and troubleshoot database-related issues, ultimately helping to ensure the smooth operation of osTicket).

![image](https://github.com/BAHIIZI/osticket-prereqs/assets/164538571/13acbfc9-5d03-430d-9156-5c420c0c74c7)

Once OsTicket has been properly installed, it will show the image above. Then a cleanup has to be done by Deleting: C:\inetpub\wwwroot\osTicket\setup and Set Permissions to “Read” only: C:\inetpub\wwwroot\osTicket\include\ost-config.php
</p>
<br />

