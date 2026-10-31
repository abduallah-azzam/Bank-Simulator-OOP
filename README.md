# Bank Management System

A console banking application written in C++ using object-oriented programming. It manages clients, transactions, users with permissions, and currency exchange.

## Features
- **Clients:** add, update, delete, find, and list clients
- **Transactions:** deposit, withdraw, total balances (also shown in words), and transfers between clients with a transfer log
- **Users:** login with a 3-attempt lockout, user management, and bitwise role-based permissions
- **Login register:** records every login with a timestamp
- **Currency exchange:** list, find, and update rates, and a currency calculator

## OOP Design
- **Inheritance:** `clsBankClient` and `clsUser` inherit from `clsPerson`; all screens inherit from `clsScreen`
- **Encapsulation:** private members with property getters and setters
- **Static factory methods:** such as `Find` and `GetAddNewClientObject`
- **Modes:** each object works in Empty, Update, or AddNew mode

## Tech Stack
- C++ (Visual Studio, Windows only)
- Data stored in text files: `Clients.txt`, `Users.txt`, `Currencies.txt`, `LoginRegister.txt`, `TransfersLog.txt`

## Notes
- Passwords are stored with a simple character-shift cipher. It is for learning only and is not secure.
- Built while following the Programming Advices C++ course; helper classes such as `clsString`, `clsDate`, and `clsInputValidate` come from the course.
