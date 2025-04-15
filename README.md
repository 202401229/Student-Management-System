Student Management System (Forked & Improved)

This is a command-line based Student Management System built in C++, forked from i-amsagar/Student-Management-System. 
The project allows adding, displaying, modifying, deleting, and searching student records with persistent storage using file handling.

As part of our Open Source Project Presentation (P3), we explored, reviewed, and improved this project by identifying and fixing functional and structural issues.

What We Fixed

1. Missing or Incorrect getdata() Calls
- Issue: The program did not call getdata() before writing a new student object, which resulted in garbage data being saved.
- Fix: Added a call to getdata() inside the write_student() function before writing to file.

2. Incorrect File Open Modes
- Issue: The program used incorrect or redundant file opening modes (like appending when overwriting was needed).
- Fix: Adjusted file modes where necessary (e.g., used ios::out for rewriting instead of ios::app).

3. No Input Validation
- Issue: The code accepted any kind of input for marks and roll numbers.
- Fix: Added basic validation to ensure only numeric values are accepted.

4. No Prompt to User Before Program Exit
- Issue: The program exited immediately after some operations.
- Fix: Added prompts and getch() or cin.get() statements to pause the output.

5. Code Formatting and Readability
- Issue: The code lacked consistent formatting and comments.
- Fix: Reformatted and added necessary comments.

Features

- Add new student record
- Display all student records
- Search student by roll number
- Modify student record
- Delete student record
- File-based data persistence

Project Structure

- main.cpp         : Main menu logic
- student.h        : Student class & declarations
- student.cpp      : Definitions of all operations
- data.txt         : Student records file
- README.md        : Project documentation

Concepts Used

- Object-Oriented Programming (C++)
- File Handling (Reading/Writing to files)
- Classes and Objects
- Function Separation for Modular Code
- Git & GitHub Workflow



Original Repository

Forked from: https://github.com/i-amsagar/Student-Management-System

Merged PR: https://github.com/i-amsagar/Student-Management-System/pull/XX

Learnings & Outcome

- Understood real-world open source collaboration
- Debugged legacy code and improved functionality
- Practiced version control and pull request workflows
- Explored C++ file handling and class-based design in-depth

