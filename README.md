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
