<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used</h2>

- Windows 10 (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Acknowledge the difference between the Agent Panel and Admin Panel.
- Configure Roles to define permissions for agents.
- Set up Departments to group tickets by areas of responsibility.
- Create Teams to pull agents from multiple departments.
- Configure user settings to allow or restrict ticket creation.
- Add Agents (workers) and Users (customers).
- Set up Service Level Agreements (SLAs) for ticket response times.
- Create Help Topics for users to categorize their tickets.

<h2>Configuration Steps</h2>

<h3>1.) Acknowledge Agent Panel vs Admin Panel</h3>

- The **Agent Panel** is used by agents to work on tickets.
- The **Admin Panel** is used to manage system settings, configurations, and permissions.

<h3>2.) Configure Roles</h3>

Navigate to **Admin Panel -> Agents -> Roles**.
Add a new role called **Supreme Admin**.
- Define permissions for agents based on the role they will have. In this lab, we will give permissions for the Tickets, Tasks, and Knowledgebase sections.

![image](https://github.com/user-attachments/assets/e506e072-2998-4fab-bef5-7d1beb5f1cab)

![image](https://github.com/user-attachments/assets/1a2b3410-c606-40aa-8b88-17cd0b304b90)

![image](https://github.com/user-attachments/assets/03856500-f6a4-4659-8e09-70bd3b79cd79)

![image](https://github.com/user-attachments/assets/f03d9ebd-9188-460b-a20c-6a300fbc7457)

<h3>3.) Configure Departments</h3>

- Navigate to **Admin Panel -> Agents -> Departments**.
- Add a new department called **SysAdmins**.
  - Use departments to control ticket visibility and assign areas of responsibility (e.g., Help Desk, SysAdmins, Networking).

![image](https://github.com/user-attachments/assets/11fb785c-e77f-44ba-bfb4-5631ec7f2071)

<h3>4.) Configure Teams</h3>

- Navigate to **Admin Panel -> Agents -> Teams**.
- Create a new team called **Claims Intake**.
  - Pull agents from different departments to form specialized teams.

![image](https://github.com/user-attachments/assets/65d83120-d398-4bca-902c-a475accad41a)

<h3>5.) Allow Anyone to Create Tickets</h3>

- Navigate to **Admin Panel -> Settings -> User Settings**.
- Uncheck **Require registration and login to create tickets** to enforce ticket creation by anyone.
- Enable **Public - Anyone can register** to disable requiring users to register and log in before creating tickets.

![image](https://github.com/user-attachments/assets/fd414943-34d8-47e3-a866-e02c97acc017)

<h3>6.) Configure Agents (Workers)</h3>

- Navigate to **Admin Panel -> Agents -> Add New**.
- Add agents with the following details:
  - **Jane**: Assigned to the **SysAdmins** department.
  - **John**: Assigned to the **Support** department.

![image](https://github.com/user-attachments/assets/c8fde524-a0f9-4655-a3b1-ffe54e6b8b03)

You can choose to set their password or send the agent a password reset email.

![image](https://github.com/user-attachments/assets/d6c8e648-a977-4d9c-b746-08dd7e67c73d)

![image](https://github.com/user-attachments/assets/3672b60f-de23-4e29-86a4-f23c6275e9be)

![image](https://github.com/user-attachments/assets/c9e6118d-2437-4e0b-8d6e-0f968e046191)

![image](https://github.com/user-attachments/assets/98e42b8b-02c4-4c92-a64e-35082e9d241d)

![image](https://github.com/user-attachments/assets/a3aca015-92dd-4dac-80ad-a1e64fb2cfb5)

![image](https://github.com/user-attachments/assets/2407a470-8733-4777-82a3-4bd1f2f96bd6)

<h3>7.) Configure Users (Customers)</h3>

- Navigate to **Agent Panel -> Users -> Add New**.
- Add users with the following details:
  - **Karen**
  - **Ken**

![image](https://github.com/user-attachments/assets/1aa6c71a-42e8-429c-891a-15bed0cecd80)

![image](https://github.com/user-attachments/assets/7dd19da1-64b4-48fc-90fd-6908f684e3c7)

<h3>8.) Configure SLA (Service Level Agreements)</h3>

- Navigate to **Admin Panel -> Manage -> SLA**.
- Add the following SLAs:
  - **Sev-A**: Grace Period = 1 hour, Schedule = 24/7.
  - **Sev-B**: Grace Period = 4 hours, Schedule = 24/7.
  - **Sev-C**: Grace Period = 8 hours, Schedule = Business Hours.

![image](https://github.com/user-attachments/assets/2210c8e6-7538-4339-9255-31f3244a41ff)

![image](https://github.com/user-attachments/assets/765930cf-e255-4024-93ba-d1892c0c618d)

![image](https://github.com/user-attachments/assets/21acc7e6-a159-48ad-b155-1b005cbe90bf)

![image](https://github.com/user-attachments/assets/5feb7356-15b5-42ca-81f9-bf8cacb7bfad)

<h3>9.) Configure Help Topics</h3>

- Navigate to **Admin Panel -> Manage -> Help Topics**.
- Add the following help topics for users to select when creating a ticket:
  - **Business Critical Outage**
  - **Personal Computer Issues**
  - **Equipment Request**
  - **Password Reset**
  - **Other**

![image](https://github.com/user-attachments/assets/9b23c9f1-02a5-4147-ba81-1fed94801c14)

![image](https://github.com/user-attachments/assets/409e31d8-a593-4a73-aeeb-6b2b011230c0)

<h2>Conclusion</h2>

By completing the post-installation configuration steps, you have successfully customized osTicket to suit your organization's requirements. You are now ready to start using osTicket to manage and resolve customer issues efficiently.
