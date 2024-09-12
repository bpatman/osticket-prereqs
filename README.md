<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source helpdesk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

<ul>
<li>Microsoft Azure</li>
<li>Virtual Machine</li>
<li>osTicket Installation Files</li>
</ul>

<h2>Installation Steps</h2>

<p>
<h3>Step 1: Use Microsoft Azure to create a Virtual Machine.   Use Remote Desktop in the created Virtual Machine.</h3>

- Sign for a free Microsoft Azure account.  You will need a credit card to sign up.  Use this link [Microsoft Azure](https://azure.microsoft.com/en-us/free)

<h3>Step 2: Enable Internet Information Services (IIS) and Fast CGI</h3>

- Use the search bar to search for Control Panel
- Open Control Panel and select Uninstall a Program
- On the left side of the screen, click Turn Windows Features On or Off
- Select Internet Information Services (IIS)
- Expand the IIS folder by clicking the plus sign
- Next, expand the World Wide Web Services folder
- Next, expand the Application Development Features folder
- Select CGI
- Click OK


<p align="center">
<img src="https://github.com/user-attachments/assets/df05c4ca-6f2f-4181-adb1-9caeb9eb5cda" height="80%" width="80%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/aa8d62fe-4ec0-4574-9286-4a03ad8ee9f5" height="80%" width="80%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/5cf96937-c386-43f4-8c5e-239b8ec30f57" height="80%" width="80%" alt="Azure Free Account"/> 
</p>


<h3>Step 3: Download and Install Installation Files
</h3>

- Click here for the installation files [link](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)

- Download PHP Manager for IIS
- Install PHP Manager

<p align="center">
<img src="https://github.com/user-attachments/assets/f61a37a5-dc2c-44d0-8116-b5ae145d4e8f" height="80%" width="80%" alt="Azure Free Account"/> 
</p>

- Download "Rewrite Module
- Install "Rewrite Module"

<p align="center">
<img src="https://github.com/user-attachments/assets/8dd9d230-99ce-4df5-b2de-62d8bef30128" height="80%" width="80%" alt="Azure Free Account"/> 
</p>

- Open File Explorer
- Click on Drive C:
- Right Click > New > Folder
- Name the folder "PHP"

<p align="center">
<img src="https://github.com/user-attachments/assets/f1dd6ef7-8f69-4884-88c9-2c5dcf65c5a0" height="80%" width="80%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/2fc16716-fa5f-46ec-8388-ac322483538f" height="80%" width="80%" alt="Azure Free Services"/>
<img src="https://github.com/user-attachments/assets/b282bf0a-3f38-4def-9ca4-d4af50d184aa" height="80%" width="80%" alt="Azure Free Services"/>
<img src="https://github.com/user-attachments/assets/496cce62-88c4-44ff-826e-39978e8fccdf" height="80%" width="80%" alt="Azure Free Services"/>
</p>

- Download "PHP 7.3.8"
- Unzip/Extract "PHP 7.3.8" to "PHP" folder that was just created

<p align="center">
<img src="https://github.com/user-attachments/assets/f244d199-8e5b-4f75-8ca4-398dc4d19ff7" height="80%" width="80%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/2f1f75bc-18c5-439a-b694-79ff3f434807" height="80%" width="80%" alt="Azure Free Services"/>
<img src="https://github.com/user-attachments/assets/7bf38212-e0e8-4a9b-8ed5-6c14f80dba6f" height="80%" width="80%" alt="Azure Free Services"/>
<img src="https://github.com/user-attachments/assets/592b6f0c-cf98-4816-beff-c98c26554ec4" height="80%" width="80%" alt="Azure Free Services"/>
<img src="https://github.com/user-attachments/assets/ba91ac6f-619e-4ff5-bd77-35f9114a6d9f" height="80%" width="80%" alt="Azure Free Services"/>
</p>

- Download and install "VC_redist_x86.exe"

<p align="center">
<img src="https://github.com/user-attachments/assets/c386e46c-e724-4ed1-980d-e4afcf127997" height="80%" width="80%" alt="Azure Free Account"/> 
</p>

- Download "MySQL"
- Install "MySQL" > Choose Setup Type "Typical" 
- Once installation is done click Finish

<p align="center">
<img src="https://github.com/user-attachments/assets/364ba34b-5270-401a-a91d-e121e8da22a2" height="80%" width="80%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/e3d645cb-d5e0-4e93-8793-5a72c7f5ba8d" height="80%" width="80%" alt="Azure Free Services"/>
</p>

- On MySQL Server Instance Configuration Wizard 
- Click Next > Standard Configuration > Next > set both user and password as "root" then click next > Execute > Finish

<p align="center">
<img src="https://github.com/user-attachments/assets/abfdaf2b-c724-427f-9a75-ae23e921a081" height="80%" width="80%" alt="Azure Free Services"/>
<img src="https://github.com/user-attachments/assets/2c55f7e1-29ba-4b37-9b18-40e6a6ad6795" height="80%" width="80%" alt="Azure Free Services"/>
</p>

- Open Internet Information Services (IIS) Manager as administrator
- Register PHP from IIS
- Open PHP Manager > click Register new PHP version > click 3 dots to browse for folder > C:\PHP > php-cgi.exe > click OK
- Go back to osTicket home

<p align="center">
<img src="https://github.com/user-attachments/assets/7c801809-e9d5-4d86-95bc-0063eb2b832b" height="80%" width="80%" alt="Azure Free Services"/>
<img src="https://github.com/user-attachments/assets/af62f3cb-6547-47bc-b09c-6f406cfbd717" height="80%" width="80%" alt="Azure Free Services"/>
<img src="https://github.com/user-attachments/assets/a1c45608-6eef-40df-b2cf-0279f9936f5e" height="80%" width="80%" alt="Azure Free Services"/>
<img src="https://github.com/user-attachments/assets/4cdafa30-2ac6-46fc-9039-e2f48a93db67" height="80%" width="80%" alt="Azure Free Services"/>
</p>

- Reload IIS (Stop and the Start the Server)
- On the top right of the screen look for Manage Server
- Stop the Server (wait for it to finish)
- Start the Server


<p align="center">
<img src="https://github.com/user-attachments/assets/c36f4e68-2855-47c6-bee4-a08042a98171" height="70%" width="70%" alt="Azure Free Account"/> 
</p>


<h3>Step 4: Install osTicket v1.15.8</h3>
     
- Download osTicket: [link](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)
- Right-click on the file and select Extract All
- Open the new osTicket folder
- Copy the "Upload" folder into C:\inetpub\wwwroot
- Rename “Upload” to “osTicket”


<p align="center">
<img src="https://github.com/user-attachments/assets/e1549f06-7758-4662-9d1b-2819a34bd0ff" height="80%" width="80%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/e9f90fa7-0ea2-415a-b226-1a9e48b2ed9f" height="80%" width="80%" alt="Azure Free Services"/>
<img src="https://github.com/user-attachments/assets/10e9b336-7852-4569-a69e-09a7a3b5604f" height="80%" width="80%" alt="Azure Free Services"/>
</p>
 
     
<h3>Step 5: Restart the IIS Server</h3>

- Search for Internet Information Services (IIS) and select Open
- Select Restart on the right-hand side 
- On the left side of the screen, select Virtualmachine --> Sites --> Default Website --> osTicket
- On the right side of the screen, click “Browse *:80”
- This should open osTicket in your web browser


<p align="center">
<img src="https://github.com/user-attachments/assets/c36f4e68-2855-47c6-bee4-a08042a98171" height="70%" width="70%" alt="Azure Free Account"/> 	
<img src="https://github.com/user-attachments/assets/025dbadc-d361-413c-95de-ca81dc8e2bfe" height="80%" width="80%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/6f926762-52b3-495a-849f-95c7d9901c3a" height="80%" width="80%" alt="Azure Free Services"/>
</p>

<h3>Step 6: Enable Extensions in IIS</h3>

- Go back to IIS --> Sites --> Default Web Site --> osTicket
- Double-click PHP Manager
- Click “Enable or Disable an Extension” at the bottom of the screen under PHP Extensions
- Right-click and enable the following
- php_imap.dll 
- php_intl.dll
- php_opcache.dll

  
<p align="center">
<img src="https://github.com/user-attachments/assets/7fc49c22-00fb-43dc-b1c8-99646c3e27b0" height="80%" width="80%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/70419adc-4655-4397-b721-11e8d810739d" height="80%" width="80%" alt="Azure Free Services"/>
</p>

<h3>Step 7: Refresh the osTicket Site in Your Browser</h3>

- Refresh the osTicket site and observe the change
- Intl Extension should now have a green checkmark next to it


<p align="center">
<img src="https://github.com/user-attachments/assets/9db3e3bd-3171-41bf-ba0a-f2ab40a06133" height="80%" width="80%" alt="Azure Free Account"/>



<h3>Step 8: Rename</h3>
 
- Open Windows Explorer and select C: > inetpub > wwwroot > osTicket > include
- Rename the following file:
- From: ost-SAMPLEconfig.php
- To: ost-config.php


<p align="center">
<img src="https://github.com/user-attachments/assets/2d320b57-73e8-4cd2-9c57-61adb9b913ce" height="80%" width="80%" alt="Azure Free Account"/>

<h3>Step 9: Assign Permissions to ost-config.php</h3>

- Right-click ost-config.php 
- Open Properties --> Security --> Advanced --> Permissions 
- Select Disable Inheritance > Remove all inherited permissions from this object 

<p align="center">
<img src="https://github.com/user-attachments/assets/7cde479b-e341-4a64-8794-1aef02773ac7" height="80%" width="80%" alt="Azure Free Account"/>

- Afterwards, select Add --> select Principal --> type in "everyone" --> select Check Names --> select OK
- Allow everyone full control (check all boxes) --> Select apply --> OK

<p align="center">
<img src="https://github.com/user-attachments/assets/4189be1d-61f1-4a5b-899a-d593e0652365" height="70%" width=70%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/cb0caf3d-6970-4396-91d4-eec8bbb9e16e" height="80%" width="80%" alt="Azure Free Services"/>
</p>

  
<h3>Step 10: Continue Setting Up osTicket in Browser</h3>

- Go back to the browser and click Continue
 - Name: Helpdesk
- Email: any email you choose
- First Name: your first name
- Last Name: your last name
- Email Address: use a different email than the one used for Helpdesk
- Create a Username and Password
  
<p align="center">
<img src="https://github.com/user-attachments/assets/20dcfec2-bd54-42a8-892d-d56ff1f22f27" height="80%" width="80%" alt="Azure Free Account"/>

<h3>Step 11: Download and Install HeidiSQL</h3>

- Installation Files [link](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)
- Download and install HeidiSQL
- Open HeidiSQL 
- Select New
- Create Username and Password
- Select Open
- On the left side, right-click Unnamed --> select Create New --> Database
- Name it “osTicket” and select OK

<p align="center">
<img src="https://github.com/user-attachments/assets/2297600d-c42e-44f2-b429-a234453e150c" height="70%" width="70%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/ffaf2f36-d3e1-407e-96d3-82a4575f4f07" height="70%" width="70%" alt="Azure Free Services"/>
<img src="https://github.com/user-attachments/assets/f6de61f9-2744-473f-93b8-b7b91ab073f7" height="70%" width="70%" alt="Azure Free Services"/>
</p>

<h3>Step 12: Continue Setting Up osTicket by Filling Out the Fields</h3>

- Go back to the browser
- MySQL Database: osTicket (the one you just created in HeidiSQL)
- Create a Username and Password
- Finally, click Install Now

<p align="center">
<img src="https://github.com/user-attachments/assets/7b497a19-b39f-4bae-9d8d-8c7a53b3e24b" height="80%" width="80%" alt="Azure Free Account"/>
</p>

A congratulations screen should display in the browser window.  Clients should be available to create help desk tickets.  This concludes the lab.  

<p align="center">
<img src="https://github.com/user-attachments/assets/8a8fd34d-19cf-46f9-aefa-35c0c0aed36d" height="80%" width="80%" alt="Azure Free Account"/>


<h3>Step 13: Post-Installation Cleanup</h3>

- Go to C: > inetpub --> wwwroot --> osTicket --> Setup
- Delete the contents in the Setup folder
- Afterwards, delete the Setup folder
- Go to C: > Inetpub --> wwwroot --> osTicket --> Include
- Right-click on ost-config.php 
- Select Securities --> Advanced --> Click on "everyone" --> edit to change permissions
- Allow everyone to only have "Read and execute" permission, then select OK > Apply > OK
	
<p align="center">
<img src="https://github.com/user-attachments/assets/afb44c25-b93e-41b1-ae0a-18c2b75a90c6" height="70%" width="70%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/5d0a9216-b4ab-471b-97d2-27526c723a6f" height="70%" width="70%" alt="Azure Free Services"/>
</p>	


