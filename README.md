📚 Library Management System (LMS)
🚀 Manage your library effortlessly with our LMS
The Library Management System (LMS) is a powerful tool designed to automate and streamline daily library operations, including book management, member registrations, book issuing/returning, and comprehensive reporting. Built with MySQL, this system provides an efficient and scalable solution for library administrators.

🌟 Key Features
📖 Book Management

Add, update, and remove books.
Track available and issued copies.
👥 Member Management

Register new members and manage existing ones.
Update member details seamlessly.
🔄 Book Transactions

Issue books to members with due dates.
Track and update returned books.
🔎 Search & Filter

Search for books by title, author, or category.
List overdue books and calculate fines (optional).
📊 Reporting

View issued books, available books, and detailed transaction logs.
🛠️ Tech Stack
Database: MySQL
Languages: SQL
Tools: SQL Queries, Foreign Key Constraints
⚙️ MySQL Queries Used
Insert Queries: To add new books, members, and transactions.
Update Queries: To modify book availability and member info.
Select Queries: To fetch data like available books, issued books, and overdue books.
Join Queries: To connect tables for reporting and transactions.
Foreign Key Constraints: To maintain integrity between members and books in the database.
📂 Database Schema
Books Table

BookID (INT): Primary Key
Title (VARCHAR), Author (VARCHAR), Category (VARCHAR)
AvailableCopies (INT)
Members Table

MemberID (INT): Primary Key
Name (VARCHAR), Email (VARCHAR UNIQUE)
PhoneNumber (VARCHAR)
IssuedBooks Table

IssueID (INT): Primary Key
BookID (INT FOREIGN KEY), MemberID (INT FOREIGN KEY)
IssueDate (DATE), ReturnDate (DATE)
Returned (BOOLEAN)
