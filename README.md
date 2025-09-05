<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
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
- Configure Service Level Agreements (SLA)
- Configure Help Topics

<h2>Configuration Steps</h2>
<br>
<h3>1. Configuring Roles</h3>
<br>
<p>
  This link is for the <a href="http://localhost/osTicket/scp/login.php">Admin/Analyst Login Page.</a> And this link is for the <a href="http://localhost/osTicket">End Users on osTicket Page.</a>
</p>
<p>
  The first thing we will do is configure roles. This will allow us to set certain permissions for each role in an enterprisee. To get started, open up the Admin/Analyst link.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-03 at 3 15 09 PM" src="https://github.com/user-attachments/assets/03257b3d-d94b-4ff9-848c-0710c71c29b0" />

</p>
<p>
  Please make sure you are on the Admin Panel, it should look similar to this. Inside here, go to the Agents tab, and then inside there, make your way to the Roles tab. 
</p>
<img width="80%" height="80%" alt="Screenshot 2025-09-03 at 3 35 49 PM" src="https://github.com/user-attachments/assets/4bf3a49d-3a16-4111-9bf5-ba71e0880941" />
</p>
<p>
You can assign the name here for the role along with any internal notes if necessary.
</p>
<p>
<img width="80%" height="80%" alt="Screenshot 2025-09-03 at 3 35 57 PM" src="https://github.com/user-attachments/assets/08e87123-a651-4ae0-8840-d360ebfd6865" />

</p>
<p>
Inside this tab, you can configure all of your permissions for this role. This will be my admin, so I will go ahead and enable all the permissions for this role.
</p>
<p>
<img width="80%" height="80%" alt="Screenshot 2025-09-03 at 3 43 37 PM" src="https://github.com/user-attachments/assets/596a2e83-1c06-4c19-8660-ab3724060b45" />
</p>
<p>
  We have successfully added our Supreme Admin role and assigned all the proper permissions, good work.
</p><br>
<h3>2. Configuring Departments</h3>
<br>
<p>
  Next, we will configure Departments. This will make assigning tickets easier, knowing where the tickets come from or even who can see the tickets as well. 
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-03 at 5 58 23 PM" src="https://github.com/user-attachments/assets/da224452-41d4-4777-9153-1b6e0b7bb0a7" />

</p>
<p>
  To create Departments, return back to the Admin page and go into the Agents tab. Click the Departments tab and then select Add New Department.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-03 at 5 59 42 PM" src="https://github.com/user-attachments/assets/207f84e5-c9fe-4c52-9bb9-d46ee621955b" />

</p>
<p>
  On this page, you can configure each department to your enterprises needs. I will create my first Department as SysAdmins and I will leave all the settings to default. You can always come back and make changes to each department.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-03 at 6 05 31 PM" src="https://github.com/user-attachments/assets/3f2ddc29-7551-4e19-a1c8-3d4453ec8459" />

</p>
<p>
  Underneath the Access tab, you can add in any Agents here. We will come back to this when we have configured some agents to work here! For now, we will Create Dept.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-03 at 6 06 16 PM" src="https://github.com/user-attachments/assets/96497ea6-9900-45da-982f-1d7b5326e40d" />
  
</p>
<p>
  We have successfully added the SysAdmins department. Very good.
</p>
<br>
<h3>3. Configuring Teams</h3>
<br>
<p>
  This step will be helpful if you have a group of people, all from different departments. For example, if you run an online bank, you can have administrators on the team as well as the help desk technicians who field the tickets themselves. To get started, go over to the admin panel on osTicket.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-03 at 6 20 18 PM" src="https://github.com/user-attachments/assets/537eaa52-b4d5-4912-9980-7cf8614b73db" />

</p>
<p>
  From the Admin panel, select the Agents tab and then select the Teams tab. I have the Add New Team button highlighted. Go ahead and click it.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-03 at 6 27 32 PM" src="https://github.com/user-attachments/assets/63545267-b36d-476b-9541-ac76c6dba125" />

</p>
<p>
As with configuring the Departments, you can also add members to the team from the members tab. I will do that later. For now, click Create Team.
</p>
<br>
<p>
  <h3>4. Allow anyone to create tickets</h3>
  <br>
</p>
<p>
  Configuring this setting will allow anyone to create a ticket even if they don't have an account. You may want to do this if you're setting up a sandbox environment. Return to the Admin page and click into the settings tab.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-04 at 9 19 58 PM" src="https://github.com/user-attachments/assets/bb9cde43-1937-4628-8814-79ad6d5743e0" />

</p>
<p>
Once inside the settings tab, click on the Users tab. You can configure all sorts of useful settings here. Again, UNCHECK the registration required box to make submitting tickets easier for a sandbox application. 
</p>
<p>
  <h3>5. Configuring Agents</h3>
</p>
<p>
  Now your osTickets system needs some workers(Agents). Head over to the Admin panel again and click on Agents.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-04 at 9 32 44 PM" src="https://github.com/user-attachments/assets/b7c3c30a-e93a-47ab-b98a-8469a04b154d" />

</p>
<p>
  Click on Add New Agent. Inside you will be able to set up any Agents you may have. Note that there is also an Access, Permissions, and a Teams tab. I will name my Agent Jane Doe.
</p>
<p>
  <img width="80%" height="80"% alt="Screenshot 2025-09-04 at 9 35 49 PM" src="https://github.com/user-attachments/assets/1ba96ab4-96af-4a49-a8d1-bd5612ae8571" />

</p>
<p>
  I have assigned my Agent Jane Doe to the SysAdmins department we created earlier, specifically to the role of Supreme Admin. I have also assigned Jane Doe to the Online Banking Team we created earlier. Click over on the Teams to perform this. 
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-04 at 9 44 14 PM" src="https://github.com/user-attachments/assets/99ff0303-299b-4533-8817-8703e07f1b21" />

</p>
<p>
  Our new agent Jane was successfully added. I also added another agent, John. I have assigned him to the Support Department and gave him the view only role.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-04 at 9 48 03 PM" src="https://github.com/user-attachments/assets/d2bde100-1b65-4f0f-abf2-29fec86876e1" />

</p>
<p>
  If you need to set a password for your agents, click on the Agent tab. Then click on the agent who's password you would like to set.
</p>
<br>
<p>
  <h3>6. Configuring Users</h3>
  <br>
</p>
<p>
  We are ready to now add Users to the Directory. To configure these settings, head over to the Agent Panel, then click on the Users tab. Look for the Agent Panel link at the top of the page, to the right of our names.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-04 at 9 56 10 PM" src="https://github.com/user-attachments/assets/a7fed4ea-0ec0-43fd-9cdd-9af2f5ced38f" />
</p>
<p>
  The Agent Panel should look like this. Find your way to the Add User button and click it. Enter in your customers information. Our customer will be Karen for our sandbox. I will only add one for my application, but add as many as you need!
</p>
<br>
<p>
  <h3>7. Configuring SLA</h3>
  <br>
</p>
<p>
  Configuring SLA, or Service Level Agreements, is important to indicating the severity of a ticket. A severity-A ticket could mean a website-wide outage versus a severity-C ticket where an employee has lost a laptop charging cable, but will not cause any stoppage in production for the company. 
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-04 at 10 15 38 PM" src="https://github.com/user-attachments/assets/e81315af-4925-43d8-9262-c2516e29b0c7" />

</p>
<p>
  Finding your way once again to the Admin Panel, click on the Manage tab. Find the SLA tab below it, and select Add New SLA Plan.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-04 at 10 18 28 PM" src="https://github.com/user-attachments/assets/3657689c-ab0e-4ad2-8b3b-3576497a9521" />

</p>
<p>
  Our first of three will be Sev-A. We can configure each SLA's grace period (time to respond before ticket is due). The schedule can also be set to 24/7, 24/5 or office hours. For Sev-A, we will go with a 1 hour grace period and a 24/7 schedule.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-04 at 10 22 43 PM" src="https://github.com/user-attachments/assets/4b719c16-812a-42e1-90ae-7cbba8a31850" />

</p>
<p>
  The second SLA will have a 4 hour grace period and the 24/7 schedule.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-04 at 10 23 21 PM" src="https://github.com/user-attachments/assets/a1e67a54-eb64-42ee-a751-27a35f21221f" />

</p>
<p>
  And our last SLA will be Sev-C. This has an 8 hour grace period. Since Sev-C will be lower priority, setting the schedule to just business will be more than fine.
</p>
<br>
<p>
  <h3>8. Configuring Help Topics</h3>
  <br>
</p>
<p>
  Adding Help Topics will be beneficial as this will help the end users decide what category to file the ticket under, which will assist the help desk in solving the tickets quicker.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-04 at 10 34 18 PM" src="https://github.com/user-attachments/assets/852e8616-86f6-4f16-a849-8531083db69a" />

</p>
<p>
  Go ahead and return to the Admin Panel once more. Click on the Manage tab, then the Help Topics tab and then click Add New Help Topic. I will be creating 5 different help topics to choose from. They will be Business Critcal Outage, Personal Computer Issues, Equipment Request, Password Reset and Other. Repeat this step for each topic and assing the Parent Topic however you would like.
</p>
<p>
  <img width="80%" height="80%" alt="Screenshot 2025-09-04 at 10 42 37 PM" src="https://github.com/user-attachments/assets/ff5880fd-9eba-4aec-9bb5-aca9ce701583" />

</p>
<p>
  All of your newly created help topics should now appear in your Help Topics tab.
</p>
<br>
<p>You have now successfully configured all of your settings needed to setup your osTicket to run in a sandbox environment. Go ahead and play around with any of your settings, you may prefer what I have shown.
</p>
<br>
<p><h3>Great work!</h3></p>
