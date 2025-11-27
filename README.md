⭐ DhanSetu – Bank Management System

DhanSetu is a console-based Bank Management System built using Java, MySQL, and JDBC.
It demonstrates core concepts of software development, relational databases, and object-oriented programming through essential banking operations.

📘 1. Introduction

DhanSetu provides a structured and secure environment for basic banking tasks such as account creation, login, balance management, transactions, and record maintenance.
The project is designed primarily for academic learning.

🛠️ 2. Features
👤 User Features

Create New Account

Secure Login Authentication

Check Balance

Deposit Amount

Withdraw Amount

Transfer Funds

View Transaction History

🛡️ Admin Features

View All Customer Accounts

View All Transaction Records

Add / Update / Delete Customer Details

💽 System Features

MySQL Database Integration

JDBC using Prepared Statements

Auto Timestamp for All Transactions

Structured Modules and Error Handling

🏗️ 3. Technologies Used
Component	Technology
Language	Java (JDK 8+)
Database	MySQL 8.0
Connectivity	JDBC (MySQL Connector/J)
Paradigm	Object-Oriented Programming
Tools	VS Code / IntelliJ / Eclipse, MySQL Workbench
🗄️ 4. Database Design
📂 Database Tables
users

user_id (PK)

name

email

password

accounts

account_number (PK)

user_id (FK)

balance

transactions

transaction_id (PK)

account_number (FK)

type (deposit/withdraw/transfer)

amount

timestamp

🧱 Database Setup
CREATE DATABASE bankmanagementsystem;
USE bankmanagementsystem;
SOURCE queries.sql;

📂 5. Project Structure
DhanSetu/
│
├── src/
│   ├── database/
│   ├── model/
│   ├── services/
│   └── ui/
│
├── lib/
├── bin/
├── queries.sql
└── README.md

⚙️ 6. Setup & Execution
Step 1: Configure Database Credentials

Edit DBConnection.java:

String url = "jdbc:mysql://localhost:3306/bankmanagementsystem";
String user = "root";
String password = "yourpassword";

Step 2: Compile
javac -cp "lib/*;." -d bin src/**/*.java

Step 3: Run
java -cp "lib/*;bin" ui.Login

📌 7. Limitations

Console-based interface

Password hashing not implemented (unless done manually)

Not optimized for concurrent multi-user transactions

🚀 8. Future Enhancements

JavaFX or Swing GUI

Encrypted password storage

Email/SMS alerts

PDF export for statements

Loan/EMI Module

Admin dashboard UI

🏁 9. Conclusion

DhanSetu demonstrates core concepts of:

Java programming

JDBC connectivity

SQL database operations

Object-oriented design

Real-world banking workflows

It is ideal for academic submission, learning, and portfolio projects.
