# Introduction 

# 🔐 Active Directory Detection & Response Project

This lab focuses on detecting **unauthorized user activity** within an Active Directory environment using **Splunk**, **Slack**, and **Shuffle** for detection and automated response. It is deployed on the **Vultr cloud platform**, providing a scalable and realistic environment for hands-on cybersecurity training.

I’m using this project to gain real-world experience with:
- **Splunk** and **Shuffle** (first-time use)
- **Firewall configuration** to improve my networking skills
- **SOC-style detection and automation workflows**

---

## 📁 Project Breakdown

### ✅ Part 1: Building a Logical Diagram
- Create a logical diagram to visualize the environment and data flow.
- Helps clarify how systems will interact and where telemetry is collected.

---

### ☁️ Part 2: Setting Up the Cloud Environment
- Deploy a **Windows Server** (for AD and test user login)
- Deploy an **Ubuntu Server** (for Splunk)
- Configure a **firewall** to control inbound/outbound access

---

### 🏢 Part 3: Install and Configure Active Directory
- Install Active Directory on the Windows Server
- Promote it to a **Domain Controller**
- Join a second Windows machine to the domain
- Create multiple user accounts
- Log in with one user to verify domain authentication is working

---

### 📊 Part 4: Configure Splunk & Create Alerts
- Install Splunk on the Ubuntu server
- Configure Splunk to ingest telemetry from Windows endpoints
- Create an **alert** for detecting successful unauthorized logins

---

### 🤖 Part 5: Integrate Slack & Shuffle for SOAR Automation
- Create an automation playbook in **Shuffle**:
  - When an unauthorized login is detected:
    - A notification is sent to **Slack**
    - An email is sent to the **SOC analyst**
    - If the analyst replies `"yes"`, the user is automatically disabled
    - If `"no"`, no action is taken
  - A final confirmation is sent to Slack once action is completed

This simulates a **real-world SOAR process**, automating detection and response within a blue team workflow.

---

## 🛠️ Technologies Used
- Vultr (Cloud Hosting)
- Windows Server & Active Directory
- Ubuntu Server
- Splunk (SIEM)
- Shuffle (SOAR)
- Slack (Notifications)
- Firewall Configuration (Networking/Security)

  
