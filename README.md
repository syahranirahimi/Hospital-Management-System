# Hospital Management System with Multi-Role Privileges

A secure, desktop-based Hospital Management System developed using **Visual Basic 2010** and **SQL Server**. This project was created as a major academic milestone for the Database System course. It emphasizes team collaboration, cross-device database networking via local IP configurations, and strict security implementation through Role-Based Access Control (RBAC).

## 👥 My Role: Project Leader & Database Architect
As the project leader, I was responsible for overseeing the development lifecycle, dividing tasks among team members, and designing the core system infrastructure. My primary technical focus areas included:
* **Networking Integration**: Configuring local IP structures to allow team members to connect their applications to a shared database server across devices.
* **Access Control Realization**: Architecting database roles, credentials, and constraints to partition actions based on user access levels.

---

## 📌 Key Features
* **Cross-Device Connectivity**: Real-time server-client communication over a shared local area network (LAN) using IP synchronization.
* **Role-Based Access Control (RBAC)**: Enhanced security framework where database authorization is strictly locked based on user roles (e.g., specific staff accounts are locked to *Update-Only* or *Delete-Only* access levels to prevent unauthorized data drops).
* **Comprehensive Medical Records Management**: Integrated modules to manage patient registrations, doctor assignments, medical treatments, and billing histories securely.

## 🛠️ Tech Stack
* **Front-End / UI**: Visual Basic 2010 (VB.NET)
* **Back-End Database**: SQL Server / Microsoft SQL
* **Networking Protocol**: Local TCP/IP database pooling

---

## 📂 System Architecture Overview
The application establishes a decentralized local network structure allowing secure operations:

```text
[ Client Machine (Staff UI) ] ──( Local IP Request )──┐
                                                      ▼
[ Client Machine (Admin UI) ] ──( Local IP Request )──┼─► [ Shared SQL Server Database ]
                                                      ▲   (Enforces Update/Delete Roles)
[ Client Machine (Doctor UI) ] ──( Local IP Request )──┘
