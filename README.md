PortfolioHub – Digital Portfolio Management System

Project Overview

PortfolioHub is a web-based digital portfolio management system developed for the **Multimedia Technology and Animation** degree program at the **University of Dodoma**. It allows students and creatives to register, log in, and manage their artwork and project portfolios online.

The system provides a shared gallery where all registered users can browse each other's work, while each user has full control over their own entries.



Degree Program
Multimedia Technology and Animation

Group Number
Group 6

Team Members
| Name                                         | Registration Number |
|------                                        |-------------------|
| SOLO JANGU WILLIAM                           | T24-03-22618 |
| Member 2                                     | [Reg. No.] |
| Member 3                                     | [Reg. No.] |






Features

User Management – Register, login, and logout securely with hashed passwords
Add Portfolio Items – Store artwork/project title, category, description, tools used, date, and optional image
Display Portfolio – Browse all portfolio entries in a responsive card gallery
My Portfolio – View and manage only your own submissions
Search – Search portfolio items by keyword, description, tools used, or category
Edit & Delete – Full CRUD control over your own items
Image Upload – Upload project images (JPG, PNG, GIF, WEBP up to 5MB)



Technologies Used

| Technology | Purpose |
|------------|---------|
| PHP 7.4+   | Server-side logic |
| MySQL      | Database storage |
| HTML5/CSS3 | Frontend structure and styling |
| XAMPP      | Local development server (Apache + MySQL) |



Installation Steps

Prerequisites
[XAMPP](https://www.apachefriends.org/) (or any LAMP/WAMP stack)
PHP 7.4 or higher
MySQL 5.7 or higher

Setup Instructions

1. Clone the repository
   ```bash
   git clone https://github.com/[YourUsername]/OpenSource_Assignment_MTA_Group[N].git
   ```

2. Move to XAMPP's web root
   ```bash
   # Windows
   move OpenSource_Assignment_MTA_Group[N] C:\xampp\htdocs\portfolio

   # Linux/Mac
   mv OpenSource_Assignment_MTA_Group[N] /opt/lampp/htdocs/portfolio
   ```

3. Start XAMPP – Start Apache and MySQL services

4. Configure database credentials 
   Open `db.php` and update:
   ```php
   define('DB_USER', 'root');   // your MySQL username
   define('DB_PASS', '');       // your MySQL password
   ```

5. Create uploads folder (if not present)
   ```bash
   mkdir portfolio/uploads
   chmod 777 portfolio/uploads   # Linux/Mac only
   ```

6. Visit the app in your browser
   ```
   http://localhost/portfolio/register.php
   ```
   The database and tables are created automatically on first run.

---
File Structure

```
portfolio/
├── db.php              ← Database connection & auto-setup
├── auth_check.php      ← Session authentication guard
├── navbar.php          ← Reusable navigation component
├── register.php        ← User registration
├── login.php           ← User login
├── logout.php          ← Session destruction
├── index.php           ← Main gallery (all portfolio items)
├── add.php             ← Add new portfolio item
├── edit.php            ← Edit existing item
├── delete.php          ← Delete item
├── view.php            ← View single item details
├── search.php          ← Search/filter portfolio items
├── my_portfolio.php    ← User's own portfolio manager
├── css/
│   └── style.css       ← Main stylesheet
├── uploads/            ← Uploaded project images
└── README.md           ← This file
```

---

Git Commands Used

```bash
# Initialize repository
git init

# Add remote origin
git remote add origin https://github.com/[YourUsername]/OpenSource_Assignment_MTA_Group[N].git

# Stage all files
git add .

# Commit with message
git commit -m "Initial project setup and database config"
git commit -m "Added user registration and login"
git commit -m "Implemented portfolio entry form"
git commit -m "Added display and listing of portfolio items"
git commit -m "Implemented search feature"

# Create development branch
git checkout -b development

# Merge development into main
git checkout main
git merge development

# Push to GitHub
git push -u origin main
```

---

GitHub Repository Link
https://github.com/sollo-kane/OpenSource_Assignment_MTA_Group_6.git


