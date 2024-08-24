# Digital Wallet Management System

## Table of Contents:

1.Overview

2.Features

3.Prerequisites

4.How to Install and Run the Project

5.How to Use the Project

6.Tests

7.Screenshots/Media

8.Future

9.How to Contribute to the Project

10.License

11.Credits

12.Author

13.Conclusion

14.Connect with Me

## Overview

This project is a simple Digital Wallet Management System implemented in C++. The system manages user accounts, allowing users to transfer money between each other. It ensures that transfers only occur if the sending user has sufficient funds. After processing transactions, users are sorted by their balance and user ID.

## Features
1.**User Management:** The system manages multiple users, each with a unique ID and balance.

2.**Money Transfer:** Users can transfer funds to other users, with checks to ensure sufficient balance.

3.**Sorting:** After processing all transactions, users are sorted by balance (ascending). If two users have the same balance, they are sorted by user ID (ascending).

4.**Transaction Feedback:** For each transaction, the system outputs either "Success" or "Failure" based on whether the transfer was possible.

5.**Prerequisites**
A C++ compiler (e.g., g++)
Basic knowledge of C++ programming

## How to Install and Run the Project
1. **Clone the Repository**:
   First, clone the repository to your local machine:
   ```sh
   git clone https://github.com/Mandeindu/digital-wallet-management-system.git

2. **Navigate to the project directory:**

   cd Digital-Wallet-Management-System

3. **Compile the project:**
   make all

4. **Run the application:**

   ./wallet_manager


## How to Use the Project
**Input:**

Provide the number of users and their initial balances.
Specify the number of transactions and the details of each transaction (sender, receiver, and amount).

**Output:**

The program will output "Success" or "Failure" for each transaction.
After all transactions, it will display the sorted list of users by balance and user ID.

**Tests**
To test the functionality, create input files with various scenarios and redirect them to the program:

./digital_wallet < input.txt > output.txt
Compare output.txt with the expected results.

## Screenshots/Media:
![digital wallet 1](https://github.com/user-attachments/assets/6e317f1f-6c82-4da7-8888-73bb4698590b)
![Digital wallet 2](https://github.com/user-attachments/assets/15ab02e1-a2e0-4474-ab5c-d65e3e6c6e03)


## Future
Additional Features: Implement features like user authentication, transaction history, and more complex sorting algorithms.
Improved User Interface: Develop a graphical interface for easier interaction.

## How to Contribute to the Project
Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes and commit them (git commit -m 'Add new feature').
Push to the branch (git push origin feature-branch).
Open a Pull Request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Credits
Thank you to the C++ community for their invaluable resources and support.

## Author
Mandeindu

## Conclusion
This Digital Wallet Management System is a basic yet powerful tool for managing user accounts and transactions. It serves as a foundation for more complex financial systems.
