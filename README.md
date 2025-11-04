"# ATM" 
# 💳 ATM Simulation System in C

A console-based **ATM Simulation System** built in **C language** that allows users to generate a PIN, check balance, deposit or withdraw money, and view their last 10 transactions.  
It demonstrates **file handling**, **linked lists**, and **modular programming** in C.

---

## 🧠 Features

- 🔐 **PIN Generation & Validation**
  - Generates a 4-digit PIN and stores it in `pin.txt`
  - Validates PIN before giving access to ATM functions

- 💰 **Banking Operations**
  - Check balance  
  - Deposit and withdraw money  
  - Prevents overdraft withdrawals

- 🧾 **Transaction History**
  - Maintains a history of the last 10 transactions  
  - Uses a **linked list** to manage queue-based storage

- 📂 **Persistent Storage**
  - Saves PINs in a text file (`pin.txt`) for reuse across sessions

---

## 🧩 Code Overview

| Function | Description |
|-----------|-------------|
| `pinGeneration()` | Generates and saves a 4-digit PIN |
| `checkPin()` | Validates user-entered PIN against saved ones |
| `showBalance()` | Displays current account balance |
| `depositMoney()` | Adds user deposit to the balance |
| `withdrawMoney()` | Deducts withdrawal amount safely |
| `saveHistory()` | Saves transaction record to linked list |
| `removeHistory()` | Removes oldest transaction when limit (10) reached |
| `showHistory()` | Displays all recent transactions |

---

## 🧾 Example Console Output
ATM System
======================
1. Generate PIN
2. Use ATM
3. Exit

Your choice: 1

PIN generated successfully
Your generated PIN: 7485
Re-run the program and use ATM with this PIN

## File Used
| File        | Purpose                  |
| ----------- | ------------------------ |
| `ATM.c`     | Main program source code |
| `pin.txt`   | Stores generated PINs    |
| `README.md` | Project documentation    |


## ⚙️ How to Compile and Run

### 🖥️ On Windows (using GCC via MinGW)
```bash
gcc ATM.c -o ATM.exe
./ATM.exe
