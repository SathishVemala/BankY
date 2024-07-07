
# Bank Simulation Project

## Project Overview

This project is a simulation of a basic banking system that allows users to create accounts, deposit and withdraw funds, and transfer funds between accounts. The system persists account data using serialization, ensuring that account information is saved and loaded between sessions.

## Requirements

- **Java Development Kit (JDK) 8 or higher**
- **Integrated Development Environment (IDE) or command-line tools to compile and run Java programs**
- **File system access to store and read the serialized account data (`accounts.dat` file)**

## Project Structure

- `Account.java`: Represents a bank account with basic functionalities like deposit, withdrawal, and transfer.
- `Bank.java`: Manages multiple bank accounts, including creating new accounts and saving/loading account data to/from a file.
- `Main.java`: Provides a command-line interface for users to interact with the banking system.

## How the Project is Developed

1. **Account Class**:
    - Implements the `Serializable` interface to enable object serialization.
    - Contains attributes like `accountNumber`, `accountHolderName`, and `balance`.
    - Provides methods for depositing, withdrawing, and transferring funds.
    - Overrides `toString` method to display account information.

2. **Bank Class**:
    - Manages a collection of `Account` objects using a `HashMap`.
    - Provides methods to create accounts, retrieve accounts, and display all accounts.
    - Implements methods to save and load account data to/from a file using serialization.

3. **Main Class**:
    - Implements a command-line interface to interact with the user.
    - Provides options to create accounts, deposit, withdraw, transfer funds, and display all accounts.
    - Uses a `Scanner` object to read user input.

## How to Use the Project

1. **Compile the Project**:
    - Open a terminal or command prompt.
    - Navigate to the project directory.
    - Compile the Java files using the following command:
      ```sh
      javac Main.java
      ```

2. **Run the Project**:
    - After compiling, run the project using the following command:
      ```sh
      java Main
      ```

3. **Interact with the Command-Line Interface**:
    - Follow the on-screen prompts to interact with the banking system.
    - Options include creating accounts, depositing funds, withdrawing funds, transferring funds, and displaying all accounts.

## Example Output

```plaintext
1. Create Account
2. Deposit
3. Withdraw
4. Transfer
5. Show All Accounts
6. Exit
Choose an option: 1
Enter account number: 12345
Enter account holder name: John Doe
Account created successfully.
1. Create Account
2. Deposit
3. Withdraw
4. Transfer
5. Show All Accounts
6. Exit
Choose an option: 2
Enter account number: 12345
Enter amount to deposit: 1000
Deposit successful.
1. Create Account
2. Deposit
3. Withdraw
4. Transfer
5. Show All Accounts
6. Exit
Choose an option: 5
Account Number: 12345, Account Holder: John Doe, Balance: 1000.0
1. Create Account
2. Deposit
3. Withdraw
4. Transfer
5. Show All Accounts
6. Exit
Choose an option: 6
```

## Conclusion

This project demonstrates a simple banking system implemented in Java with object serialization to persist data. Users can create accounts, deposit and withdraw funds, transfer funds between accounts, and view account information through a command-line interface. The system ensures data persistence by saving and loading account information to and from a file.
