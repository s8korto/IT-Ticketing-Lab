# Creating Users and Agents

## Objective 

Configure the osTicket environment by creating departments, roles, teams, support agents, and end users to prepare the help desk for daily IT operations at Contoso Manufacturing.

---

## Business Scenario 

Contoso Manufacturing has recently deployed **osTicket** to centralise IT support requests. Before employees can begin submitting tickets, the IT Administrator must configure the help desk structure, assign permissions, and create support staff accounts.

---

# Step 1 - Create Departments

### Purpose

Departments organise tickets based on the type of support required and ensure requests are routed to the correct team.

### Procedure

1. Log in to the **Admin Panel**.
2. Navigate to **Agents → Departments**.
3. Select **Add New Department**.
4. Create the following departments:
   - Help Desk
   - Systems Administration
   - Network Support
5. Save the configuration.

### Verification

Confirm all departments appear in the department list.

![Departments](screenshots/01-Departments.png)

---

# Step 2 - Create Roles

### Purpose

Roles define the permissions available to support staff based on their responsibilities.

### Procedure

1. Navigate to **Agents → Roles**.
2. Select **Add New Role**.
3. Create the following roles:
   - Auditor
   - Help Desk
   - IT Manager
   - System Administrator
4. Configure the appropriate permissions for each role.
5. Save the changes.

### Verification

Verify each role appears in the Roles list with the correct permission settings.

![Roles](screenshots/02-Roles.png)