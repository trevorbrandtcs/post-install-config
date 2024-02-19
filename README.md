<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket
- osTicket Agent Login and Ticket Submission Page

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Create and Configure Roles, Departments, Teams, Agents, Users, and SLAs.
- Let anyone submit a ticket.
- Create and Configure Help Topics at Different Severity Levels.


<h2>Configuration Steps</h2>

<p>
<img src="https://imgur.com/2YmYf0U.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Welcome back! Let's get right into it. Assuming you're here from the last tutorial and doing these in order, go ahead and log into osTicket using the username and password you made. Notice that you can swap back and forth between an admin and agent panel.
</p>
<br />

<p>
<img src="https://imgur.com/B9nTxIj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We're going to create some roles. From the Admin panel, navigate to the Agents Tab. Click on roles, and then click "Add A New Role". We're going to name this one Supreme Admin. After you've typed a name for the role, go to the permissions tab and give this one every permission there is. Repeat the process for however many roles you'd like to add.
</p>
<br />

<p>
<img src="https://imgur.com/lizSLQL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, we'll create some departments. Starting from the Admin Panel, click on the Agents Tab. Click on Departments, and then click on "Add A New Department". Name this one System Administrators. Notice all of the fields you can change like SLAs, Manager, and so on. Repeat the process as many times as you'd like.
</p>
<br />

<p>
<img src="https://imgur.com/AUVS6Zm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Moving on, let's create a few teams. Back in the Admin Panel, click on the Agents Tab. Click on Teams, notice that Level I Support is already a team. Click on "Add A New Team" and name this one Level II Support. Repeat this process as many times as you'd like.
</p>
<br />

<p>
<img src="https://imgur.com/XGoNsOD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, we'll let anyone, even anonymous users, submit tickets. Navigate to the Admin Panel, and click on Settings-> Users. Take note that the setting is already set to Public, we could change this, or we could even require registration by checking the appropriate box. Since it's already public and without registration, we can leave it alone.
</p>
<br />

<p>
<img src="https://imgur.com/0t6aZ4V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Let's create a few Agents, we'll call them Jane and John. Agents are employees of the company. Go to the Admin panel and click on the Agents Tab. Click on "Add A New Agent" and fill out the first and last name fields, the email, and the username fields. Next, click "Set Password" and then uncheck the box, set the password, and uncheck the box that requires a password change at the agent's next login. Then give all of the appropriate permissions and assign to teams as needed. 
</p>
<br />

<p>
<img src="https://imgur.com/pmgVCdl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we'll create a couple of users, their names will be Ken and Karen. Users represent the customers. In the top right hand corner, switch to the Agent Panel. From the Agent Panel, click on the Users Tab, and then click on "Add User". Fill out the email and full name fields.
</p>
<br />

<p>
<img src="https://imgur.com/RZNC2ZW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate back to the Admin Panel, let's add a few SLAs. SLAs are Service Level Agreements, they dictate how quickly tickets are responded to, usually based on severity. From the Admin Panel, click on the Manage Tab, and then click on SLA. We'll add three SLAs in total. Sev-A: Business Critical, must be responded to within 1 hour in a 24/7 period. Sev-B: Moderate issue, must be responded to within 4 hours in a 24/7 period. Sev-C: Low Priority, Must be responded to within 8 hours during business hours. Click on "Add New SLA Plan" and fill out the fields accordingly.
</p>
<br />

<p>
<img src="https://imgur.com/M4pPiKE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finally, we'll add a few Business Help Topics. Business Help Topics are essentially a category of problem that already has specific characteristics and SLAs tied to it. From the Admin Panel click Manage -> Help Topics -> "Add New Help Topic". We'll create four in total. 
  
  <ol type="1">
   <li>Business Critical Outage - Click into New Ticket Options and select System Administrators, Open, Emergency, and Sev-A. Click Add Topic.</li>
   <li>Personal Computer Issues - Click into New Ticket Options and select Support, Open, Normal, and Sev-B. Click Add Topic.</li>
   <li>Equipment Request - Click into New Ticket Options and select Maintenance, Open, Normal, and Default. Click Add Topic.</li>
   <li>Password Reset: Click into New Ticket Options and select Support, Open, Normal, Sev-B. Click Add Topic.</li>
</ol>
</p>
<br />

<p>
This step is completed! We've officially configured osTicket. The <a href="https://github.com/trevorbrandtcs/ticket-lifecycle">next section</a> will cover a few example tickets, and how to respond to them.
</p>
<br />
