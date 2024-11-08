# ATM Transaction System

This project is a basic ATM Transaction System implemented in C. It allows users to perform various banking operations such as checking their balance, withdrawing cash, and depositing cash, with a PIN-based security check.

## Features

- **Balance Check**: Displays the user's current account balance.
- **Withdraw Cash**: Allows the user to withdraw cash if they have sufficient funds.
- **Deposit Cash**: Enables the user to deposit cash into their account.
- **PIN Security**: Requires a user PIN (default: 1669) to access the ATM services.
- **Exit Option**: Provides a way for users to exit the ATM system.

## How It Works

1. **PIN Verification**: Users are prompted to enter their PIN before accessing the ATM functions. The system will reject incorrect PIN entries and request a valid PIN.
2. **Main Menu**: After successful PIN entry, users can choose from the following options:
    - Check Balance
    - Withdraw Cash
    - Deposit Cash
    - Exit
3. **Transaction Continuation**: After completing a transaction, users are prompted to either perform another transaction or exit.

## Program Flow

The program runs in a loop, continuously prompting the user for their PIN until the correct one is entered. After successful PIN verification, the user can perform the following actions:

- **Check Balance**: Displays the current balance.
- **Withdraw Cash**: Allows the user to withdraw a specified amount. If the withdrawal amount exceeds the current balance, an "Insufficient Balance" message is displayed.
- **Deposit Cash**: Prompts the user to enter an amount to deposit, which is then added to their current balance.
- **Exit**: Ends the session and displays a thank you message.

## Code Structure

- The code uses a `while` loop to verify the PIN.
- A `do-while` loop enables the continuation of transactions until the user decides to exit.
- A `switch` statement handles the different transaction options.

## Example Usage

ENTER YOUR SECRET PIN NUMBER: 1669  
NAMASKAAR  
Welcome to ATM SERVICES

- CHECK BALANCE  
- WITHDRAW CASH  
- DEPOSIT CASH  
- EXIT  

Enter your choice: 1

YOUR BALANCE IN Rs: 25000

DO YOU WISH TO HAVE ANOTHER TRANSACTION? (y/n): y


## How to Run

1. Copy the code into a `.c` file (e.g., `atm_transaction.c`).
2. Compile the code using a C compiler, such as GCC:

    ```bash
    gcc atm_transaction.c -o atm_transaction
    ```

3. Run the executable:

    ```bash
    ./atm_transaction
    ```

## Requirements

- A C compiler (e.g., GCC) to compile and run the program.
