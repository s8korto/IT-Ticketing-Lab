# Installing osTicket

## Objective

Deploy an internal help desk system for an X Company.

---

## Lab Environment

| Component | Value |
|-----------|------|
| Virtual Machine | Windows Server 2022 |
| Web Server | IIS |
| PHP Version | 8.3.x |
| Database | MySQL server 8.4.X and MySQL Workbench |
| Application | osTicket |

---

# Step 1 - Install IIS

Internet Information Services (IIS) hosts the osTicket web application.

### Procedure

1. Open **Server Manager**.
2. Select **Add Roles and Features**.
3. Choose **Role-based installation**.
4. Select the local server.
5. Enable:

- Web Server (IIS)

6. Click **Install**.

### Verification

Open a browser and navigate to:

```
http://localhost
```

The IIS default page should appear.

![Windows-Features](screenshots/01-Windows-Features.png)

---

# Step 2 - Install PHP

### Purpose

osTicket is written in PHP and requires the PHP runtime.

### Procedure

1. Download PHP.
2. Extract files to:

```
C:\PHP
```

3. Configure IIS to use PHP.

### Verification

Create:

```
info.php
```

Contents:

```php
<?php phpinfo(); ?>
```

Navigate to:

```
http://localhost/info.php
```

The PHP information page should load.

![PHP-Installed](screenshots/02-PHP-Installed.png)

---

# Step 3 - Install MySQL

### Purpose

MySQL stores tickets, users, departments, and system settings.

### Procedure

1. Install MySQL Server.
2. Create a root password.
3. Verify the service is running.

### Verification

Log in using MySQL Workbench.

![MySQL-Installed](screenshots/03-MySQL-Installed.png)

---

# Step 4 - Create Database

### Purpose

Create the database required by osTicket.

### SQL Commands

```sql
CREATE DATABASE osticket;
```

### Verification

Confirm the database exists.

![Database-Configuration](screenshots/04-Database-Configuration.png)


