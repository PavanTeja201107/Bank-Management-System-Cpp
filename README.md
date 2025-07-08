# Bank-Management-System-Cpp

A robust, secure, and scalable terminal-based application written in **C++** that simulates core banking functionalities such as account creation, authentication, deposits, withdrawals, fund transfers, and transaction history tracking using **OOP**, **Stacks**, and **File I/O**.

## Features

- **Secure Authentication** using dynamically generated **tokens and PINs**
- **Transaction History** tracking using a custom **stack-based structure**
- **Fund Transfers** between accounts with full validation
- **Data Persistence** with structured file output using `ofstream`
- **Time-based unique IDs** using `chrono`
- **Constant-Time Access** to accounts using `unordered_map`
- **Menu-Driven Interface** for intuitive CLI interaction

## Technologies and Libraries

- **Language:** C++
- **Libraries Used:**
  - `<iostream>`, `<fstream>`, `<stack>`, `<unordered_map>`, `<string>`, `<chrono>`

## Key Components

**createAccount()**
Generates unique account number and token using chrono, verifies user input, and stores new accounts in an unordered_map.

**accessAccount()**
Provides secure access using token and PIN.

**deposit() / withdraw()**
Performs balance update after validations, logs transaction in a stack.

**transfer()**
Transfers funds securely between two verified accounts, logs transactions for both.

**TransactionStack**
A stack implementation to store, view, and export last N transactions.

**saveAccountToFile()**
Writes account data and recent transactions to accounts.txt, ensuring persistence across sessions.

## How to Compile and Run (Locally)
**On Windows/Linux/macOS:**
Make sure you have g++ installed. Open terminal inside the project folder:
Command for compilation: g++ main.cpp -o bankApp
Command for output: ./bankApp           # Use bankApp.exe if you're on Windows CMD
## OUTPUT: 
# Menu
![image](https://github.com/user-attachments/assets/21631ca4-28fc-4fbb-b7dc-c941097c3982)
# Sample Output
![image](https://github.com/user-attachments/assets/d6e90f33-64f8-4811-b51e-e6c371c479d4)

