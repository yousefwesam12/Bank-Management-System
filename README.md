# 🏦 Object-Oriented Bank Management System (C++)

A comprehensive, console-based **Bank Management System** implemented in **C++** using strict **Object-Oriented Programming (OOP)** principles. The system operates with full data persistence using flat-file databases (`.txt`) and features a highly structured abstract screen architecture for modular execution.


---

## ✨ Features

* **🧩 Clean OOP & Abstract Screens:** Utilizes base layout components (`clsScreen`) to standardize the user interface across all functional areas of the application.
* **💾 File-Based Data Persistence:** Real-time reading/writing of records to flat files (`Clients.txt`, `Users.txt`, `Currencies.txt`) ensures all application states are saved permanently.
* **🔐 Secure Login & Activity Logging:** Features a dynamic registration workflow (`LoginRegister.txt`, `RegisterLog.txt`) to audit system access and user transactions over time.
* **💸 Full Transaction Suite:** Implements complete monetary transactions including Deposits, Withdrawals, Total Balance aggregations, and Secure Client Transfers (`clsTransferScreen`).
* **💱 Multi-Currency Calculator System:** Integrated currency tracking modules capable of dynamically checking list views and executing currency conversions on-the-fly.
* **🛠️ Complete CRUD Operations:** Fully independent interfaces to Add, Update, Delete, and List both Bank Clients and System Users securely.

---

## 📂 Project Architecture

The repository isolates logic, database layout, and ui components flawlessly:

### 🗃️ Database Layer (File System)
* `Clients.txt`: Stores core bank customer financial balances and profiles.
* `Users.txt`: Holds administrator credentials and access permission flags.
* `Currencies.txt`: Contains international exchange rates and country codes.
* `LoginRegister.txt` / `RegisterLog.txt`: Automated logs for user sessions and account actions.

### 🏛️ Core Business Logic Classes
* `clsBankClient` & `clsBankUser`: Encapsulate the core fields, getters/setters, and methods for managing data records.
* `clsCurrency`: Manages monetary metrics and calculation functions.
* `clsDate` & `clsPeriod` & `clsString` & `clsUtil`: Robust helper classes providing high-level utilities for date formatting, validation, string manipulation, and system tools.

### 🖥️ Presentation Layer (UI Screens)
* `clsScreen`: The base structure for all UI components.
* `clsAddNewClientScreen`, `clsDeleteClientScreen`, `clsUpdateClientScreen`: Individual panels dedicated to handling customer records.
* `clsTransactionsScreen`, `clsTransferScreen`, `clsTransferLogScreen`: Manage all account-to-account operations.
* `clsCurrencyListScreen`, `clsCurrencyCalculator`: Interface tools dedicated to handling foreign currency operations.

---

## 🚀 How to Run the Project

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/yousefwesam12/Bank-System.git](https://github.com/yousefwesam12/Bank-System.git)
