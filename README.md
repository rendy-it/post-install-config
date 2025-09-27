<p align="center">
<img width="2560" height="1440" alt="osTicket" src="https://github.com/user-attachments/assets/d181166e-76b0-4613-a8e7-6857158f5875" />

</p>

<h1>osTicket - Post-Installation Configuration</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Windows and Linux Virtual Machines on Microsoft Azure
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10 Pro </b> (21H2)

<h2>Post-Install Setup</h2>

-	Setup 1: Admin Panel & the Agent Panel
-	Setup 2: Configure Agent Roles
-	Setup 3: Configure Departments
-	Setup 4: Configure Teams
-	Setup 5: Allow anyone to create tickets.
-	Setup 6: Configure Agents (Workers)
-	Setup 7: Configure Users (Customers)
-	Setup 8: Configure SLA (Service Level Agreements)
-	Setup 9: Configure Help Topics


<h2>Configuration Steps</h2>

<h2> << Setup 1: Admin Panel & the Agent Panel >> </h2>
<p>
<img width="1155" height="827" alt="Step 0" src="https://github.com/user-attachments/assets/42848d88-a428-4325-900b-a91e6f937809" />



</p>
<p>
  
- Log into your Windows-VM, then log in osTicket. 

</p>
<br />
<p>
<img width="1154" height="566" alt="Step 0a" src="https://github.com/user-attachments/assets/84de02e9-1491-4983-b714-66cb1548a990" />


<p>
  
- Which will direct you to the Agent Panel.
- The Agent Panel is where you the worker is working the tickets.

  
</p>
<br />
<p>
<img width="963" height="407" alt="Step 1b" src="https://github.com/user-attachments/assets/93446a31-9cc7-430a-9f31-bf92e3cf258c" />


</p>
<p>
  
- Next, Click on the Admin Panel at the top right.


</p>
<br />
<p>
<img width="737" height="884" alt="Step 1b1" src="https://github.com/user-attachments/assets/19d6f19e-d9ae-4f32-8f7b-26932064e63e" />


</p>
<p>
  
- The Admin Panel is where you configure settings on the backend for osTicket.


</p>
<br />

<h2> << Setup 2: Configure Agent Roles >> </h2>

<p>
<img width="963" height="452" alt="Step 2" src="https://github.com/user-attachments/assets/b3b9875d-7a4f-4669-9be5-969458021d5d" />


</p>
<p>
  
- Once on the Admin Panel page, we are now going to create our osTicket role.
- We are going to create a Supreme Admin Role to give it lots of permissions. This is just an example as this is not normal in the work field.
- Go to the “Agents” tab. Select “Roles” then select “Add New Role”.




</p>
<br />
<p>
<img width="960" height="624" alt="Step 2a" src="https://github.com/user-attachments/assets/4c95b7a0-4fb0-40c4-af4e-21a47cba6dfc" />


<p>
  
- Next, input the name “Supreme Admin” then select “Permissions”.
   
</p>
<br />
<p>
<img width="964" height="761" alt="Step 2b" src="https://github.com/user-attachments/assets/add345fe-a9ba-495a-bd42-bc30f0524ae3" />


<p>
  
- Next, be sure to check every single permission for the “Tickets”, “Tasks” and “Knowledgebase” tabs then select “Add Role”.
   
</p>
<br />
<p>
<img width="963" height="501" alt="Step 2c" src="https://github.com/user-attachments/assets/1ef5f87c-3b52-478d-8da7-a20c80f9592b" />


<p>
  
- Now you have created your first Role as an Admin in osTicket.
   
</p>
<br />


<h2> << Setup 3: Configure Departments  >> </h2>
<p>
<img width="966" height="382" alt="Step 3" src="https://github.com/user-attachments/assets/df440bf5-544d-4634-8f1e-51e0f3924bb1" />

</p>
<p>
  
- We are going to create a department in osTicket.
- On the Admin Panel page, go to the "Agents" tab. 
- Select “Departments” then select “Add New Department”.


</p>
<br />

<p>
<img width="962" height="1168" alt="Step 3a" src="https://github.com/user-attachments/assets/2b44c302-cb77-4b8a-bf5f-f88534a7085a" />

</p>
<p>
  
- Next, input the name “SysAdmins” then select “Create Dept”.


</p>
<br />

<p>
<img width="963" height="435" alt="Step 3b" src="https://github.com/user-attachments/assets/fd33de3f-89ef-4065-94c5-d77891667511" />


</p>
<p>
  
- Now you have created your first Department in osTicket. 


</p>
<br />

<p>
<img width="1004" height="676" alt="Step 3c" src="https://github.com/user-attachments/assets/1ee9f1fd-78b2-4b51-8742-9dc942e91db3" />




</p>
<p>
  
- From the Installation Files folder on your Desktop:
  - Install the PHP Manager (PHPManagerForIIS_V1.5.0.msi).




</p>
<br />

<p>
<img width="1004" height="676" alt="Step 3d" src="https://github.com/user-attachments/assets/8c5efad0-d48e-4eb6-a669-606419bf90b9" />




</p>
<p>
  
- Next, in the installation files folder:
  -	Install the Rewrite Module (rewrite_amd64_en-US.msi).





</p>
<br />

<p>
<img width="792" height="394" alt="Step 3e" src="https://github.com/user-attachments/assets/ea59a03c-41f3-4e41-832d-7afb4b33ca86" />





</p>
<p>
  
- Next, we are going to create the directory C:\PHP :
  -	Go to your Windows (C:) drive and create a folder named “PHP”.






</p>
<br />

<p>
<img width="1185" height="751" alt="Step 3f" src="https://github.com/user-attachments/assets/9ea1a96a-ca47-4711-bfa6-ad6a71d73da9" />





</p>
<p>
  
- Now go back to the installation files folder and unzip the “php-7.3.8-nts-Win32-VC15-x86” zip file in to the PHP folder.



</p>
<br />
<p>
<img width="989" height="605" alt="Step 3g" src="https://github.com/user-attachments/assets/fb30b596-963f-4296-8a53-f114f5050c69" />



</p>
<p>
  
- Next, in the installation files folder:
  -	Install "VC_redist.x86".




</p>
<br />
<p>
<img width="1012" height="668" alt="Step 3h" src="https://github.com/user-attachments/assets/c50ecce9-952c-44f0-a691-f21b7909bbcb" />



</p>
<p>
  
- Next, in the installation files folder:
  - Install “MySQL 5.5.62” (mysql-5.5.62-win32.msi).
  - Select “Typical Setup”, then click Next.





</p>
<br />

<p>
<img width="357" height="271" alt="Step 3h1" src="https://github.com/user-attachments/assets/8a2b6bc6-11ca-413b-b13c-d1c22e67cfaa" /> <img width="69" height="271" alt="Right Pointing Arrow for Step 3h 1_2" src="https://github.com/user-attachments/assets/66e054cc-2d13-4456-b2f8-aaee676cb56a" /> <img width="357" height="271" alt="Step 3h2" src="https://github.com/user-attachments/assets/00f1cdf3-2e11-49ef-bf88-032cbcb84987" />







</p>
<p>
  
- Then the “Instance Configuration Wizard” window will appear.
- Select “Standard Configuration”, then click Next.






</p>
<br />
<p>
<img width="358" height="274" alt="Step 3h4" src="https://github.com/user-attachments/assets/b15dc0da-b3d2-4192-9b07-7a50f64bd022" /> <img width="69" height="271" alt="Right Pointing Arrow for Step 3h 1_2" src="https://github.com/user-attachments/assets/eeee5dc0-1d35-4375-ba0e-26da002003ea" /> <img width="358" height="274" alt="Step 3h5" src="https://github.com/user-attachments/assets/f3fb90e7-3d30-4ef3-a080-0fdeb5def206" />






</p>
<p>
  
- Select Next again, then create a username and password and make sure you do not forget it. Then click Next.
- Then, select “Execute”.


</p>
<br />
<p>
<img width="755" height="590" alt="Step 3i" src="https://github.com/user-attachments/assets/1893f77e-7c90-4dda-8e52-ed05b9404fb4" />




</p>
<p>
  
- Next, Open IIS as an Administrator.



</p>
<br />
<p>
<img width="1034" height="415" alt="Step 3i2" src="https://github.com/user-attachments/assets/be704377-40d6-4235-bbbe-0756104c26d7" />





</p>
<p>
  
- Next, double click on “PHP Manager”.



</p>
<br />
<p>
<img width="623" height="527" alt="Step 3i3" src="https://github.com/user-attachments/assets/058f9bf5-7318-4c5c-a42f-b0f111e74ac8" />






</p>
<p>
  
- Then, click on “Register new PHP version”.



</p>
<br />

<p>
<img width="510" height="220" alt="Step 3i4" src="https://github.com/user-attachments/assets/0ee3d8aa-bc8a-4713-bf3a-2d012549bce4" />





</p>
<p>
  
- Then, click on the 3 dots button “…” next to the path bar.



</p>
<br />
<p>
<img width="949" height="572" alt="Step 3i5" src="https://github.com/user-attachments/assets/73a65c30-e1c7-4cc7-a01d-a55a5af3b82a" />





</p>
<p>
  
- Then, go to the “PHP” folder that we created and select the “php-cgi” application file. Click open then click OK.



</p>
<br />
<p>
<img width="1063" height="371" alt="Step 3i6" src="https://github.com/user-attachments/assets/e9f375cb-d3da-4ec3-8eaf-cc6513198257" />




</p>
<p>
  
-	Then go back to the main interface and on the top right, click “Stop” then click on “Start”.



</p>
<br />

<h2> << Step 4: Install osTicket >> </h2>
<p>
<img width="1184" height="609" alt="Step 4" src="https://github.com/user-attachments/assets/2136e797-a7cc-4850-af6b-22aef6e18127" />


</p>
<p>
  
- Head back to the Installation Files folder on your Desktop.
  -	Right click on the “osTicket-v1.15.8” zip file and Extract all.
  -	In which it will create a folder named “osTicket-v1.15.8”.



</p>
<br />

<p>
<img width="282" height="287" alt="Step 4a" src="https://github.com/user-attachments/assets/df382abe-d665-452c-b927-068b31781da0" /> <img width="111" height="287" alt="Right Pointing Arrow for Step 4a_b" src="https://github.com/user-attachments/assets/be476924-9def-4803-b208-0562bbb8af09" /> <img width="282" height="287" alt="Step 4b" src="https://github.com/user-attachments/assets/303306e4-5854-4f93-8ebe-f9117eb525c0" />




</p>
<p>
  
- Next, open a new file explorer folder and head to this directory “C:\inetpub\wwwroot”.
- Then, head over to the “osTicket-v1.15.8” folder that we extracted earlier and copy the “upload” folder. 


</p>
<br />

<p>
<img width="282" height="287" alt="Step 4b1" src="https://github.com/user-attachments/assets/fba0a8cc-1b78-45c7-9fa2-bac35ffe3176" /> <img width="111" height="287" alt="Right Pointing Arrow for Step 4a_b" src="https://github.com/user-attachments/assets/3ec0fe5d-e35f-46c7-b68f-40198a902993" /> <img width="282" height="287" alt="Step 4b2" src="https://github.com/user-attachments/assets/0a15047c-fbc7-4aaa-a648-11bd64e18761" />




</p>
<p>
  
- Next, paste the “upload” folder into the “C:\inetpub\wwwroot” directory.
-	Then, rename it to “osTicket”.




</p>
<br />

<p>
<img width="1063" height="371" alt="Step 3i6" src="https://github.com/user-attachments/assets/f8441738-c677-4f29-b72a-fa665ce21eab" />



</p>
<p>
  
- Next, go back to the “IIS” main interface, and click “Stop” and then “Start”.


</p>
<br />

<p>
<img width="1021" height="374" alt="Step 4c" src="https://github.com/user-attachments/assets/ec3b24e5-1ee8-4e6e-8246-067171bcc0c6" />


</p>
<p>
  
- Then toggle down “Sites” and select “osTicket”.




</p>
<br />

<p>
<img width="1843" height="693" alt="Step 4c1" src="https://github.com/user-attachments/assets/d1f9b9c8-2b08-4f62-a3d5-e3d2ca8dcd45" />







</p>
<p>
  
- Select “Browse *80 (http)” which should then load osTicket into your web browser.
- You want to note that there are a few recommended extensions not present with the “X” symbol next to them. We will get some of them in the next few steps.







</p>
<br />

<p>
<img width="1034" height="415" alt="Step 3i2" src="https://github.com/user-attachments/assets/2629a6d3-3c30-4da7-a1e1-9697e423ea7c" />






</p>
<p>
  
- Next, go back to the “IIS” and double click on “PHP Manager”.



</p>
<br />
<p>
<img width="556" height="555" alt="Step 4d" src="https://github.com/user-attachments/assets/0216239e-489d-4f72-9b01-eef56df2b2a6" />



</p>
<p>
  
- Click on “Enable or disable an extension”




</p>
<br />
<p>
<img width="233" height="300" alt="Step 4d1" src="https://github.com/user-attachments/assets/974c7673-71be-4e0d-8b72-a247be337566" /> <img width="97" height="300" alt="Right Pointing Arrow for Step 4d1_d2" src="https://github.com/user-attachments/assets/a4226908-23cf-4a1c-9bbf-1c88a0c5b76a" /> <img width="233" height="197" alt="Step 4d2" src="https://github.com/user-attachments/assets/b96a01a5-5f4c-4567-8378-b0879907b322" />






</p>
<p>
  
- Then, you want to right click and enable “php_imap.dll”, “php_intl.dll” and “php_opcache.dll”.




</p>
<br />

<p>
<img width="765" height="594" alt="Step 4d3" src="https://github.com/user-attachments/assets/74cf3840-9ba1-43e7-b27e-c480d5a6a221" />



</p>
<p>
  
- Next, go back to osTicket in the browser and you want to reload the page. Then you will notice there are more extensions than before.  


</p>
<br />
<p>
<img width="855" height="482" alt="Step 4e" src="https://github.com/user-attachments/assets/38e5b9cc-af44-4f5c-8f50-9186ae67ea37" />



</p>
<p>
  
- Next, go to the folder that we renamed to “osTicket” which will put you to this directory “C:\inetpub\wwwroot\osTicket”


</p>
<br />
<p>
<img width="651" height="484" alt="Step 4e1" src="https://github.com/user-attachments/assets/ae7abb3b-4241-443d-be04-acf40780fed5" />




</p>
<p>
  
- Then, go to the “include” folder.
- Then, look for the file named “ost-sampleconfig.php”. 




</p>
<br />
<p>
<img width="635" height="484" alt="Step 4e2" src="https://github.com/user-attachments/assets/228e2024-7197-4eb4-9688-7f46a0be8993" />



</p>
<p>
  
- Then, rename it to “ost-config.php”.



</p>
<br />
<p>
<img width="320" height="253" alt="Step 4f" src="https://github.com/user-attachments/assets/e6529c6e-e465-47f1-a3b7-c1ff6a117c61" /> <img width="73" height="385" alt="Right Arrow for Step 4f_4f1" src="https://github.com/user-attachments/assets/757c29dc-fa48-4b4c-bd55-37c6fd85a887" /> <img width="276" height="385" alt="Step 4f1" src="https://github.com/user-attachments/assets/ae518866-ef20-4c88-8a06-0d3276ed225f" />



</p>
<p>
  
- Next, we are going to assign permissions to the “ost-config.php” file.
 - Right click it and select properties.
 - Then, select the “Security” tab and select Advanced.



</p>
<br />

<p>
<img width="585" height="395" alt="Step 4f2" src="https://github.com/user-attachments/assets/32b8a9c6-0d51-406a-988a-34f4f7e26d31" />


</p>
<p>
  
- Then, select “Disable Inheritance” and select Remove all.



</p>
<br />
<p>
<img width="261" height="395" alt="Step 4f3" src="https://github.com/user-attachments/assets/73f32fbe-acfa-4a16-98c2-22f430336435" /> <img width="61" height="395" alt="Right Arrow for Step 4f3_4f4" src="https://github.com/user-attachments/assets/8c148944-2215-40a4-a9f1-3c6254314ed7" /> <img width="262" height="395" alt="Step 4f4" src="https://github.com/user-attachments/assets/734e1408-0c81-4483-9e1c-53d20e2789d6" />





</p>
<p>
  
- Then, click on “Add” and then “Select a principal”.



</p>
<br />
<p>
<img width="453" height="247" alt="Step 4f5" src="https://github.com/user-attachments/assets/64b29821-e12c-4573-93bf-2f6bdb69f30e" />





</p>
<p>
  
- Then, type “Everyone” and click on Check Names which will then show “Everyone” underlined. Then press OK.



</p>
<br />
<p>
<img width="703" height="455" alt="Step 4f6" src="https://github.com/user-attachments/assets/a51159f1-1dd8-48c6-a5f7-0df453833c72" />



</p>
<p>
  
- Then, check the “Full Control” box then press OK.



</p>
<br />
<p>
<img width="588" height="399" alt="Step 4f7" src="https://github.com/user-attachments/assets/ab53d020-1cc5-4036-99b0-506ceae29a72" />



</p>
<p>
  
- Then click on Apply then click on OK to finish.




</p>
<br />
<p>
<img width="632" height="567" alt="Step 4g" src="https://github.com/user-attachments/assets/e2a4c136-8054-4778-a441-7f81783c1f0d" />


</p>
<p>
  
- Next, we are going to set up osTicket’s settings. 
  -	Go back to osTicket in the browser and select “ Continue >> ”.



</p>
<br />
<p>
<img width="631" height="618" alt="Step 4g1" src="https://github.com/user-attachments/assets/86bef592-9fec-4733-97e0-a56d60957598" />


</p>
<p>
  
- On the next page, fill out all the information. Make sure to use two different emails.


</p>
<br />
<p>
<img width="949" height="573" alt="Step 4h" src="https://github.com/user-attachments/assets/91d963e1-2476-48f3-a143-6e19a0460f91" />


</p>
<p>
  
- Next, head back to the osTicket Installation Files folder on your Desktop.
  -	Install “HeidiSQL_12.3.0.6589_Setup”.



</p>
<br />
<p>
<img width="689" height="484" alt="Step 4h1" src="https://github.com/user-attachments/assets/d5e0bbf4-a720-4335-a3be-b4ed2aa8715f" />



</p>
<p>
  
- Once installed, open it and select “New”.



</p>
<br />
<p>
<img width="690" height="486" alt="Step 4h2" src="https://github.com/user-attachments/assets/5d877c78-2f40-4fad-ae91-cbd3ac3a9157" />


</p>
<p>
  
- Then, input the username and password that you made earlier when you installed “MySQL 5.5.62” back in Step 3 and click Open.



</p>
<br />
<p>
<img width="939" height="596" alt="Step 4h3" src="https://github.com/user-attachments/assets/9dd76b2c-6e2f-4dfe-b3f7-873562d27809" />


</p>
<p>
  
- Then right click “Unnamed”, then “Create New”, then “Database”.



</p>
<br />
<p>
<img width="940" height="597" alt="Step 4h4" src="https://github.com/user-attachments/assets/1e851576-e92d-4068-a75a-e8eab323a231" />


</p>
<p>
  
- Then for the Database name, type in “osTicket” and click on Ok.



</p>
<br />
<p>
<img width="825" height="423" alt="Step 4i" src="https://github.com/user-attachments/assets/d76c476d-ba86-4126-9ed0-0424330f587f" />



</p>
<p>
  
- Next, head back to the web browser to continue setting up osTicket:
  - For “MySQL Database”, type in “osTicket”
  - For “MySQL Username”, type in the username you chose.
  - For “MySQL Password”, type in the password you chose.
-	Then click “Install Now”.




</p>
<br />
<p>
<img width="826" height="642" alt="Step 4j" src="https://github.com/user-attachments/assets/550e5119-ee1b-499e-9540-07d747a60a24" />


</p>
<p>
  
- Congratulations! You have now fully installed osTicket.


</p>
<br />
<p>
<img width="1155" height="827" alt="Step 4j1" src="https://github.com/user-attachments/assets/d3d53683-8061-4d2b-b605-a18b87b10f9b" />


</p>
<p>
  
- Next, you want to check and make sure your login works:
  -	Go to: http://localhost/osTicket/scp/login.php in the browser.
  -	Type in the Username and the password you made earlier for the osTicket settings. Then Clikc "Log In".



</p>
<br />
<p>
<img width="1154" height="566" alt="Step 4j2" src="https://github.com/user-attachments/assets/979c7046-42b6-48d5-9265-57be64fe9854" />


</p>
<p>
  
- Once logged in, this is what the page should look like.  

</p>
<br />

<h2> << Conclusion >> </h2>

<p>
  
- Close the Remote Desktop connection.
- Go Back to your Azure resource group page.
- Make sure your VMs are on “Stop” status if you are not going to use them right away. This way you will not be charged while they are not in use.
- Also, make sure your VMs are on “Stop” status if you are not going to use them right away. This way you will not be charged while they are not in use.
- To conclude, we have successfully installed osTicket inside our Windows Virtual Machine that is being resourced by the Azure cloud infrastructure. 


</p>
<br />



