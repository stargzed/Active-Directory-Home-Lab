# 🖥️ Active Directory Help Desk Lab (AWS + Spiceworks)

---

## 📌 Overview

Built a hands-on Active Directory environment in AWS to simulate real-world IT help desk and system administration tasks. This lab includes a domain controller, client machine, and a help desk ticketing system (Spiceworks) used to manage and resolve user incidents.

---

## 🛠️ Technologies Used

* AWS EC2 (Cloud Infrastructure)
* Windows Server 2022
* Active Directory Domain Services (AD DS)
* Remote Desktop Protocol (RDP)
* Spiceworks Help Desk
* Windows Event Viewer

---

## 🧱 Lab Architecture

* Domain Controller deployed in AWS
* Active Directory domain: **jaylab.local**
* Client machine joined to domain
* DNS configured for domain communication
* Help desk system used for ticket management

---

## ⚙️ Setup Summary

### 🔹 Domain Controller

* Installed Active Directory Domain Services
* Promoted server to Domain Controller
* Created domain: **jaylab.local**

### 🔹 Client Machine

* Configured DNS to point to Domain Controller
* Joined system to domain
* Authenticated using domain credentials

### 🔹 User Management

* Created domain users (e.g., **saint**)
* Managed passwords and account settings
* Configured Remote Desktop access permissions

---

## 🎟️ Help Desk Ticketing (Spiceworks)

Simulated real-world IT support scenarios using a ticketing system:

### 🎫 Ticket Examples

**1. User Unable to Log In**

* Issue: User could not access system
* Investigation: Checked Event Viewer logs
* Resolution: Reset password and verified access

---

**2. Account Lockout**

* Issue: Multiple failed login attempts
* Investigation: Identified authentication failures
* Resolution: Unlocked account and restored access

---

**3. Remote Desktop Access Issue**

* Issue: User unable to log in via RDP
* Investigation: Verified permissions
* Resolution: Added user to Remote Desktop Users group

---

## 🔍 Security & Log Analysis

Analyzed authentication activity using Event Viewer:

* **Event ID 4776** → Credential validation (NTLM authentication)
* **Event ID 4625** → Failed login attempts

Used logs to:

* Identify incorrect password attempts
* Investigate login failures
* Understand authentication workflows

---

## 🧠 Skills Demonstrated

* Active Directory administration
* User account management
* Help desk ticketing workflow
* Troubleshooting login issues
* DNS and network configuration
* Security log analysis
* Remote access configuration (RDP)

---

## 🧾 Key Takeaways

This project demonstrates how enterprise environments manage user authentication, handle IT incidents, and analyze security events. It provided hands-on experience troubleshooting real-world issues such as login failures, account lockouts, and permission misconfigurations.

---

## 🚀 Future Improvements

* Integrate SIEM tool (e.g., Splunk) for log monitoring
* Automate alerting for failed login attempts
* Expand environment with additional client machines
* Implement Group Policy (GPO) configurations

---
