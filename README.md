# 🏦 ATM Application

A simple banking system designed to simulate the core functionality of an Automated Teller Machine (ATM). The application allows users to manage their bank accounts and perform common banking operations like checking balances, transferring money, withdrawing funds, and viewing transaction history.

---

## 📋 Table of Contents
- [Overview](#-overview)
- [Project Goals](#🎯-goals-of-the-project)
- [System Architecture & Roles](#-system-overview)
  - [Account Holder](#account-holder)
  - [Administrator](#administrator)
- [Core Features](#-main-features)
- [Security Implementation](#-security)
- [System Component Breakdowns](#⚙️-core-system-components)
- [Workflow Examples](#-example-flows)

---

## 🔍 Overview
This project gives developers practical experience in designing, developing, testing, and implementing a software system from start to finish. It provides an opportunity to work with critical backend and frontend concepts such as user management, authentication, account management, transactions, data persistence, and system security.

In addition to user-facing features, the application provides administrative capabilities to manage users and monitor global account activities.

---

## 🎯 Goals of the Project
* **Real-World Simulation:** Simulate a real-world banking system ecosystem.
* **UX & Security:** Provide a simple, intuitive, and secure way for users to manage their funds.
* **Role-Based Access:** Incorporate administrative controls for oversight and user management.
* **Full-Lifecycle Experience:** Gain practical experience building a complete software system from requirements design through implementation and testing.
* **Core Software Concepts:** Apply software development principles such as authentication, authorization, transactional integrity, and data persistence.

---

## 👥 System Overview
The ATM Application consists of two primary user roles:

### Account Holder
Account holders can securely access and manage their personal bank accounts. 
* Create and manage a user profile.
* View current account balances in real-time.
* Withdraw money safely from an account.
* Transfer money to another account instantly.
* View and monitor transactional account history.

### Administrator
Administrators are responsible for system oversight, managing users, and monitoring activities within the banking platform.
* View, modify, and manage user accounts.
* Monitor global account activities and anomalies.
* Audit system-wide transactions.
* Update or correct account information.
* Review historical transaction logs for security.

---

## 🚀 Main Features
* **User Account Management:** Users can seamlessly register accounts and access their profile dashboard.
* **Balance Inquiry:** Account holders can instantly view their current available ledger balance.
* **Money Withdrawal:** Users can withdraw funds securely from their accounts (conditional on sufficient funds).
* **Money Transfer:** Users can transfer money between internal accounts while the system securely records the ledger entries.
* **Transaction History:** Account holders can view complete logs of previous activities, including breakdowns of withdrawals and transfers.
* **Administration Panel:** A dedicated portal for system administrators to audit users and monitor transaction activities.

---

## 🔒 Security
The application implements strict security measures to protect user accounts and financial data. Depending on your choice of stack, the security architecture includes:

* **Authentication:** Multi-factor or secure credential-based login.
* **Password Hashing:** Secure password storage using modern hashing algorithms (e.g., bcrypt, Argon2).
* **RBAC (Role-Based Access Control):** strict authorization barriers separating Account Holders and Administrators.
* **Transaction Validation:** Server-side transaction validation to ensure operations only execute with valid inputs and sufficient funds.
* **Access Protection:** Guardrails against unauthorized account brute-forcing or session hijacking.
* **Audit Logging:** Comprehensive transaction logging and auditing trails for data integrity.

---

## ⚙️ Core System Components
The application is structured into the following logical layers:

| Component | Responsibility |
| :--- | :--- |
| **Authentication** | Handles user authentication, tokens, and session access control. |
| **User Management** | Manages registration, profiles, and basic user data. |
| **Account Management** | Manages financial accounts, statuses, and ledger balances. |
| **Transaction Management** | Processes atomicity-safe withdrawals, deposits, and transfers. |
| **Transaction History** | Records immutable history and exposes searchable transaction logs. |
| **Administration** | Exposes privileged toolsets for monitoring and account moderation. |
| **Data Storage** | The persistence layer (SQL/NoSQL) storing users, accounts, balances, and logs. |

---

## 🔄 Example Flows

### Account Holder User Flow
