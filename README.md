Banking System using Object Oriented Programming in C++ with multiple banking functionalities
# Banking System using Object-Oriented Programming in C++

## Project Description

This project is a simple console-based banking system implemented using **Object-Oriented Programming (OOP)** in C++. It allows users to perform typical banking operations such as opening an account, making deposits, withdrawing funds, closing an account, and checking the balance.

### Features:
- **Open Account**: Create a new account by providing first name, last name, and an initial balance.
- **Deposit**: Add money to the account.
- **Withdraw**: Withdraw money from the account, ensuring a minimum balance of $500 is maintained.
- **Balance Enquiry**: Check the current balance of an account.
- **Close Account**: Close an account and delete the related data.
- **Show All Accounts**: Display details of all active accounts.

## Technologies Used
- **C++**: The main programming language used for this project.
- **OOP**: The project employs core OOP principles like classes, inheritance, and encapsulation.
- **File Handling**: Account details are stored in a file for session persistence.

## Getting Started

### Prerequisites
You need a C++ compiler (like g++, clang++) installed on your system.

### Compilation and Execution

1. **Clone the repository**:
    ```bash
    git clone <https://github.com/lkhatri7/Banking_system.git>
    ```

2. **Compile the code**:
    ```bash
    g++ -o banking_system main.cpp
    ```

3. **Run the executable**:
    ```bash
    ./banking_system
    ```

## How the Project Works

### Account Class

The `Account` class represents a bank account and includes details like:
- Account Number
- First Name
- Last Name
- Balance

It supports basic operations like deposit, withdrawal, and data persistence through file handling.

### Bank Class

The `Bank` class manages multiple accounts using a `std::map` with the account number as the key. It performs operations such as:
- Opening a new account
- Balance inquiry
- Depositing and withdrawing money
- Closing accounts
- Displaying all accounts

### Minimum Balance

The system enforces a **minimum balance of $500**. If a withdrawal results in a balance below this limit, an `InsufficientFunds` exception is thrown.

## File Handling

Account details are saved in the `Bank.data` file for persistence. Whenever an account is opened, closed, or modified, the file is updated.

## Future Enhancements
- Adding user authentication for more secure access to accounts.
- Implementing a graphical user interface (GUI).
- Supporting multiple account types such as savings and current accounts.

