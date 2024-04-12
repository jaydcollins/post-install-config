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

- Configure Roles
- Configure Teams and Departments
- Configure Agents
- Configure SLA
- Create Help Topics

<h2>Configuration Steps</h2>

<p>
<img src="https://github.com/kphillip1/post-install-config/assets/165929885/1170612b-aef9-4ab3-bfd6-b60be0fa30d5" height="80%" width="80%"/>
</p>

- To configure roles, go to: Admin Panel > Agents > Roles. Add role. Name it and enable all ticket permissions.

<br />

<p>
<img src="https://github.com/kphillip1/post-install-config/assets/165929885/3d6cd94d-0209-41c7-9cec-927c7e15d775" height="80%" width="80%" />
</p>

- Go to Admin Panel > Agents > Departments, Name the department and select a manager.
- Click "Creat Dept".
- Next, go to Admin Panel -> Agents -> Teams.
- Select "Add team".
- Name it "Level II Support" and add member by clicking on "Members" tab.
- Go to Admin Panel > Settings > User Settings to make sure that the registration required box is not checked.

<br />

<p>
<img src="https://github.com/kphillip1/post-install-config/assets/165929885/18fe1aa7-589e-43c6-90af-b3abaaf75cd3" height="80%" width="80%" />
</p>

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
<img src="https://github.com/kphillip1/post-install-config/assets/165929885/f6d60345-0fc6-47d2-9f30-63966f0547fd" height="80%" width="80%" >
</p>

- Go to Admin Panel > Manage > SLA and click "add new SLA plan". 
- Place these settings for Sev-A: (1 hour, 24/7). 
- Sev-B will be (4 hours, 24/7)
- Sev-C will be (8 hours, Monday - Friday).

<br />

<p>
<img src="https://github.com/kphillip1/post-install-config/assets/165929885/a593e70b-e376-4672-8e07-d5823e723d89" height="80%" width="80%"/>
</p>

- Go to Admin Panel > Manage > Help Topics and click "Add help topic".
- Title the first one "Business Critical Outage", the second "Personal Computer Issues", the third "Equipment Request", and lastly "Password Reset".
- Log into the user portal of osTicket at: http://localhost/osTicket/.
- Use a user you created to create tickets.


<br />

<h2 align="center"> Nice work! OsTicket is configured and ready for tickets. </h2>
