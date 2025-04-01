<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This project outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [Project Walkthrough](https://www.youtube.com)

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
<img src="https://github.com/user-attachments/assets/a2aa6a17-2565-4170-9948-0e5574beb48a" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


## Configure Departments
<p>Admin Panel ---> Agents ---> Departments</p>
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

### Be sure to leave the settings as default
<p>
<img src="https://github.com/user-attachments/assets/2139f5f1-0ded-490b-ba99-ea1c4aad2e14" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/6a4ff701-d235-41cd-ae53-4809fc584cc2" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Create the department
<p>
<img src="https://github.com/user-attachments/assets/e3120794-352f-474a-b8b2-970173c80e82" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


## Configure Teams
<p><p>Admin Panel ---> Agents ---> Teams</p></p>
<p>
<img src="https://github.com/user-attachments/assets/b5033d6c-a146-43a3-bf75-5b463effb45f" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/97ba4b04-9cc6-46e0-ad11-a34503358233" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Create the Team called `Online Banking`
<p>
<img src="https://github.com/user-attachments/assets/f9022502-3d22-468d-82d8-addeeb5f66d4" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/8bcd1103-95a5-48c7-b26b-e062c1b4f8b6" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


## Allow anyone to create tickets
<p>Admin Panel ---> Settings ---> User Settings</p>
<p>
<img src="https://github.com/user-attachments/assets/fcc5cc99-bf93-4e66-94bb-ec4774748971" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Check the option `Require registration and login to create tickets`, then save the changes
<p>
<img src="https://github.com/user-attachments/assets/0f9b70cc-7e40-4437-b229-d0d160000517" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


## Configure Agents
<p>Admin Panel ---> Agents ---> Add New</p>
<p>
<img src="https://github.com/user-attachments/assets/ff80b773-32a2-4677-b4c9-440c62762892" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Add two new Users: `Jane` and `John`, `Jane` will be added to the SysAdmin dept, and `John` will be added to the Support dept
<p>
<img src="https://github.com/user-attachments/assets/1fd279b2-3972-483a-9a72-4b26ac19762e" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

## Jane's Access
### For `Jane`, enter her first name, last name, email and username
<p>
<img src="https://github.com/user-attachments/assets/a49f4c64-05fc-4bff-af4b-112c169486c2" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### For `Jane`, set her password to `Password123!`
<p>
<img src="https://github.com/user-attachments/assets/272b071a-553d-482b-b4fd-5116b6ae1f32" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Uncheck the `Send the agent a password reset email` checkbox to set the password for the user
<p>
<img src="https://github.com/user-attachments/assets/751dfc2a-5595-40b9-b6c0-69710842c25f" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/bcd730a7-fb92-48a5-bdb8-d441c585294b" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Make a secure password then click "Set"
<p>
<img src="https://github.com/user-attachments/assets/88176194-598a-4ed3-80fd-d469bd649ec6" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Make a secure password then click "Set"
<p>
<img src="https://github.com/user-attachments/assets/88176194-598a-4ed3-80fd-d469bd649ec6" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### In the Access tab, set the department to `SysAdmins` and the role as the `Supreme Admin`
<p>
<img src="https://github.com/user-attachments/assets/67e94ca7-dc9b-4eec-81ed-8840c1566c0e" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/4df35215-774b-4394-bef2-5a210799d6fb" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


## John's Access
### For `John`, enter his first name, last name, email and username
<p>
<img src="https://github.com/user-attachments/assets/73bf7d55-1b7c-49eb-9b13-4ec70d5c9c58" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### For `John`, set his password to `Password123!`
<p>
<img src="https://github.com/user-attachments/assets/a0763b8a-c355-4e7a-9219-d302357620b0" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Uncheck the `Send the agent a password reset email` checkbox to set the password for the user
<p>
<img src="https://github.com/user-attachments/assets/751dfc2a-5595-40b9-b6c0-69710842c25f" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/bcd730a7-fb92-48a5-bdb8-d441c585294b" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Make a secure password then click "Set"
<p>
<img src="https://github.com/user-attachments/assets/88176194-598a-4ed3-80fd-d469bd649ec6" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### In the Access tab, set the deoartment to `Support` and the role as the `Supreme Admin`
<p>
<img src="https://github.com/user-attachments/assets/b1b87768-bda1-467c-9995-544433880b38" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/a4e58d2b-1a25-452f-b0ae-2b97fa76422c" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


## Configure Users
<p>Agent Panel ---> Users ---> Add New</p>
<p>
<img src="https://github.com/user-attachments/assets/9d8fdd80-eb07-4889-a833-dd8c2e7592c1" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Add new users: `Karen` and `Ken`
<p>
<img src="https://github.com/user-attachments/assets/6aa32c3d-1a53-4fa3-8f38-6c5413e7e1d7" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/25820a3f-534c-4afe-8bf5-25217962e545" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/4d744cf6-be02-41b6-86e4-64e8fce9e2c9" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/1fbdeb16-0312-4188-a280-8f30e63c4375" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/cce12fd8-9d5a-4cb3-91b2-159428cb19a4" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/f78833d5-6ba8-45dd-9bba-129f326fd8a6" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


## Configure SLA
<p>Admin ---> Manage ---> SLA</p>
<p>
<img src="https://github.com/user-attachments/assets/5a43fbf8-0c6d-4e6c-b8b8-9c95034c6c45" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Sev-A: Grace Period will be set to 1 hour since this is our highest level of severity
<p>
<img src="https://github.com/user-attachments/assets/e96203c2-0999-4f82-91b0-1caa90dd9aeb" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Sev-B: Grace Period will be set to 4 hours, major impact to production
<p>
<img src="https://github.com/user-attachments/assets/b4040371-92d3-47bf-961c-3d9141698f3c" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Sev-C: Grace Period will be set to 8 hours, little impact to production
<p>
<img src="https://github.com/user-attachments/assets/1862541d-2254-4990-afe1-06243fde492f" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />


## Configure Help Topics
<p>Admin ---> Manage ---> Help Topics</p>
<p>
<img src="https://github.com/user-attachments/assets/2bcd5df4-2903-4bd9-ac65-637ced259ad8" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

### Create categories for easy access when users are reporting an issue
<p>
<img src="https://github.com/user-attachments/assets/4abfa45a-c4ef-42e0-b2d7-ebfbaf6d9890" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />
<p>
<img src="https://github.com/user-attachments/assets/4648a1dd-c342-4f0e-8351-736d0453cae0" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/79524750-0e4a-436a-9ee4-05f7a88634f6" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/a774b669-a7a0-4a57-976d-d68c168762cd" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/b693e9f0-4bd5-492e-bd72-e2fb9acd91b6" width="500" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/11ea6974-4b7e-4b39-8321-5f8552efd129" width="500" alt="Disk Sanitization Steps"/>
</p>
<br />

## End Results
<p>
<img src="https://github.com/user-attachments/assets/c12b3a84-920f-45a5-a28b-17c6a518a637" width="500" alt="Disk Sanitization Steps"/>
</p>

---

<br />


# End of Project
