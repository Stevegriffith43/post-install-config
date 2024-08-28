<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

<h3>The goal for the objectives below is to have a basic understanding of how these ticketing environments work
</h3>

- Configure Roles
- Configure Departments
- Configure Teams
- Demonstrate creating and editing tickets
- Configuring Users
- Configuring SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<h3>Configure Roles</h3>

<p>Roles define the permissions assigned to agents within specific departments they can access. Each role has a specific set of permissions that can be toggled on or off for agents assigned to that role and department. You can create and assign an unlimited number of roles to agents, allowing them access to different departments as needed.</p>

 - Admin Panel -> Agents -> Roles
 - "Supreme Admin" Role (A role to have complete control of every permission in the system)

 ![image](https://github.com/user-attachments/assets/e00e84dd-5e08-4d93-b510-d8e3a09f9834)
 ![image](https://github.com/user-attachments/assets/c30648ec-3d57-4058-a6d8-6ca483c6fe15)
 ![image](https://github.com/user-attachments/assets/44b1eaad-ae2f-48ff-adbf-9b41d7fd449e)

<br />

<h3>Configure Departments</h3>

<p>
Since tickets are routed through various departments in the help desk, numerous settings can be configured for each department.
</p>

- Admin Panel -> Agents -> Departments
- System Administrators

![image](https://github.com/user-attachments/assets/4a1e3e29-adf0-48e9-9756-3aebeee5f3a2)

<br />

<h3>Configure Teams</h3>

<p>
Teams let you organize agents from different departments to address specific issues or users using Help Topics or Ticket Filters. This setup overrides individual department rules, allowing specialized teams to handle specific tasks. To create a team, go to the Agents tab in your Admin Panel, click on Teams, and select Add New Team. You can then add agents and designate a team leader to receive separate alerts and notices.
</p>

- Admin Panel -> Agents -> Teams
- Level I Support
- Level II Support

![image](https://github.com/user-attachments/assets/5cce4755-8f00-4448-9f5a-3e1c4a713211)

<br />
