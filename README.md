# ostickpost-install-config
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

- Create a New Role
- Add Permissions
- Create a Department
- Create some Agents
- Create some Users
- Create SLAs
- Create Help Topics

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/KMv9SYt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The First thing we are going to do is log in and make sure you are on the "Admin Panel". We are going to start off creating Roles which are permissions granted to Agents based on their department. We are going to create a Role for the Supreme Admin. So in the Admin Panel select the "Agents" tab and below that select the "Roles" tab and select "Add New Role"
</p>
<br />

<p>
<img src="https://i.imgur.com/E118pbY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From here, you will enter the name "Supreme Admin" and then select the "Permissions" tab. Since this is the Supreme Admin, we will be giving them access to everything. Select all the boxes under the "Ticket" tab and then do the same for "Task" and "Knowledgebase" tabs. Then select "Add Role".
</p>
<br />

<p>
<img src="https://i.imgur.com/ONdcRXz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next we are going to create some departments. Tickets are sent to differenmt departments on help desk. Under the same "Agents" tab, you will select the "Departments" tab. From here we will make a System Administrators department. Type in "System Administrators" and use default settings. At the Bottom click on "Create Dept". Next we will create Teams. Teams allow you to pull Agents from different departments for specific tasks or issues. On the same "Agents" tab, select the "Teams" tab. Create a team name which we will call in this example "Level II Support". Since we don't have any members yet just add yourself and then "Create Team" at the bottom. 
</p>
<br />

<p>
<img src="https://i.imgur.com/nE4f9yE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We will now configure the settings to allow anyone to create tickets. Go to the "Settings" tab at the top and select "Users" and select "Settings" tab. Make sure the "Registration Required" is not checked off.
</p>
<br />

<p>
<img src="https://i.imgur.com/E0DvXzh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We are now going to create Agents Jane and John. So go to the "Agents" tab and select the button "Add New Agents". You will type in Jane Doe and give email jane.doe@osticket.com. Create a user name for example jane.doe and then select the "Set Password" button. Make sure to uncheck the two boxes and then set the password. Then select the "Access" tab and add Jane to "System Administrators" and select "Supreme Admin" from the other drop down. Go to the "Teams" tab and add Jane to our "Level II Support" and then select "Create".
</p>
<br />

<p>
<img src="https://i.imgur.com/d2aOYer.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We are now going to create another user. Click on the "Add New Agent" and we created an agent named John Doe. Do the same thing as we did with Jane and create account and set password. Under the "Access" tab, put John under the Support department and allow him to "View Only" on the drop down to the right. Then select "Create"
</p>
<br />

<p>
<img src="https://i.imgur.com/tUPRin9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We are now going to create Users which are the people who report and create tickets for the help desk. We will be switching to the "Agent Panel" on the top right of the screen. Select the "User" tab and select the "Add User" button. Create a user. We used Karen and gave her an email and select the "Add User" button. Create another user Ken the same way you did with Karen.
</p>
<br />

<p>
<img src="https://i.imgur.com/ULTxfWc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We are now going to set up SLA's which stand for Service Level Agreements. This sets the length of time that the help desk Administrator expects the ticket to be closed. Go back to the Admin Panel and select the "Manage" tab and select "SLA". We will create three. Select the "Add New SLA Plan" button. We will name the first one SEV-A and set it for 24/7 Schedule with a 1 hour grace period. This means it doesn't matter if it's on the weekened. If a ticket comes in at Sunday at 10PM, then it needs to be resolved by 11PM on that same Sunday. Click "Add Plan"
</p>
<br />

<p>
<img src="https://i.imgur.com/Ag9FlxG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We add another SLA and name it SEV-B and set that also to 24/7 schedule with a 4 hour grace period. We will make the last one named SEV-C. This one will be on an 8 hour grace period and will be scheduled for normal business hours Monday - Friday 8AM- 5PM with U.S. Holidays. This means if you get the ticket Friday at 3PM, the ticket should be done by 2PM on Monday. 
</p>
<br />

<p>
<img src="https://i.imgur.com/56t6j9P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We are finally going to set Help Topics. This is for when the user (Ken and Karen) are creating tickets, they can say what the issue is. In the same Admin Panel, select the "Manage" tab and select the "Help Topics" tab. Click on "Add New Help Topic". We are going to create the first one with "business Critical Outage" and select "Add Topic" button. You will do the same thing for "Personal Computer Issues", "Equipment Request", and "Password Reset".
</p>
<br />

<p>

</p>
<p>
This concludes our post install of osTicket. In my next section, we will be role playing as Karen and Ken creating tickets and Jane and John with their help desk and completing those tickets. 
</p>
<br />et-preqs
