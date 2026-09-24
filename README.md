# 🏦 Simple ATM Application

A simple banking system designed to simulate the core functionality of an Automated Teller Machine (ATM). The application allows users to manage their bank accounts and perform common banking operations like checking balances, transferring money, withdrawing funds, and viewing transaction history.

The ATM Application is a simple banking system that allows account users to manage their
bank accounts and allows administrators to manage users and monitor account activities.

The main purpose of the ATM Application is to provide a simple and secure way for users
to manage their accounts while giving administrators the tools needed to manage
accounts and monitor transactions.

## 👥 User Roles & Permissions

The application provides distinct dashboards and functional capabilities depending on the authenticated user's role:

### 💳 Account User
Manages their own account and performs permitted financial transactions.
* **View Balance:** Check current available funds in the account.
* **Withdraw Money:** Remove cash or payout funds from the account.
* **Transfer Money:** Send funds between internal accounts only.
* **View Transaction History:** Review past logs of deposits, withdrawals, and transfers.

### 🔑 Admin
Manages users and accounts, and retains read-only visibility over account-user transactions for operational, auditing, and administrative purposes.
* **Add User / Create Account:** Set up new user profiles and assign secure credentials.
* **Edit User / Account:** Modify existing user profiles and data.
* **Delete User / Account:** Remove inactive or terminated accounts from the system.
* **View Account User Transactions:** Audit and monitor transaction histories across all user accounts.

---
