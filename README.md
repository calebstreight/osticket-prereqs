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

<h2> Prerequisites and Step by Step osTicket Setup</h2>

- First I enabled IIS in Control panel > Programs > Turn Windows Features on or off. Next you want to hit the drop down menu and enable 'CGI' inside of the 'Application Development Features' folder. Lastly in the 'Common HTTP Features' folder make sure all folders are checked. (As Shown below.)

- For trouble shooting and making sure everything was done correctly, simply go on a internet browser and type the loopback address, '127.0.0.1' and you should be displayed with an IIS webpage. (Also Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/fe30a78b-4935-4cde-9b39-547a6d6347cf)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/5b216df6-a7c7-472f-b442-c1228553ba14)


- Next you're going to install 'PHP Manager' for IIS. (Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/5ed09a4c-3815-411f-a236-b8c0081d2fc3)


- Next install 'Rewrite Module' for IIS. (Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/81bf20db-ace5-40e8-8a3b-9d9a3d7b942a)


- Next create the directory C:\PHP. This PC > C-drive > create folder 'PHP'. (Shown below)

  ![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/be01bc79-d928-4c5e-a342-02e47c0e8f74)


- Next download 'PHP' and extract the PHP folder into the directory (C:\PHP), that we created above. (Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/49b4b6c7-ec24-411b-ba41-bb3744670737)

  
- Next download 'Microsoft Visual C++' (Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/43e08267-d484-4dd4-ad62-d900560df509)
