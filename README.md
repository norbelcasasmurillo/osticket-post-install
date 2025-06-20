<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Configuration Steps</h2>

<p align="center">
Login using Username: adminuser ; Password: Password1 ; Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php 

</p>
<p>

![image](https://github.com/user-attachments/assets/66e151ed-cdc0-4794-986d-e7705ec3064b)
</p>
<br />

<p align="center">
Have this ready when you need it. End Users osTicket URL: http://localhost/osTicket 

</p>
<p>

![image](https://github.com/user-attachments/assets/154aadb7-eca7-43a8-a396-8ab1400300ed)
</p>
<br />

<p align="center">
In order to configure roles (for grouping permissions), go to Admin Panel -> Agents -> Roles (Then click Add New Role). Type "Supreme Admin".

</p>
<p>

![image](https://github.com/user-attachments/assets/edb98175-a779-4adc-a83e-de1692e6b481)
</p>
<br />

<p align="center">
Then click on Permissions, then check everything. (In Tickets, Tasks, and Knowledgebase). Then click "Add the Role".

</p>
<p>

![image](https://github.com/user-attachments/assets/33985605-7d8b-4254-9942-0bec6a4a66f8)
</p>
<br />

<p align="center">
To configure departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking), go to Admin Panel -> Agents -> Departments (Then click Add New Department, and type SysAdmins)

</p>
<p>

![image](https://github.com/user-attachments/assets/46775c18-6a41-436c-9c61-293776705d19)
</p>
<br />

<p align="center">
Choose the Top Level Department for parent and name it SysAdmin, then click Create Dept at the bottom of the page.

</p>
<p>

![image](https://github.com/user-attachments/assets/32e4681f-a9f2-46b3-bb81-46b595106aca)

</p>
<br />

<p align="center">
(Note: can make additional steps for the lab report for the course), then click "Add New Department". 

</p>
<p>

<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p align="center">
In order to configure Teams, go to Admin Panel -> Agents -> Teams (Pull Agents from different Departments).

</p>
<p>

![image](https://github.com/user-attachments/assets/c312d7fb-514b-4c05-a278-a1673be9c109)


</p>
<br />

<p align="center">
Click Add New Teams, name it Online Banking, then create it.

</p>
<p>

![image](https://github.com/user-attachments/assets/b7fcb73b-bc03-4ed9-b53f-dedeeb23ca29)

</p>
<br />

<p align="center">
In order to allow anyone to create tickets, go to Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets) (To check and make sure)
Registration Required: Require registration and login to create tickets

</p>
<p>

![image](https://github.com/user-attachments/assets/faddc9df-325c-4842-b111-565e8e0c7e56)

</p>
<br />

<p align="center">
In order to configure Agents (workers), go to Admin Panel -> Agents -> Add New.

</p>
<p>

![image](https://github.com/user-attachments/assets/fa255269-bdf1-4e86-9ce8-8bf4d2488283)

</p>
<br />

<p align="center">
Name: Jane (Dept: SysAdmins) ; Email: Jane@lognpacific.com

</p>
<p>

![image](https://github.com/user-attachments/assets/2e5250f1-9feb-4a3f-b7b0-9fdf59ba7c01)
</p>
<br />

<p align="center">
Click on the Access tab. Then for primary department choose Sysadmins and Supreme Admin.

</p>
<p>

![image](https://github.com/user-attachments/assets/c7a763af-b290-42a3-8881-d4e11559089b)
</p>
<br />

<p align="center">
Click on the teams tab, then for assigned teams select Online banking. 

</p>
<p>

![image](https://github.com/user-attachments/assets/72656336-6366-410a-bd3e-0b2fb85a0d55)
</p>
<br />

<p align="center">
Also, add a new agent name: John (Dept: Support). Email: John@lognpacific.com ; Primary department: Support and View Only ; Assign to no team, then add agent.

</p>
<p>

![image](https://github.com/user-attachments/assets/fce4fff9-66e6-4b30-8057-82b0ef9d42b3)

</p>
<br />

<p align="center">
Set both of their passwords by updating it. (You need to click on each agent before updating password) (They don’t change their password when they login too.)

</p>
<p>

![image](https://github.com/user-attachments/assets/8dd385da-8d07-4068-8a17-0a74937a6a77)

</p>
<br />

<p align="center">
Next, in order to configure Users (customers), go to Agent Panel -> Users -> Add New.

</p>
<p>

![image](https://github.com/user-attachments/assets/e9bfdf7e-1623-44c6-88cf-ecf1655fd8ad)

</p>
<br />

<p align="center">
- **Name:** Karen
- **Email:** karen@lognpacfic.com


</p>
<p>

![image](https://github.com/user-attachments/assets/72f0e0ea-c821-46ab-becd-c2d1405fcfc5)
</p>
<br />

<p align="center">
- **Name:** Ken
- **Email:** ken@lognpacific.com

</p>
<p>

![image](https://github.com/user-attachments/assets/ae3b84f8-c575-4c72-b271-1fa61b0af397)
</p>
<br />

<p align="center">
In order to configure SLA, go to Admin Panel -> Manage -> SLA.

</p>
<p>

![image](https://github.com/user-attachments/assets/e265e577-bde3-4227-8d2e-3ec4552f55dd)

</p>
<br />

<p align="center">
Then click Add New SLA. And put it as Sev-A (Grace Period: 1 hour, Schedule: 24/7).

</p>
<p>

![image](https://github.com/user-attachments/assets/16ec9780-6bf6-408b-aecd-1e3d362ffa60)
</p>
<br />

<p align="center">
Then, click on Add New SLA again. This time put Sev-B (Grace Period: 4 hours, Schedule: 24/7).

</p>
<p>

![image](https://github.com/user-attachments/assets/6bfaed1f-ee1b-419e-8899-3ad23d6f8195)

</p>
<br />

<p align="center">
Then also add this one too. Sev-C (Grace Period: 8 hours, Business Hours).

</p>
<p>

![image](https://github.com/user-attachments/assets/25d3c7fc-a515-4e47-a33e-c9d200ebd479)

</p>
<br />

<p align="center">
Next, in order to configure Help Topics (For when users create a ticket), go to Admin Panel -> Manage -> Help Topics (Then click Add New Help Topics).

</p>
<p>

![image](https://github.com/user-attachments/assets/f840e070-6545-4082-bfec-381baca47218)
</p>
<br />

<p align="center">
Set it to Business Critical Outage (Report a Problem), then add.

</p>
<p>

![image](https://github.com/user-attachments/assets/40e82717-1098-4207-8f00-f6504c86424a)

</p>
<br />

<p align="center">
Add another Help Topic and sset it to Personal Computer Issues (Report a Problem).

</p>
<p>

![image](https://github.com/user-attachments/assets/aaf49d75-f0a4-4fb8-85dc-44669b24d937)

</p>
<br />

<p align="center">
Add another Help Topic. Set it to Equipment Request (General Inquiry).

</p>
<p>

![image](https://github.com/user-attachments/assets/7f656b8b-497e-422f-bb9e-3c3b114a4b8e)

</p>
<br />

<p align="center">
Add another Help Topic. Set it to Password Reset (Report a Problem).

</p>
<p>

![image](https://github.com/user-attachments/assets/9c765aa9-3e92-417b-8280-5defa013244e)

</p>
<br />

<p align="center">
Add another Help Topic. Set it to Other (General Inquiry)

</p>
<p>

![image](https://github.com/user-attachments/assets/3dc04ea1-1a3c-4582-9d59-4ccb19a155b8)

</p>
<br />
