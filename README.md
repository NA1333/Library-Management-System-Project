# Library Management System-Project
The Library Management System (LMS) is designed to manage and automate the day-to-day operations of a library. It allows librarians to manage books, members, and book transactions (issue and return) efficiently. The system is built using MySQL as the database, which stores all data related to books, members, transactions, and optionally, librarian authentication and book categories.
Key Features of This Project:
Book Management:
Add, update, and remove books from the database.
Keep track of available and issued copies of each book.
Member Management:
Register new members, track member details, and update information.
Book Issuing and Returning:
Issue books to members and track due dates.
Mark books as returned and update the available copies.
Search and Filter:
Search books by title, author, or category.
List overdue books and calculate fines (if implemented).
Reporting:
View issued books, available books, and detailed transaction logs.
MySQL Queries Used:
Insert Queries: To add new books, members, and transaction records.
Update Queries: To update information about book availability and member details.
Select Queries: To fetch information like available books, issued books, and overdue books.
Join Queries: To combine data from multiple tables (e.g., books and members for transactions).
Foreign Key Constraints: Used to maintain referential integrity between related tables (e.g., linking members and books in the IssuedBooks table).
SQL Data Types and Keys:
1. Data Types:
INT: Used for unique IDs (e.g., BookID, MemberID, IssueID).
VARCHAR(n): For storing text data such as book titles, author names, member names, emails, and phone numbers.
DATE: To store issue dates, return dates, and membership join dates.
BOOLEAN: For tracking return status (Returned field in IssuedBooks table).
AUTO_INCREMENT: Applied to primary keys to generate unique identifiers automatically.
2. Keys:
Primary Key: Uniquely identifies each record in a table.
Example: BookID in the Books table, MemberID in the Members table.
Foreign Key: Establishes a link between two tables, ensuring that records in one table correspond to valid records in another.
Example: MemberID in IssuedBooks refers to MemberID in the Members table, and BookID in IssuedBooks refers to BookID in the Books table.
Unique Key: Enforces uniqueness in certain columns.
Example: Email in the Members table to ensure no duplicate registrations.
