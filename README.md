# Configure-Access-Control
# 🔐 Packet Tracer Lab – Configure AAA Authentication, Email, and FTP Services

## 📌 Overview

This Cisco Packet Tracer lab demonstrates how to configure **Authentication, Authorization, and Accounting (AAA)** along with **Email** and **FTP** services in a secure enterprise network. The lab provides hands-on experience with identity management, wireless authentication, email server configuration, FTP file transfers, and user privilege enforcement.

---

# 🎯 Objectives

### Part 1 – Configure and Use AAA Authentication

* Configure user accounts on a RADIUS (AAA) server.
* Authenticate wireless clients using WPA2 Enterprise.
* Verify successful DHCP address assignment after authentication.

### Part 2 – Configure and Use Email Services

* Enable SMTP and POP3 services.
* Create email user accounts.
* Configure email clients.
* Send and receive emails between network users.

### Part 3 – Configure and Use FTP Services

* Enable the FTP service.
* Create FTP user accounts with different permissions.
* Upload and download files using FTP.
* Verify user privilege restrictions.

---

# 🛠 Technologies Used

* Cisco Packet Tracer
* AAA (RADIUS Authentication)
* WPA2 Enterprise Wireless Security
* DHCP
* SMTP
* POP3
* FTP
* Command Line Interface (CLI)

---

# 🏗 Network Services Configured

## AAA Authentication

Configured a centralized AAA (RADIUS) server to authenticate wireless users.

### User Accounts

| Username | Password   |
| -------- | ---------- |
| user1    | PASSuser1! |
| user2    | PASSuser2! |

Wireless laptops authenticated against the AAA server before receiving DHCP addresses.

---

## Wireless Configuration

Configured:

* SSID: **HQ-INT**
* Authentication: **WPA2 Enterprise**
* User authentication through AAA server
* Automatic IP assignment using DHCP

Verified both laptops successfully obtained IP addresses in the:

192.168.50.0/24

network.

---

# 📧 Email Service Configuration

Enabled:

* SMTP
* POP3

Configured email domain:

mail.cyberhq.com

## Email Users

| Username | Email Address                                               |
| -------- | ----------------------------------------------------------- |
| HQuser1  | [HQuser1@mail.cyberhq.com](mailto:HQuser1@mail.cyberhq.com) |
| HQuser2  | [HQuser2@mail.cyberhq.com](mailto:HQuser2@mail.cyberhq.com) |
| BRuser1  | [BRuser1@mail.cyberhq.com](mailto:BRuser1@mail.cyberhq.com) |
| BRuser2  | [BRuser2@mail.cyberhq.com](mailto:BRuser2@mail.cyberhq.com) |

Configured multiple PCs and laptops as email clients.

Verified:

* Email composition
* Email transmission
* Email reception

---

# 📁 FTP Service Configuration

Enabled the FTP server and created users with role-based permissions.

## FTP Accounts

| User  | Privileges                                         |
| ----- | -------------------------------------------------- |
| sukyi | Read, Write, Delete, Rename, List                  |
| ajulo | Read, Write, Delete, Rename, List                  |
| malia | Read, Write, Rename, List *(Delete not permitted)* |

---

# 🔄 FTP Operations Performed

Successfully demonstrated:

* FTP login
* Directory listing
* File download
* File upload
* File rename
* Permission enforcement

Commands used:

```bash
ftp 192.168.75.2
dir
get aMessage.txt
put aMessage_new.txt
rename aMessage_new.txt aMessage_rename.txt
delete aMessage_new.txt
quit
```

---

# 🔒 Security Concepts Demonstrated

* Authentication
* Authorization
* Centralized Identity Management
* WPA2 Enterprise Security
* RADIUS Authentication
* Access Control
* Role-Based Permissions
* Secure Email Services
* File Transfer Management
* User Privilege Enforcement

---

# ✅ Skills Practiced

* Configuring AAA authentication
* Managing wireless security
* Configuring DHCP clients
* Creating user accounts
* Configuring SMTP and POP3
* Setting up email clients
* Sending and receiving email
* Configuring FTP services
* Uploading and downloading files
* Managing FTP permissions
* Using FTP CLI commands
* Troubleshooting authentication issues

---

# 📚 Key Learning Outcomes

By completing this lab, you will be able to:

* Configure centralized authentication using a RADIUS server.
* Secure wireless access with WPA2 Enterprise.
* Configure enterprise email services using SMTP and POP3.
* Create and manage user accounts for network services.
* Configure an FTP server and assign user permissions.
* Perform secure file transfers between clients and servers.
* Verify access control through role-based privileges.
* Understand the relationship between authentication and authorization in enterprise networks.

---

# 🖥 Lab Environment

* Cisco Packet Tracer
* Headquarters (HQ) Network
* AAA/RADIUS Server
* Mail Server
* FTP Server
* Wireless Laptops
* Desktop PCs
* DHCP Services

---

# 🚀 Conclusion

This lab provides practical experience in configuring essential enterprise network services. By integrating AAA authentication, wireless security, email communication, and FTP file management, the lab demonstrates how centralized identity management and role-based access control improve both network security and operational efficiency. It reinforces key cybersecurity and networking concepts commonly used in enterprise environments and prepares learners for real-world Cisco networking and security tasks.
