<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png"/>
</p>

<h1> How to Install osTicket </h1>
This is an easy guide to installing a help desk ticketing system called osTicket.<br/>

<h2> Software & Technologies Used</h2>

- Windows 10
- Microsoft Azure (Virtual Machines)
- Remote Desktop (RDP)
- Internet Information Services (IIS)

  <h2> Prerequisites </h2>

- Create a Virtual Machine in Azure
- Install osTicket v1.15.8
- Install PHP
- Install Rewrite
- Install Microsoft Visual C ++
- Install MySQL
  
  <h2>Steps</h2>
<h2 align="center">Step 1: Create Virtual Machine in Azure</h2>
<br />
<p>
<h3>First, start by creating a Virtual Machine</h3>
<br />
</p>
<p>
  
![image](https://github.com/user-attachments/assets/0a93218b-d290-4308-961c-830c37fabf47)
![image](https://github.com/user-attachments/assets/68698e4b-dc2a-42c7-9d18-a38c8c4891bd)
![image](https://github.com/user-attachments/assets/14c854f3-25ed-4027-accb-70807ce0d771)



</p>
<p>
  
- Name Resource Group Ex: osTicket
- Name Virtual Machine Ex: osTicket-vm
- Select Region
- Select image Windows 10 Pro
- Select Size (of atleast 2vpcus)
- Create Username/Passowrd (Place in notepad, wordpad, etc.)
- Check Licensing box
- Review and Create
- CreatE
- Copy Public I.P. Address
<br />

<h2 align="center">Step 2: Open your Remote Desktop Connection app on your computer and connect to your Virtual Machine that was created in Azure. </h2>
<br />
<p>
  
![image](https://github.com/user-attachments/assets/af54e5cc-07c7-485d-ba20-aa61434753de)

- Paste Public I.P. Address
</p>
<br />

  
<h2 align="center">Step 3: Now we need to install / Enable IIS in Windows </h2>
<br />
<p>
  
![image](https://github.com/user-attachments/assets/de8140bd-1b30-4fcb-a9e1-65fb7116e875)
<img src="https://i.imgur.com/iB0DDRd.png" height="75%" width="100%" />

- Go to your "Control Panel"
- Click "Programs" > "Turn Windows features on or off"
- Scroll down to "Internet Information Services (IIS)" Expand it</p>
- World Wide Web Services
- Application Development Features
- CGI
- OK
<br />
<br />
<h2 align="center">Step 4: Files You Need to Download</h2>

![image](https://github.com/user-attachments/assets/6b70498d-054b-4436-91d0-9a70e20cf950)

- ### [Download Now](https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6) 📁
<br />

![image](https://github.com/user-attachments/assets/7f983bdc-0739-4bf0-8fd2-f128a8ec446e)

- Install PHP Manager
- Download the PHP manager file, and agree with all the terms. We've now downloaded the PHP manager into our operating system.

<p>
  
  ![image](https://github.com/user-attachments/assets/c4912e29-6373-4224-a10d-a976d77d6d39)

- Install Rewrite Module</h3>
- Download the Rewrite Module file, agree with all the terms and it should now be installed onto the Computer.

![image](https://github.com/user-attachments/assets/c92b05ab-11fc-48ac-8f2c-0cbb73f9db45)

- Create Directory C:\PHP
- Open another folder
- Go to Windows (C:)
- Right click > New > Folder
- PHP
<br />
<p>
<h2 align="center"> Step 5: Unzip "php-7.3.8-nts-Win32-VC15-x86.zip" into the "PHP" file
</h2>
<p>
  
![image](https://github.com/user-attachments/assets/64018344-5ad0-472a-96ee-bf40afe46560)
- Right click "php-7.3.8-nts-Win32-VC15-x86"
- Extract all
- Browse
- Windows C:
- PHP
- Select Folder
- Extract
</p>
<br/>
<h2 align="center">Step 6: Install VC_REDIST</h2>

![image](https://github.com/user-attachments/assets/69c4c857-38a9-41bf-9485-29e5b08898fb)
- Agree
- Install

<h2 align="center">Step 7: Install MySQL </h2>

![image](https://github.com/user-attachments/assets/820df876-071f-4868-9b22-d49096e2dd7f)

- Download and install MySQL
- Choose "Typical" Setup
- Install
![image](https://github.com/user-attachments/assets/651adb2a-f7ef-4b69-a3dc-8c5c887f24c0)

- Launch Configuration Wizard (after install)
- Standard Configuration

![image](https://github.com/user-attachments/assets/ffd5fb23-8c57-4ef3-875b-1092f8515b4e)

- Create a password
- Execute

- Agree with any terms and agreements up until you get to the password portion
-  Here you can create a username and password for the database that you'll be using to store the Ticket Information used in osTicket. 
</h3>
<p>
<h2 align="center">Step 8: Open IIS</h2>
  
![image](https://github.com/user-attachments/assets/8c318def-0e67-43d7-b7ea-1c00fc19055b)
![image](https://github.com/user-attachments/assets/fce7e876-dc39-4d70-81a7-7a760a647f32)

- Run as Admin
- Register PHP in IIS
- Go to PHP manager
- Register new PHP version
- Click the browse button (...)
- Windows C:
- PHP folder
- php-cgi
- OK
<br/>
<p>
<h2 align="center">Step 9:  Reload IIS</h2>

![image](https://github.com/user-attachments/assets/646eac80-e288-42b6-b812-9abdcf57b652)

- Open IIS
- Stop/Start the server
</p>  
<br /> 
<p>
  <h2 align="center">Step 10: Install osTicket v1.15.8</h2>

![image](https://github.com/user-attachments/assets/1b824c63-156c-4fa0-a368-386d68db4e91)

- Extract osTicket v1.15.8
</p>
<br />
<br /> 
<p>
  <h2 align="center">Step 11: Rename "upload" to "osTicket"</h2>

![image](https://github.com/user-attachments/assets/5eb77ebe-7c90-497f-8cb4-b6743e93ad89)
![image](https://github.com/user-attachments/assets/e40b1f3c-4ff1-4a89-bcab-4c04d0282d30)
![image](https://github.com/user-attachments/assets/c5e062fb-cf10-435f-96f8-d61962ef30c1)


- Windows C:
- inetpub
- wwwroot
- Copy "upload" folder into "wwwroot" folder
- Rename "upload" to "osTicket"
</p>
<br />
<p>
<h2 align="center">Step 12: Reload IIS</h2>

![image](https://github.com/user-attachments/assets/646eac80-e288-42b6-b812-9abdcf57b652)

- Open IIS
- Stop/Start the server
</p>  
<br />
<p>
<h2 align="center">Step 13:  Load osTicket Site</h2>

![image](https://github.com/user-attachments/assets/21c30cd0-75ca-418e-b06a-33ae218eeb79)

- Go to sites
- Default
- osTicket
- (On the right) click Browse *80
- " If you try to browse it and the website doesn't show up, you might have done something wrong."
</p>
<h2 align="center">Step 14: Enable Extensions in IIS: (Note that some extensions are not enabled)</h2>
<br />

![image](https://github.com/user-attachments/assets/af6c5fa5-9276-4251-b8ce-3f095de7ff46)

<p>
  
- Go back to IIS
- Sites 
- Default 
- osTicket
- Double click PHP Manager
- Enable php_imap.dill
- Enable php_intl.dill
- Enable php_opache.dill
- Referesh the osTicket site in your in your browser, observe the changes
</p>
<h2 align="center">Step 15: Rename ost-config.php</h2>
<br />
<p>
<h4>From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php.</h4>
<h4>To: C:\inetpub\wwwroot\osTicket\include\ost-config.php:</h4>
</p>
<p>
	
![image](https://github.com/user-attachments/assets/ab390899-dae3-4317-acd3-6df8212f8ac8)
- Windows C:
- inetpub
- wwwroot
- osTicket
- include
- Find "ost-sampleconfig.php"
- Right click it and rename to "ost-config.php" 
</p>
<br />
<h2 align="center">Step 16: Assign Permissions> ost-config.php</h2>
  
![image](https://github.com/user-attachments/assets/43d9e867-00ce-4a38-8e42-92a2ac0434cc)
![image](https://github.com/user-attachments/assets/518ffd3f-9d1a-4259-9a10-300abff0b9f4)
![image](https://github.com/user-attachments/assets/25528f4b-ff86-45ee-b557-4d7f97f15bf3)
![image](https://github.com/user-attachments/assets/1a9866b1-568e-4d7c-a5e9-aec983c0adc1)
![image](https://github.com/user-attachments/assets/d48ab9e2-5a41-4a8c-8057-4105a9777b98)
![image](https://github.com/user-attachments/assets/ba5ffa89-56cc-4873-811d-d495043af602)
![image](https://github.com/user-attachments/assets/258bd6d0-1634-4449-84f6-423200aa9728)

<p>
	
- Right click "ost-config.php"
- Go to properties
- Click on Security tab
- Advanced
- Disable inheritance 
- Remove all inherited permissions from this object:
- Add
- Select a principle
- Enter everyone
- Ok
- Check Full Control
- Ok
</p>
<br />

<h2 align="center">Step 17: Continue Setting up osTicket in the browser</h2>

![image](https://github.com/user-attachments/assets/4ee863d3-fa24-401a-985b-74d203d592d2)

<p>
	
- Go back to osTicket website
- Click continue
- Name Helpdesk
- Enter a default email (receives email from customers)
- Fill Admin User info.
</p>
<br />
<h2 align="center">Step 18: Download and Install HeidiSQL</h2>
<br />
<p>
	
![image](https://github.com/user-attachments/assets/f93be9ba-0092-4aec-b4e3-9b92048eec1a)
![image](https://github.com/user-attachments/assets/b8485626-6588-4e31-9abe-3a213c980a09)
![image](https://github.com/user-attachments/assets/0c6cefc1-e460-4f2f-92cc-0e7b000771f6)



</p>
<p>
	
- Go back to files
- Desktop
- osTicket-Installation
- Open Heidi
- Install
- "Make sure the checkbox for (Launch HeidiSQL) is selected before you hit finish"
- Skip
- New
- User: root
- Password: root
- Open (Your now connected to the session)
- Create a database called "osTicket"
- Right click "Unnamed"
- Create New
- Database
- Name: osTicket
</p>
<br />

<h2 align="center">Step 19: Continue Setting up osTicket in the browser</h2>

![image](https://github.com/user-attachments/assets/2b4dba82-343f-43f7-a643-b54ab6fcc409)


- MySQL Database: osTicket
- MySQL Username: root
- MySQL Password: root
- Click “Install Now!”
</p>
<br />
<h2 aligh="center">Step 20: Congratulations, hopefully it is installed with no errors!</h2>
<p>
	
![image](https://github.com/user-attachments/assets/8b8c9537-3c79-40dd-ad85-42da39e8ecfd)

<br />
<h2 align="center">Clean up (OPTIONAL)</h2>

<img src="https://i.imgur.com/eg0ZPG3.png" height="75%" width="100%" />
<img src="https://i.imgur.com/n6k46XL.png" height="75%" width="100%" />
<br />

- Delete: C:\inetpub\wwwroot\osTicket\setup:
- Set Permissions to “Read” only:
- C:\inetpub\wwwroot\osTicket\include\ost-config.php:


<h2 align="center">Login to the osTicket Admin Panel (http://localhost/osTicket/scp/login.php)</h2>
<br />
<p>
	
![image](https://github.com/user-attachments/assets/2a64a20d-77cf-4313-a745-bd709d951f56)

</p>
<br />

<h1 align="center"> Congratulations, you've finished installing osTicket!!!</h1>
