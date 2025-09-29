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

<h2> << Setup 4: Configure Teams  >> </h2>
<p>
<img width="963" height="365" alt="Step 4" src="https://github.com/user-attachments/assets/35c01c0e-86bf-40c6-a774-80f68269910b" />

</p>
<p>
  
-	We are going to create a Team in osTicket.
-	On the Admin Panel page, go to the "Agents" tab.
-	Select “Teams” then select “Add New Team”.


</p>
<br />

<p>
<img width="964" height="731" alt="Step 4a" src="https://github.com/user-attachments/assets/8d9bea70-b2be-404c-b5f9-1c501e343660" />


</p>
<p>
  
- Next, input the name "Online Banking" then select “Create Team”.


</p>
<br />

<p>
<img width="963" height="387" alt="Step 4b" src="https://github.com/user-attachments/assets/e888620f-b21c-48de-9cfb-1009afeb6508" />


</p>
<p>
  
- Go back to the Teams page and you will see your new team created.


</p>
<br />

<h2> << Setup 5: Allow anyone to set up tickets >> </h2>
<p>
<img width="962" height="737" alt="Step 5" src="https://github.com/user-attachments/assets/b94a56d6-4b45-4d3d-bd5b-7b38f9f1419f" />


</p>
<p>
  
- We are going to turn off the setting that requires registration and login for a user to create tickets.
- On the Admin Panel page, go to the "Settings" tab.
- Select “Users” and make sure that the “Require registration and log in to create tickets” box is checked off then select “Save Changes”.


</p>
<br />

<h2> << Setup 6: Configure Agents (Workers) >> </h2>
<p>
<img width="962" height="404" alt="Step 6" src="https://github.com/user-attachments/assets/599b8dfe-b415-46e7-aae9-3d8502fec79d" />


</p>
<p>
  
- We are going create 2 Agents. 1st one will have an Admin Role and the 2nd will have a Support role.
- On the Admin Panel page, go to the "Agents" tab.
- Select the secondary “Agents” tab and select “Add New Agent”.



</p>
<br />

<p>
<img width="963" height="495" alt="Step 6a" src="https://github.com/user-attachments/assets/44f25ed2-88d9-46af-ad29-52eb32dbb57d" />


</p>
<p>
  
- Input a Name, Email and Username. Then select “Set Password”.



</p>
<br />

<p>
<img width="651" height="393" alt="Step 6a1" src="https://github.com/user-attachments/assets/9f4ffd64-58d5-43d3-a443-0e42e7ab0729" />


</p>
<p>
  
- Next, input your password and make sure to uncheck “Send the agent a password reset email” and “Require password change at next login” then select “Set”.



</p>
<br />
<p>
<img width="962" height="628" alt="Step 6a2" src="https://github.com/user-attachments/assets/7417b51d-7602-4cdf-9e35-08790f8f4ad0" />


</p>
<p>
  
- Next, select the “Access” tab. For “Primary Department” we are going to select “SysAdmins” as the Department and select “Supreme Admin” as the Role.
- Next, for “Extended Access” we are going to select “Support” as the Department, then click “Add” and select “Supreme Admin” as the Role. 



</p>
<br />

<p>
<img width="963" height="478" alt="Step 6a3" src="https://github.com/user-attachments/assets/74268d8c-4825-4599-a88f-361034a98452" />


</p>
<p>
  
- Next, select the “Teams” tab. For “Assigned Teams” we are going to select “Online Banking” as the Team then click “Add” then select “Create”.



</p>
<br />

<p>
<img width="961" height="441" alt="Step 6a4" src="https://github.com/user-attachments/assets/600c5e10-1828-49a4-afe9-43d1f129764f" />



</p>
<p>
  
- Now select the “Agents” under the “Agents” tab and you will now see the new agent that we just created.



</p>
<br />

<p>
<img width="963" height="458" alt="Step 6b" src="https://github.com/user-attachments/assets/c13e81ed-ec96-4bb4-9e4f-f641277ffcdd" />


</p>
<p>
  
- Now for the 2nd Agent:
  - Do the same as before. Select “Add New Agent”.


</p>
<br />

<p>
<img width="963" height="496" alt="Step 6b1" src="https://github.com/user-attachments/assets/e60f803b-8efd-44e8-9da7-573669b4ced2" />



</p>
<p>
  
- Input a Name, Email and Username. Then select “Set Password”.


</p>
<br />

<p>
<img width="649" height="391" alt="Step 6b2" src="https://github.com/user-attachments/assets/9fc48943-c0f5-4d98-9f18-4b9e355607ed" />




</p>
<p>
  
- Next, input your password and make sure to uncheck “Send the agent a password reset email” and “Require password change at next login” then select “Set”.


</p>
<br />

<p>
<img width="963" height="592" alt="Step 6b3" src="https://github.com/user-attachments/assets/27b7354b-d171-4008-84d5-6aea25255133" />



</p>
<p>
  
- Next, select the “Access” tab. For “Primary Department” we are going to select “Support” as the Department and select “Expanded Access” as the Role. Then select “Create”.

</p>
<br />

<p>
<img width="964" height="461" alt="Step 6b4" src="https://github.com/user-attachments/assets/d20cf556-e05a-45ca-8b99-7a873a4c27a9" />



</p>
<p>
  
- Now select the “Agents” under the “Agents” tab and you will now see the new agent that we just created.


</p>
<br />

<h2> << Setup 7: Configure Users (Customers) >> </h2>
<p>
<img width="960" height="397" alt="Step 7" src="https://github.com/user-attachments/assets/0a4420ed-d3d6-4b6b-9447-3a10a81eedfa" />



</p>
<p>
  
- We are going create 2 Users:
  - On the Admin Panel page, go to the top right and select "Agent Panel". 



</p>
<br />

<p>
<img width="960" height="407" alt="Step 7a" src="https://github.com/user-attachments/assets/e012118d-6b26-422c-adf6-00aa594a1b38" />


</p>
<p>
  
- Then, select the “Users” tab and select “Add User”.


</p>
<br />

<p>
<img width="648" height="395" alt="Step 7a1" src="https://github.com/user-attachments/assets/d60909a6-5646-48f3-a852-db2164aef169" />


</p>
<p>
  
- Input an Email and Name. Then select “Add User”.


</p>
<br />

<p>
<img width="648" height="395" alt="Step 7a2" src="https://github.com/user-attachments/assets/e1fe150c-99dc-4240-abfa-e30acfc80330" />


</p>
<p>
  
- Repeat the same steps as above for a second user.


</p>
<br />

<p>
<img width="960" height="461" alt="Step 7a3" src="https://github.com/user-attachments/assets/287b0d0a-e086-46f4-97fc-37e43847c114" />


</p>
<p>
  
- Now select the “Users” tab and you will now see the new users that we just created.


</p>
<br />

<h2> << Setup 8: Configure SLA (Service Level Agreements) >> </h2>
<p>
<img width="960" height="358" alt="Step 8" src="https://github.com/user-attachments/assets/feda43e5-2037-4063-bbe0-4c1f7c6593c1" />


</p>
<p>
  
- The purpose of the SLA is to provide a length of time in which the help desk Administrator expects tickets to be closed.
- We are going to create 3 different SLAs.
  - Head to the Admin Panel in osTicket.
  - Select “Manage” then select “SLA” and select “Add New SLA Plan”.


</p>
<br />

<p>
<img width="960" height="714" alt="Step 8a" src="https://github.com/user-attachments/assets/72efb808-faf2-42fd-b365-19121dcca9c3" />


</p>
<p>
  
- For our first SLA, we are going to name it "SEV-A", with a grace period of “1” Hour and a “24/7” schedule.
- Then select “Add Plan”.
- This one will be the most urgent SLA plan of the 3.


</p>
<br />

<p>
<img width="960" height="723" alt="Step 8b" src="https://github.com/user-attachments/assets/40be8a76-d32e-4ae3-b5bf-0733d19c9a17" />


</p>
<p>
  
- Next for the 2nd SLA plan.
- Repeat the previous steps.
- We are going to name it "SEV-B", with a grace period of “4” Hours and a “24/7” schedule as well. Then select “Add Plan”.
- This one will be the 2nd most urgent SLA plan of the 3.



</p>
<br />

<p>
<img width="960" height="726" alt="Step 8c" src="https://github.com/user-attachments/assets/0982c7f0-4fbe-4a9e-914a-b02c1df0e744" />


</p>
<p>
  
- Next for the 3rd SLA plan.
- Repeat the previous steps.
- We are going to name it "SEV-C", with a grace period of “8” Hours and a “Monday-Friday from 8 am-5 pm with U.S. Holidays” schedule. Then select “Add Plan”.
- This one will be the 3rd most urgent SLA plan of the 3.



</p>
<br />

<p>
<img width="960" height="477" alt="Step 8d" src="https://github.com/user-attachments/assets/5fd02f1c-3d23-4cd6-bf8b-5c2dfc742429" />


</p>
<p>
  
- Now back to the SLA page, you will see all 3 of the SLA plans we have just created.


</p>
<br />

