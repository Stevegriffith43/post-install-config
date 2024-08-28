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

<h3>Allowing anyone to create tickets</h3>

- Admin Panel -> Settings -> User Settings
- Registration Required: Require registration and login to create tickets

![image](https://github.com/user-attachments/assets/75a46cec-5bd4-456b-9aaa-932affd01a8f)

<br/>

<h3>Configure Agents</h3>

<p>Agents are granted access to the help desk to handle and resolve tickets. When adding an agent, they must be assigned a Primary Department and a Primary Role for handling tickets and tasks within that department. Additionally, agents can be granted Extended Access to other departments and assigned different roles for those areas. These settings can be adjusted in the Access tab of the agent’s profile.</p>

- Admin Panel -> Agents -> Add New
- Jane
- John

![image](https://github.com/user-attachments/assets/a42fa7f4-497b-4468-a1fb-a19225482aa9)

<br/>

<h3>Configure Users</h3>

<p>Users are the owners of tickets within the help desk. When a ticket is created, it is linked to the user’s email address found in the User Directory. Users can be added to or removed from the User Directory at any time. However, if a user is deleted, their associated tickets must also be removed.</p>

- Agent Panel -> Users -> Add New
- Karen
- Ken

![image](https://github.com/user-attachments/assets/1d2b8faf-8fa3-4623-b784-3f6385390939)

<br />

<h3>Configure SLA(Service Level Agreement)</h3>

<p>The SLA Plan sets the expected timeframe within which the help desk Administrator anticipates tickets will be resolved. Effectively a procedure, ruling, or guideline to complete tickets.</p>

- Admin Panel -> Manage -> SLA
- Sev-A (1 hour, 24/7)
- Sev-B (4 hours, 24/7)
- Sev-C (8 hours, business hours)

![image](https://github.com/user-attachments/assets/ad5e7be0-32d8-4b3f-b3ab-549eddb40ef5)

<br />

<h3>Configure Help Topics</h3>

<P>Help Topics streamline ticket management by ensuring tickets are routed to the correct department and addressed quickly. You can create and nest Help Topics for detailed categorization, such as Human Resources and Human Resources/Payroll. These topics also set ticket configurations, including the SLA and priority level. When creating new tickets, Help Topics must be chosen in both the client portal and for internal tickets, but users are not aware of the specific configurations linked to each Help Topic.</P>

- Configure Help Topics
- Admin Panel -> Manage -> Help Topics
- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset

![image](https://github.com/user-attachments/assets/f79557ac-ab1b-48fa-a21e-c9001fe1efd4)

<br />
