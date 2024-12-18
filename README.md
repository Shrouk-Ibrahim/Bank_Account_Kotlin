
# Bank Account Project

This Kotlin project simulates a simple banking system that allows users to create and manage different types of bank accounts. It provides functionalities for creating a **Debit**, **Credit**, or **Checking** account, and allows users to make deposits or withdrawals based on the account type.

## Features

- **Account Creation**: Users can choose from three types of accounts:
    - Debit Account
    - Credit Account
    - Checking Account
- **Deposit and Withdrawal Operations**:
    - Users can deposit money into their account.
    - Users can withdraw money from their account, with checks for sufficient balance.
- **Account Balance Management**:
    - The account balance is randomly initialized between 0 and 1000 dollars.
    - Account balances are updated with every transaction (deposit or withdrawal).

## How It Works

1. **Starting the Program**:
    - The program prompts the user to choose the type of account they wish to create.
    - If the user provides an invalid input, the program will ask them to try again (up to 3 attempts).

2. **Bank Operations**:
    - After creating an account, users can make either a deposit or withdrawal.
    - For **Debit accounts**, users can withdraw money if they have sufficient balance.
    - For **Credit accounts**, users can make deposits to reduce the debt balance.

3. **Exit**:
    - After each set of operations, users are asked whether they want to perform another operation or create a new account.
    - The program terminates when the user chooses not to create another account.

## Code Structure

- **`BankAccountProject` class**:
    - Contains the main logic for the banking system.
    - Has methods to handle:
        - Account creation.
        - Deposit and withdrawal operations.
        - Balancing and handling errors like insufficient funds.

- **Key Methods**:
    - `debitWithdraw(amount: Int)`: Handles withdrawal from debit accounts.
    - `creditDeposit(amount: Int)`: Handles deposit to credit accounts.

## Example Flow

- **Account Type Selection**:
  ```
  What type of account would you like to create?
  1 - Debit account
  2 - Credit account
  3 - Checking account
  Choose an option (1, 2, or 3): 1
  ```

- **Deposit and Withdrawal Operations**:
  ```
  Would you like to make a deposit or withdrawal? (deposit/withdraw): deposit
  Enter amount: 100
  You successfully deposited 100 dollars. The new balance is 100 dollars.
  ```

- **Handling Errors**:
  ```
  Can't withdraw, no money on this account!
  ```

## Requirements

- Kotlin 1.3 or higher.
- An IDE such as IntelliJ IDEA for running the Kotlin code.

## How to Run the Project

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/Shrouk-Ibrahim/Andriod.git
   ```
2. Open the project in IntelliJ IDEA or any Kotlin-supported IDE.
3. Run the `BankAccountProject` class.



