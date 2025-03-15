<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This project outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [Video Walkthrough](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- <b>Configure Roles</b>: Assign certain roles to for certain users
- <b>Configure Departments</b>: Add the necessary departments for certain users and agents
- <b>Configure Teams</b>: Pull Agents from different Departments
- <b>Configure Agents</b>: The workers, basically the people that help solve the tickets
- <b>Configure Users</b>: The customers/end-users
- <b>Configure SLA</b>: Service Level Agreement that is a formal contract between the service level provider and the client
- <b>Configure Help Topics</b>: Categories for issues, helps users choose an issue that is related on their end


<h2>Configuration Steps</h2>

# osTicket Configuration

## Log into the Admin/Analyst panel with the credentials created for osTicket
<p>
<img src="https://github.com/user-attachments/assets/129ee379-54ad-4de7-a10b-9cadb71da8d2" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/a95ce5a6-5985-4c0d-b2dc-e98c05ab12fd" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

## Configure Roles (for grouping permissions)
<p>Admin Panel ---> Agents ---> Roles</p>
<p>
<img src="https://github.com/user-attachments/assets/b5033d6c-a146-43a3-bf75-5b463effb45f" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/01b38d9c-7f4b-4857-b849-b36fcf9d8a28" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/ba0fe77b-7e2b-4094-9fd5-ab7a982d045e" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Creat a new role called `Supreme Admin`
<p>
<img src="https://github.com/user-attachments/assets/681b72d1-654a-4fff-b364-b470a08f6b8a" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Be sure to assign the Role with Permissions for both the `Tickets` and `Tasks` categories
<p>
<img src="https://github.com/user-attachments/assets/3612ab64-bb65-4e8d-82a7-c99fc89bf315" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/93bf808a-159a-4086-814a-6fd95c49d5d5" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Add the role
<p>
<img src="https://github.com/user-attachments/assets/e46cebb2-3877-4248-878d-96b19ed51209" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/872fb477-69ac-473e-bdab-2b4b1213f95f" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


## Configure Departments
<p>
<img src="https://github.com/user-attachments/assets/b5033d6c-a146-43a3-bf75-5b463effb45f" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/d0ae055f-9cd3-4554-8b80-216750053cec" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


### Add the department named `SysAdmins`
<p>
<img src="https://github.com/user-attachments/assets/d0ae055f-9cd3-4554-8b80-216750053cec" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />
