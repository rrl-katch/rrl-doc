# 🚌 RRL Bus Ticketing System

Professional Bus Ticket Booking & Management System.

The system contains only two panels:

1. 🎫 Station Booking Panel  
2. ⚙️ Admin Panel  

---

## 📌 System Overview

### 🎫 Station Booking Panel
Used for:
- Ticket booking
- Ticket printing with QR Code
- Duplicate ticket print
- Daily summary
- Settlement management

### ⚙️ Admin Panel
Used for:
- Station management
- Agent management
- Route & fare configuration
- Reports & summaries
- System settings

---

# 🚀 Project Setup Guide

## 1️⃣ Install Git

Download & Install Git:

https://github.com/git-for-windows/git/releases/download/v2.53.0.windows.1/Git-2.53.0-64-bit.exe

After installation, verify installation by running:

git --version

---

## 2️⃣ Install XAMPP (IMPORTANT)

Download XAMPP 7.4.1:

https://sourceforge.net/projects/xampp/files/XAMPP%20Windows/7.4.1/xampp-windows-x64-7.4.1-1-VC15-installer.exe/download

### Recommended Installation Path:

D:\xampp

If D drive does not exist, create it.

---

## 3️⃣ Enable Required PHP Extension

Open:

D:\xampp\php\php.ini OR open xampp-control.exe and Apache -> Configure -> php.ini

Find:

;extension=intl

Remove the semicolon to enable:

extension=intl

Restart Apache after saving.

---

## 4️⃣ Clone the Project

Open Command Prompt and run:

cd D:\xampp\htdocs

git clone https://github.com/rrl-katch/rrl.git

When prompted:
- Enter provided username
- Enter provided Git Token (NOT password)

Configure Git (One-Time Setup):

git config --global user.name "rrl-katch"

git config --global user.email "rrl.katch@gmail.com"

⚠️ **IMPORTANT:** After cloning the repository, update the lock station in start_app_rrl.bat file.

---

⚠️ If the project is not installed inside:

D:\xampp\htdocs\rrl

You must update:
- start_app.bat
- Any hardcoded project paths

---

## 5️⃣ Database Setup

Start XAMPP:
- Start Apache
- Start MySQL

Open:

http://localhost/phpmyadmin/

Create a database named:

rrl

Click Create.

Import the database:

- Select database rrl
- Click Import
- Choose file: rrl_database.sql (inside project folder)
- Click Go

---

## 6️⃣ Start Application

Open in browser:

http://localhost/rrl/

---

# 🔐 Panel URLs

Station Booking Panel:
http://localhost/rrl/

Admin Panel:
http://localhost/rrl/admin

(Default credentials will be provided separately.)

---

# 📁 Important Folders

public/uploads/qrcode/   → Ticket QR Code Images  
application/             → Core Application Logic  
start_app.bat            → Auto Start Script  

---

# 🛠 Daily Development Workflow

Before starting work each day:

git fetch origin
git reset --hard origin/main

(If using start_app.bat, this runs automatically.)

---

# 🔄 Common Issues

Apache Not Starting:
- Check if Port 80 is already in use
- Stop IIS if enabled

MySQL Not Starting:
- Ensure no other MySQL service is running

404 Error:
Ensure project path is:
D:\xampp\htdocs\rrl

Database Error:
- Confirm database name is rrl
- Ensure MySQL is running

---

# 📦 Environment Details

PHP Version: 7.4  
MySQL: XAMPP Default  
Framework: CodeIgniter  
Environment: Localhost  

---

# ✅ Setup Checklist

✔ Git Installed  
✔ XAMPP Installed in D Drive  
✔ intl Extension Enabled  
✔ Project Cloned in htdocs  
✔ Database Created (rrl)  
✔ SQL Imported  
✔ Apache & MySQL Running  
✔ Application Accessible  

---

# 🚌 RRL Bus Ticketing System

Professional • Secure • Reliable
