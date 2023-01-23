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

- Login to the osTicket Admin Panel
- Congfire Roles
- Configure Deparments
- Configure Teams
- Configure Help Topics

<h2>Configuration Steps</h2>
<p> Login to the osTicket Admin Panel. Below displays the tickets for admin/helpdesk User Interface (UI) that will reflect the tickets that are created by the End User ([http://localhost/osTicket/scp/login.php](http://localhost/osTicket/scp/login.php))
</p>
<p align="center">
<img src="https://i.imgur.com/uzAA73f.png" height="65%" width="65%" alt="UI admin/help desk Tickets"/>
</p>

<br />
- <b>Configure</b> <a href="https://docs.osticket.com/en/latest/Admin/Agents/Roles.html">[Roles]</a>
    <ol>
  <li>Admin Panel -> Agents -> Roles</li>
  <li>Supreme Admin</li>
  </ol>
<p align="center">
<img src="https://i.imgur.com/Jw4EbMN.png" height="65%" width="65%" alt="UI to add Role"/>
</p>
<p>Below we have entered <b>"Supreme Admin"</b> as the role</p>
<p align="center">
<img src="https://i.imgur.com/sJukhDR.png" height="65%" width="65%" alt="enter role name"/>
</p>
<br />
<p> Now we can enable the <a href="https://docs.osticket.com/en/latest/Features/Visibility%20Permissions.html">permissions</a> for this role and as the "Supreme Admin" we've enabled every possible permission available.  
<p align="center">
<img src="https://i.imgur.com/OgnLk0E.png" height="65%" width="65%" alt="list of permissions"/>
</p>
<hr>
<p>
  -<b>Configure</b> <a href="https://docs.osticket.com/en/latest/Admin/Agents/Departments.html">[Departments]</a>
    <ol>
    <li>Admin Panel -> Agents -> Departments</li>
    <li> System Administrators</li>
      </ol>
</p>
<p align="center"> 
  <img src="https://i.imgur.com/WH7YRLn.png" height="65%" width="65%" alt="create department selection"/>
</p>
<br />
<p align="center">
<img src="https://i.imgur.com/44g5RJ2.png" height="65%" width="65%" alt="create department name"/>
  </p>
  <hr>
  - <b><i>Configure </i></b> <a href="https://docs.osticket.com/en/latest/Admin/Agents/Teams.html">[Teams]</a>
  <ol><li>Admin Panel -> Agents -> Teams</li>
    <li>Level I Support </li>
    <li>Level II Support </li>
</ol>
<p align="center">
    <img src="https://i.imgur.com/M1ISoyE.png" height="65%" width="65%" alt="create department name"/>
    </p>
    <p align="center">
    <img src="https://imgur.com/steRLxe.png" height="65%" width="65%" alt="create team"/>
    </p>
<p align="center">
          <img src="https://i.imgur.com/xUwxacj.png" height="65%" width="65%" alt="dipslays current teams"/>
    </p>
-<b>Allow anyone to create tickets </b> in <a href="https://docs.osticket.com/en/latest/Admin/Settings/Users.html?highlight=registration">User Settings</a>
    <ol>
    <li>Admin Panel -> Settings -> User Settings </li>
    <li>Registration Required: Require registration and login to create tickets -for this lab, we will leave it unchecked so that tickets can be created without restrictions/limitations</li>
    </ol>
    <p align="center"> 
    <img src="https://i.imgur.com/uMx7BbE.png" height="65%" width="65%" alt="require registration checkbox option"/>
         </p>
  <hr>
  - <b><i>Configure</b></i> <a href="https://docs.osticket.com/en/latest/Admin/Agents/Agents.html">[Agents (workers)]</a>
    <ol>Admin Panel -> Agents -> Add New
    <li>Jane</li>
        <li>John </li>
        </ol>
  <p align="center">
    <img src="https://i.imgur.com/pxwqK2W.png" height="70%" width="70%" alt="create agents"/>
    </p>
<p align="center">
    <img src="https://i.imgur.com/Hp11jGk.png" height="65%" width="65%" alt="establish access"/>
    </p>
    <hr>
    - <b><i>Configure</i></b> <a href="https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html">[Users (customers)]</a>
    <ol>Agent Panel -> Users -> Add New
        <li>Karen</li>
    <li>Ken</li>
</ol>
<p align="center">
    <img src="https://i.imgur.com/hukYViC.png" height="65%" width="65%" alt="agent panel new user"/>
    </p>
    <p align="center">
    <img src="https://i.imgur.com/QihL6U3.png" height="65%" width="65%" alt="new user created"/>
    </p>
    <hr>
    - <b><i>Configure</b></i> <a href="https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html">[SLA]</a>
    Admin Panel -> Manage -> SLA
    <ol>
    <li>Sev-A (1 hour, 24/7)</li>
    <li>Sev-B (4 hours, 24/7)</li>
    <li>Sev-C (8 hours, business hours)</li>
    </ol>
    <p align="center">
    <img src="https://i.imgur.com/KH2b0nw.png" height="65%" width="65%" alt="add new SLA"/>
    </p>
    <p align="center">
    <img src="https://i.imgur.com/NB5Ovwi.png" height="65%" width="65%" alt="add new SLA severity"/>
    </p>
<p align="center">
    <img src="https://i.imgur.com/uDkD7Lv.png" height="65%" width="65%" alt="list of current SLA"/>
    </p>
<hr>
- <b><i> Configure </b></i> <a href="https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html?highlight=help%20topics">Help Topics</a>
     <h5>Admin Panel -> Manage -> Help Topics</h5>
        <li> Business Critical Outage </li>
        <li> Personal Computer Issues </li>
        <li> Equipment Request </li>
        <li> Password Reset </li>
 <p align="center">
    <img src="https://i.imgur.com/n44Un1L.png" height="65%" width="65%" alt="create new help topic"/>
</p>
    <p align="center">
    <img src="https://i.imgur.com/MOE3unk.png" height="65%" width="65%" alt="business critical outage"/>
    </p>
    <p align="center">
    <img src="https://i.imgur.com/6dBcOCd.png" height="65%" width="65%" alt="personal computer issue"/>
    </p>
    <p>Below reflects all of the tickets that we've created</p>
<p align="center">
    <img src="https://i.imgur.com/RFC1bTH.png" height="65%" width="65%" alt="all tickets that have been created"/>
