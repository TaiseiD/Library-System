# Library-System
A PHP-MySQL Library Management System that manages books, students, publishers, and borrow records. Supports full CRUD operations, organized folder structure, and clean UI with CSS. Users can add, view, edit, or delete data easily via the web interface using XAMPP server

---

## ⚙️ SETUP INSTRUCTIONS

### 🧩 Step 1: Install and Open XAMPP
Make sure you have **XAMPP** installed on your computer.  
If not, download it here 👉 [https://www.apachefriends.org](https://www.apachefriends.org).

Then:
- ✅ Start **Apache**
- ✅ Start **MySQL**

---

### 🗃️ Step 2: Create the Database
1. Open your browser and go to [http://localhost/phpmyadmin](http://localhost/phpmyadmin).  
2. Click on the **SQL** tab.  
3. Copy and paste the contents of the file: database_setup.sql
4. Click **Go** to execute the script.  
- This will create the database **`booksactivity`** and all the necessary tables.

---

### 📂 Step 3: Place the Project in XAMPP Folder
1. Open **File Explorer**.  
2. Navigate to: C:\xampp\htdocs
3. Copy your project folder **Booksactivity** into the `htdocs` directory.

✅ Example path:C:\xampp\htdocs\Booksactivity


---

### 🌐 Step 4: Access the System
Once everything is ready, open your browser and go to:

👉 [http://localhost/Booksactivity/index.php](http://localhost/Booksactivity/index.php)

---

# 📁 Project Folder Structure — Booksactivity

```markdown
Booksactivity/
│
├── assets/
│   ├── form.css
│   ├── index.css
│   ├── nav.css
│   └── read.css
│
├── database/
│   └── connection.php
│
├── function/
│   ├── book/
│   │   ├── createBookFunc.php
│   │   ├── deleteBookFunc.php
│   │   ├── showBookFunc.php
│   │   └── updateBookFunc.php
│   │
│   ├── borrow/
│   │   ├── createBorrowFunc.php
│   │   ├── showBorrowFunc.php
│   │   └── updateBorrowFunc.php
│   │
│   ├── publisher/
│   │   └── (publisher functions here)
│   │
│   └── student/
│       └── (student functions here)
│
├── interface/
│   ├── book/
│   │   ├── addBook.php
│   │   ├── readBook.php
│   │   └── updateBook.php
│   │
│   ├── borrow/
│   │   ├── addBorrow.php
│   │   ├── readBorrow.php
│   │   └── updateBorrow.php
│   │
│   ├── navigation/
│   │   └── navigation.php
│   │
│   ├── publisher/
│   │   ├── addPublisher.php
│   │   ├── readPublisher.php
│   │   └── updatePublisher.php
│   │
│   └── student/
│       ├── addStudent.php
│       ├── readStudent.php
│       └── updateStudent.php
│
├── database_setup.sql
└── index.php
```

---

## 🧠 Notes

- Always make sure **Apache** and **MySQL** are **running** in XAMPP before opening the project.
- Database connection settings are located in: database/connection.php
- You can edit your credentials there (default username: `root`, password: `""`).
- To import the SQL file manually, open phpMyAdmin → Import → Select `database_setup.sql` → Click **Go**.

---

## 🧹 Common Fixes

**❌ Problem:** “Failed to connect to database”  
✅ **Fix:** Make sure MySQL is running, and check your `connection.php` credentials.

**❌ Problem:** “404 Not Found”  
✅ **Fix:** Ensure the folder name inside `htdocs` is exactly **Booksactivity** (case-sensitive).

**❌ Problem:** “Access denied”  
✅ **Fix:** Check if you have permission to access the directory, or run XAMPP as Administrator.

---

## 👨‍💻 Developer Notes

This system supports:
- CRUD operations for Books, Borrow Records, Students, and Publishers
- Organized folder structure for scalability
- Easy deployment using XAMPP on localhost

---

🪶 *Developed using PHP, MySQL, HTML, and CSS.*


