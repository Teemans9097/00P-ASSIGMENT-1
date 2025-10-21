# Mini Library Management System

## Overview
The Mini Library Management System is a simple Python-based project designed to manage books, members, and borrowing operations in a library. It includes features for adding, updating, deleting, searching, borrowing, and returning books, as well as maintaining member details.  
The system demonstrates the core concepts of modular programming, data structure management, and role-based access.

---

## Project Structure
MiniLibrarySystem
├── operations.py # Core backend logic (books, members, borrow/return)
├── demo.py # Console-based demo interface
├── tests.py # Simple test script to verify operations
└── README.md # Project documentation


---

## Features
- Add, update, and delete books  
- Add, update, and delete members  
- Borrow and return books with stock tracking  
- Search books by title or author  
- Record and view borrow history  
- Basic user login for admin, staff, and student roles  

---

## Roles and Permissions
| Role     | Access Level | Description |
|-----------|---------------|-------------|
| **Admin** | Full Access | Can manage books, members, and borrowing |
| **Staff** | Moderate Access | Can assist with borrowing and returning |
| **Student** | Limited Access | Can view and borrow books |

---

## How to Run

### 1. Clone or Download
Copy the project folder or clone from your repository (if applicable):
```bash
git clone https://github.com/yourusername/minilibrarysystem.git
cd minilibrarysystem
python demo.py
python tests.py
Basic tests passed. If you see this message, tests ran without immediate assertion failures.
from operations import add_book, add_member, borrow_book, return_book

add_book("B001", "Python Basics", "John Smith", "Programming", 3)
add_member("M001", "Alice", "alice@email.com")
borrow_book("B001", "M001")
return_book("B001", "M001")
System Flow

Books and Members are stored in Python dictionaries.

Borrowing reduces the number of available copies.

Returning increases the number of available copies.

All actions are recorded in a borrow history list.

Tests verify core behaviors and handle errors gracefully.
