<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This project outlines the configuration of osTicket, an open-source help desk ticketing system after the installation process. This lab assumes a virtual machine has been established with the prerequisite files installed for working osTicket. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles, Departments & Teams
- Allow Users to Create Tickets
- Configure Users
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<p>
<img src="https://imgur.com/CURq2PC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/IHwQJcV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/ULXpzQT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Log into the OsTicket browser and make sure you are on the "admin panel" (note if it shows "agent panel" up top then you are currently in the admin panel and vice versa) reference picture # 1. Click agents --> roles --> add new role --> create a "super admin" whom can do every task and has all permissions/access. This process will need to be repeated to perform the next two steps which are: configuring the departments & teams (create a "System Administrators department" & "level II Support team"). Please reference screenshots above.
</p>
<br />

<p>
<img src="https://imgur.com/Pz4KJSI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to settings -> Users -> settings again and make sure the box titled "Require registration and login to create tickets" is unchecked. This is will allow everyone access to make tickets without restrictions. 
</p>
<br />

<p>
<img src="https://imgur.com/lsniCuX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<img src="https://imgur.com/AJRxGyZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/plHrj8I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create two new test agents ("John Doe" and "Jane Doe")--> Assign John to "System Administrators" department with "Super admin" permissions level & add him to "Level II support" team. All of these options are located under the "access & Teams" tabs on the same agent screen. Next add "Jane Doe" the same way as previously completed for John Doe. Please reference pictures above that are in order.
</p>
<br />

<p>
<img src="https://imgur.com/r537R13.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this step you will configure how customers and employees use the ticketing system software. Go to the agent panel --> Users tab --> create new user --> create two new generic users named "Jerry" and "Kim" with email addresses. Any name or email combonation is fine since these are both just test accounts for the third and final part of this entire Lab titled "Ticket Lifecycle". 
</p>
<br />

<p>
<img src="https://imgur.com/axEMi5X.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, a "Service Level Agreement" (SLA) needs to be created. Here are the layouts: "Sevice Level I" - helpdesk tickets must be responded to within 1 hour on a 24/7 schedule. "Service Level II" - ticket response time must be within 4 hours on a 24/7 schedule. "Service level III"- within 8 hours on a regular business hour time frame. Go to admin panel -> manage -> SLA to create all three of these SLAs. 
</p>
<br />

<p>
<img src="https://imgur.com/DKVAXHN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/qifHwMA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The last step is to configure "help topics". In this step you will create the help ticket names in OsTicketing for users to select when they are having specific issues.  The tickets will also need to be assigned to a "department" along with a "SLA priority". You can even auto-assign that particular help desk ticket topic to a group like "Support level I" or level II depending on the severity. Ex: create ticket help topic titled "Network Outage" --> priority level "emergency" --> "Service level I" SLA plan --> sent to the "System Administrators" group --> auto-assigned to the "support team" or to an individual agent like John or Jane. This concludeds how to setup help desk support tickets from the admin level post Installation.
