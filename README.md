<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Prerequisites</h2>

- [osTicket: Prerequisites and Installation](https://github.com/norbelcasasmurillo/osticket-prereqs)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Allow Anyone To Create Tickets
- Configure Agents
- Configure Users
- Configure Service Level Agreements (SLA)
- Configure Help Topics

<h2>Configuration Steps</h2>

<p align="center">

  Log in using: 
- **Username:** adminuser
- **Password:** Password1
- **Admin/Analyst Login Page:** http://localhost/osTicket/scp/login.php 

</p>
<p>

![image](https://github.com/user-attachments/assets/29053156-5908-4f52-9552-f422866984d8)
</p>
<br />

<p align="center">
  
Open this link to have this ready when you need it later.
- **End Users osTicket URL:** http://localhost/osTicket 

</p>
<p>

![image](https://github.com/user-attachments/assets/d3d7d0df-56b0-4dd7-9073-cfda28eefb42)
</p>
<br />

<h3 align="center"> Configure Roles </h3>
<p align="center">
In order to configure roles (for grouping permissions), go to Admin Panel -> Agents -> Roles (Then click Add New Role). Type "Supreme Admin".

</p>
<p>

![image](https://github.com/user-attachments/assets/06b83ca2-d7af-4c71-b913-1ec841ab5487)
![image](https://github.com/user-attachments/assets/97a1254c-e69a-487a-a718-34c9c0418ce4)

</p>
<br />

<p align="center">
Then click on Permissions, then check everything. (In Tickets, Tasks, and Knowledgebase). Then click "Add the Role".

</p>
<p>

![image](https://github.com/user-attachments/assets/fd579eb3-ea19-448a-8469-9a58f9a66c90)
</p>
<br />

<h3 align="center"> Configure Departments </h3>
<p align="center">
To configure departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking), go to Admin Panel (You are already here from the previous steps) -> Agents -> Departments (Then click Add New Department)

</p>
<p>

![image](https://github.com/user-attachments/assets/cb6f5732-1b0f-4fcb-852f-95e3421ad74c)
</p>
<br />

<p align="center">

- **Parent:** Top Level Department
- **Name:** SysAdmins 
- **Schedule:** Monday - Friday 8am - 5pm with US Holidays

Leave all the other setting options alone, and then click Create Dept at the bottom of the page.

</p>
<p>

![image](https://github.com/user-attachments/assets/4ce71a8e-6eb8-4149-84c3-7ef0f33d4101)

</p>
<br />

<h3 align="center"> Configure Teams </h3>
<p align="center">
In order to configure Teams, go to Admin Panel (you are already there) -> Agents -> Teams. Then click Add New Teams.

</p>
<p>

![image](https://github.com/user-attachments/assets/bab7d030-d71f-4339-8d54-81ddb3d4fe62)


</p>
<br />

<p align="center">
Name the new team "Online Banking", then click "Create Team" at the bottom. 

</p>
<p>

![image](https://github.com/user-attachments/assets/fed34035-f51a-4fcd-9a5e-3b106729949e)

</p>
<br />

<h3 align="center"> Allow Anyone to Create Tickets  </h3>
<p align="center">
In order to allow anyone to create tickets, go to Admin Panel -> Settings -> User Settings (Uncheck this box: Require registration and login to create tickets). Then click "Save Changes" if this wasn't already saved. 

</p>
<p>

![image](https://github.com/user-attachments/assets/f2429016-8c5d-4720-9802-ae0f50c268ea)

</p>
<br />

<h3 align="center"> Configure Agents </h3>
<p align="center">
In order to configure Agents (workers), go to Admin Panel -> Agents -> Add New Agent.

</p>
<p>

![image](https://github.com/user-attachments/assets/8298ab6f-446d-4468-9200-5e1d1d340fb8)

</p>
<br />

<p align="center">

- **Name:** Jane Doe
- **Email:** Jane@lognpacific.com
- **Username:** jane 

</p>
<p>

![image](https://github.com/user-attachments/assets/670a03c1-b526-4448-8f63-a021208566c5)
</p>
<br />

<p align="center">
Click on the Access tab. Then for primary department choose Sysadmins and Supreme Admin.

</p>
<p>

![image](https://github.com/user-attachments/assets/73773e7c-c8f8-493a-bc8e-a01b68e24661)
</p>
<br />

<p align="center">
Click on the teams tab, then for assigned teams select Online banking. Then click the "Create" button. 

</p>
<p>

![image](https://github.com/user-attachments/assets/e715f423-7904-487f-b060-4f5d387846e6)
</p>
<br />

<p align="center">
Also, to add a new agent name. Go back to Admin Panel -> Agents -> Add New Agent.

</p>
<p>

![image](https://github.com/user-attachments/assets/8c2f53fe-dd12-43f9-89e1-d4272fc0e932)

</p>
<br />

<p align="center">
(Same steps for creating the first agent)

- **Name:** John Doe
- **Email:** John@lognpacific.com
- **Username:** john
- **Primary department:** Support and View Only
- **Team:** Select none
- Then click the "Create" button. 
</p>
<p>

![image](https://github.com/user-attachments/assets/01961733-bdc8-4f90-8031-0379583fb6f0)

</p>
<br />

<p align="center">
Go back to the agents panel. Click on Agent Jane to setup her password. Then click on "Set Password". 

</p>
<p>

![image](https://github.com/user-attachments/assets/0dd487bd-7fc7-4b88-8080-fa0128ae90e0)
![image](https://github.com/user-attachments/assets/ab660dc0-dd61-47af-abe1-1d4a597bd5b8)

</p>
<br />

<p align="center">

Uncheck the "Send the agent a password reset email" box. Then for the password put **Password1**. Also, uncheck the "Require password change at next login" box. Then click update. Do this process for Agent John as well. 

</p>
<p>

![image](https://github.com/user-attachments/assets/e395be99-98cd-4db4-97ff-37e45ac00ea1)


</p>
<br />

<h3 align="center"> Configure Users (customers) </h3>
<p align="center">
Next, in order to configure Users (customers), go to Agent Panel -> Users -> Add New.

</p>
<p>

![image](https://github.com/user-attachments/assets/1e2033b8-9e70-4c7f-9441-2e0ec8ef8c66)
![image](https://github.com/user-attachments/assets/f7806475-f6a4-4062-bf68-684b6f261d15)

</p>
<br />

<p align="center">

- **Name:** Karen
- **Email:** karen@lognpacific.com
- Then click "Add User"

</p>
<p>

![image](https://github.com/user-attachments/assets/de927a3e-7a4f-4591-a263-7c7b4c0c0a87)
</p>
<br />

<p align="center">
Click the User tab again, and click "Add User"

- **Name:** Ken
- **Email:** ken@lognpacific.com
- Then click "Add User"

</p>
<p>

![image](https://github.com/user-attachments/assets/f7806475-f6a4-4062-bf68-684b6f261d15)
![image](https://github.com/user-attachments/assets/cbabb4bc-d285-4e6a-a736-45dca7feb24b)
</p>
<br />

<h3 align="center"> Configure Service Level Agreement (SLA) </h3>
<p align="center">
In order to configure SLA, go to Admin Panel -> Manage -> SLA. Then click Add New SLA.

</p>
<p>

![image](https://github.com/user-attachments/assets/18e017a5-15ee-4fe6-b946-a9fcea9657ff)

![image](https://github.com/user-attachments/assets/03c99db1-4620-40bf-beb7-ceea6c26191d)

</p>
<br />

<p align="center">

- **Name:** Sev-A
- **Grace Period:** 1 hour
- **Schedule:** 24/7
- Then click "Add Plan"
</p>
<p>

![image](https://github.com/user-attachments/assets/bac237bc-9529-41bd-bacf-af5eee674ed9)
</p>
<br />

<p align="center">
Then, click on Add New SLA again. This time put: 

- **Name:** Sev-B 
- **Grace Period:** 4 hours
- **Schedule:** 24/7
- Then click "Add Plan"

</p>
<p>

![image](https://github.com/user-attachments/assets/613a0f54-e6e8-40f2-a509-b616cbc52292)

</p>
<br />

<p align="center">
Then, click on Add New SLA again. This time put: 

- **Name:** Sev-C 
- **Grace Period:** 8 hours
- **Schedule:** Business Hours (Monday - Friday 8am - 5pm with US Holidays)
- Then click "Add Plan"

</p>
<p>

![image](https://github.com/user-attachments/assets/eed708cf-f4e3-4da1-8cdd-f9d55afb1ba7)

</p>
<br />

<h3 align="center"> Configure Help Topics </h3>
<p align="center">
Next, in order to configure Help Topics (For when users create a ticket), go to Admin Panel (you are already there) -> Manage -> Help Topics. Then click Add New Help Topic. 

</p>
<p>

![image](https://github.com/user-attachments/assets/a00b8506-abe4-4e91-b714-67be502071d8)
</p>
<br />

<p align="center">
Set it to:

- **Topic:** Business Critical Outage
- **Parent Topic:** Report a Problem
- Then click "Add Topic"

</p>
<p>

![image](https://github.com/user-attachments/assets/ef25b99a-13e7-4302-ad31-92f531f08fde)

</p>
<br />

<p align="center">
Add another Help Topic by clicking the Help Topic tab, then click on "Add New Help Topic" and set it to:
  
- **Topic:** Personal Computer Issues
- **Parent Topic:** Report a Problem
- Then click "Add Topic"

</p>
<p>

![image](https://github.com/user-attachments/assets/9077ebf9-87ef-4d49-8ce3-415ba61c6015)

![image](https://github.com/user-attachments/assets/fdbdc61f-abfc-48e4-ba6c-565cc18c7f22)

</p>
<br />

<p align="center">
Add another Help Topic by clicking the Help Topic tab, then click on "Add New Help Topic" and set it to:
  
- **Topic:** Equipment Request 
- **Parent Topic:** General Inquiry
- Then click "Add Topic
</p>
<p>

![image](https://github.com/user-attachments/assets/3da45c7a-5318-479a-98a1-b73ab2d30ec7)

![image](https://github.com/user-attachments/assets/f4b021c7-c672-4489-8ec9-c980a4e4eaba)

</p>
<br />

<p align="center">
Add another Help Topic by clicking the Help Topic tab, then click on "Add New Help Topic" and set it to:
  
- **Topic:** Password Reset 
- **Parent Topic:** Report a Problem
- Then click "Add Topic
</p>
<p>

![image](https://github.com/user-attachments/assets/e787a11b-e73d-4df2-9428-0e900ee0f07e)

![image](https://github.com/user-attachments/assets/3ec5cb25-7b58-40ab-acb8-8f173ce6a227)

</p>
<br />

<p align="center">
Add another Help Topic by clicking the Help Topic tab, then click on "Add New Help Topic" and set it to:
  
- **Topic:** Other 
- **Parent Topic:** General Inquiry
- Then click "Add Topic
</p>
<p>

![image](https://github.com/user-attachments/assets/4c45d4a9-2b50-419e-a9f8-9d59503fad8b)

![image](https://github.com/user-attachments/assets/954dfda4-251b-4e21-b7bc-e831576486b4)

</p>
<br />

<h3 align="center">Conclusion</h3>

<p align="center">
Great job! You've successfully configured osTicket on your Windows virtual machine. To avoid unnecessary charges, be sure to shut down the VM in Azure when you're not using it. Well done on completing this project!
</p>
