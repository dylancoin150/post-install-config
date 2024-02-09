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
- Configure Departments
- Configure Teams
- Allow anyone to create tickets
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

1. Login to osTicket and go to Admin Panel -> Agents -> Roles -> Add New Role. Name your new role "Supreme Admin", then click on Permissions and check everything allowing that role to have complete access to everything.

2. Under Agents go to Departments (still in the Admin Panel) and click Add New Department. Name your new department "System Administrators" and click "Create Dept".

3. Under Agents go to Teams (still in the Admin Panel) and click "Add New Team" and name it "Level II Support". Click "Members", add the agents you want to be on that team, and click "Create Team".

4. Under "Settings" go to "Users" and ensure that "Require registration and login to create tickets" is unchecked.

5. Under Agents go to Agents (still in the Admin Panel) and click "Add New Agent". Fill out their name (i.e. Jane Doe), and create their usernames and passwords. Under "Access" you can select the department(s) the agent is allowed to access. You can get more specific about the permissions for the agent if you want under "Permissions." Lastly, you can assign the agent to a specific team under "Teams". Click "Create" to finalize and save all of the agent's information. *Repeat this step as many times as needed to add more agents*

6. Go to Agent Panel -> Users -> Add User. You can fill out the user's information (email, name, phone number, and internal notes i.e. ken.doe@osticket.com, Ken Doe)

7. Go to Admin Panel -> Manage -> SLA -> Add New SLA Plan. Name your new SLA Plan "SEV-A", set the schedule (business hours, 24/7, etc.), set the grace period (how long you have to complete the ticket), and click Add Plan. *Repeat this step as many times as needed to add more SLA Plans*

8. Go to Manage -> Help Topics -> Add New Help Topic. Add the topic name and choose the parent topic (i.e. how important it is).
