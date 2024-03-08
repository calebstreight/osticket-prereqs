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

<h2> Prerequisites and Step by Step osTicket Installation</h2>

- First enable IIS in Control panel > Programs > Turn Windows Features on or off. Next you want to hit the drop down menu and enable 'CGI' inside of the 'Application Development Features' folder. Lastly in the 'Common HTTP Features' folder make sure all folders are checked. (As Shown below.)

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


- Lastly download 'MySQL Server'. Make sure to select 'Standard Setup' when installing MySQL Server and remembering your 'root password' we will need it later. (Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/f5e83c76-502b-47a1-9f18-9054b7f195b9)


 - Next open 'IIS' as administrator and navigate to 'PHP Manager' once opened. Click 'PHP Manager' to open it in 'IIS' and click 'Register New PHP Verison'. Next, navigate to C:\PHP and click 'CGI' inside the folder. Click done. Now navigate to 'restart' inside of 'IIS'. Now your finished setting up PHP inside of 'IIS'. (All shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/cd6bb5f1-ed45-4d7f-801e-63894c7f5708)
![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/ac5f9089-b6ba-46f4-86c5-5ca49c92433c)
![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/a29e4011-672a-47ae-b665-c57423cf1931)
![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/c58f9b77-3c8c-4b76-9ecb-f45df3788f83)


- Next Download osTicket and Extract 'upload' folder to c:\inetpub\wwwroot. Then Within c:\inetpub\wwwroot, Rename 'upload' to 'osTicket'. After this step is finished restart 'IIS' again. (Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/fbb4da8a-91d3-42dd-a94d-548cf644ffff)
![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/73cf65a6-47ac-43b4-bc78-6308d6bf1212)
![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/cb450aee-f660-4e30-b369-c6dd1a319e9b)


- Next inside of 'IIS' on the left side click the drop down on 'Sites' folder then the drop down on 'Default Web Site' and then highlight 'osTicket'. Once 'osTicket' is highlighted click 'Browse *:80(http)' on the right (Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/c6ea6930-f931-438a-9eab-ed9ad7d67ff7)
![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/68d03cb2-636e-406f-9b87-ccb61a783ac3)


- If done correctly osTicket should be open in a web browser like so (Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/0520a216-3b80-43f2-8473-32a1912256fd)


- Next to enable some of the red X's shown on the osTicket installer we will navigate to osTicket folder in 'IIS' (the folder that we highlighted in the previous step) and we will highlight it once again and click 'PHP Manager" and once inside 'PHP Manager' scroll down and click 'Enable or disable an extension'. Then highlight and enable, 'php_imap.dll', 'php_intl.dll', 'php_opcache.dll'. 

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/e2c5ee7a-ad44-4452-a722-b9dca70adfbf)
![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/40dfd6ba-5f46-4343-8b77-3a7551e5930c)


- Next refresh the 'osTicket' installer page and it should now look like so.  (Shown below)

  ![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/3e279604-6bdc-426b-ba05-eab5f9c61913)


  - Next rename a folder From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
  To: C:\inetpub\wwwroot\osTicket\include\ost-config.php. delete 'sample' from file. (Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/cee26d96-2db1-4fb4-a678-5b507b82c05d)


- Next Assign Permissions: ost-config.php Disable inheritance -> Remove All ---- New Permissions -> Everyone -> All (setting this file so everyone has permissions to make changes to it. This is because osTicket will be manipulating this folder.) (Shown below) properties > Security > Advanced > Disable Inheritance > Add > Everyone.

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/95075f5d-cd5e-4468-bbbc-14cb78d63c72)
![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/0df4666a-1f04-4cac-9bef-34e9bb1f1589)
![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/6263630e-275e-48a3-8f2a-8c97d6f81ab3)


- Next we are going to hit 'continue' on osTicket installer webpage and fill it out. (Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/a83b8b2c-c401-4afa-b01f-34949f28337c)
![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/b5f8ade1-1a61-4038-9348-0d54806ad1fd)


- Next We're gonna install 'HeidiSQL' which allows us to connect to that SQL data base. (Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/c4162211-f6c2-4c36-8748-51959dfd46df)


- Next Inside of HeidiSQL use your password that you created earlier that I mentioned to keep track of. Once that is entered we are connected to the server. (Shown below) 

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/ee5bdbf5-e076-4d5b-8b9f-28a9af75b22b)
![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/1da9d930-7558-4a1e-98a8-c0fabc337ba0)


- Next in the HeidiSQL data base we are going to create a new data base by right clicking on 'unnamed' and scrolling down to 'create new' and then click 'data base' and name it 'osTicket'. (Show below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/d58e3a53-87d1-469e-86b6-4e243a8b4d64)


- Go back to the osTicket browser installtion site and finish filling out the 'SQL' portion. We will use the username and password that we used to login to HeidiSQL and the 'SQL database' name is the one we just created which is 'osTicket'. (Shown below)

![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/53b76d43-2a6f-46a4-b9f6-fe5aa9173d3d)


- Lastly click 'Install' on the bottom of the osTicket webpage. If everything is done correctly you will have osTicket up and running. Use 'admin' information you just filled out to log in. (Shown below)

  ![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/8c4cff7e-32a1-402d-ad3a-bf9e84b948ab)
  ![image](https://github.com/calebstreight/osticket-prereqs/assets/162412951/ea78cd93-0d40-4f2b-83a3-32807180d5b2)

