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

- Windows 10</b> (22H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Teams and Departments
- Configure Agents
- Configure SLA
- Create Help Topics

<h2>Configuration Steps</h2>

<p>
<img width="607" alt="image" src="https://github.com/jaydcollins/post-install-config/assets/164976272/d2b32801-5292-49a9-a320-285d67be1173">
</p>

- To configure roles, go to: Admin Panel > Agents > Roles. Add role. Name it and enable all ticket permissions.

<br />

<p>
<img width="703" alt="image" src="https://github.com/jaydcollins/post-install-config/assets/164976272/78989986-2ce9-4342-ae8c-58de626448df">
</p>

- Go to Admin Panel > Agents > Departments -> Add New Departent. Name the department and select a manager.
- Click "Creat Dept".
- Next, go to Admin Panel -> Agents -> Teams.
- Select "Add team".
- Name it "Level II Support" and add member by clicking on "Members" tab.
- Go to Admin Panel > Settings > User Settings to make sure that the registration required box is not checked.

<br />

<p>
<img width="617" alt="image" src="https://github.com/jaydcollins/post-install-config/assets/164976272/3c923c92-bc6f-402c-990f-78daca0ccb7e">
</p>

-Time to create some agents and managers!
- Go to Admin Panel -> Agents and click "Add new agent".
- Create name and email.
- Press the set password button.
- Deselect the "Send the agent a password reset" box and create a password.
- Deselect the "require password change" box and press "set".
- Click on "Access" tab and select "System Administrators".
- Also select the department you created. In extended access below, select the department you created and add "support" department as well.
- Next, click on "teams" tab and select the team you created.
- Click "Create".
- Add another agent with limited permissions.
- To create users, go to Agent Panel > Users > and click on "Add user".
- Create name, email and password.
- Click "Add User".

<br />
<p>
<img width="598" alt="image" src="https://github.com/jaydcollins/post-install-config/assets/164976272/61607b38-b52f-4d7d-924f-fd6b96e6d472">
</p>

- Go to Admin Panel > Manage > SLA and click "add new SLA plan". 
- Place these settings for Sev-A: (1 hour, 24/7). 
- Sev-B will be (4 hours, 24/7)
- Sev-C will be (8 hours, Monday - Friday).

<br />

<p>
<img width="604" alt="image" src="https://github.com/jaydcollins/post-install-config/assets/164976272/ecd77a4f-54d9-4f38-a7b9-9eac235bc046">
</p>

- Go to Admin Panel > Manage > Help Topics and click "Add help topic".
- Title the first one "Business Critical Outage", the second "Personal Computer Issues", the third "Equipment Request", and lastly "Password Reset".
- Log into the user portal of osTicket at: http://localhost/osTicket/.
- Use a user you created to create tickets.


<br />

<h2 align="center"> Nice work! OsTicket is configured and ready for tickets. </h2>
