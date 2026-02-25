# 🚌 RRL Bus Ticketing System

**Professional Bus Ticket Booking & Management Platform**

A secure, high-performance ticketing system designed for transport
operators to manage station bookings, ticket issuance, settlements, and
centralized administration.

------------------------------------------------------------------------

# 📘 Table of Contents

1.  System Architecture\
2.  Panel Overview\
3.  System Requirements\
4.  Installation Guide\
5.  Database Configuration\
6.  Application Launch\
7.  Panel Access URLs\
8.  Project Structure\
9.  Daily Development Workflow\
10. Troubleshooting Guide\
11. Environment Specifications\
12. Final Setup Checklist

------------------------------------------------------------------------

# 🏗 System Architecture

The system consists of two operational panels:

-   🎫 Station Booking Panel (Operational Use)
-   ⚙️ Admin Panel (Administrative Control)

Each panel is role-based and designed for specific operational
responsibilities.

------------------------------------------------------------------------

# 🎫 Panel Overview

## 1️⃣ Station Booking Panel

### Key Features

-   Ticket booking with real-time validation
-   Thermal ticket printing with QR Code
-   Duplicate ticket reprint
-   Daily transaction summary
-   Settlement and reconciliation management
-   Agent-based booking tracking

------------------------------------------------------------------------

## 2️⃣ ⚙️ Admin Panel

### Key Capabilities

-   Station management
-   Agent management
-   Route configuration
-   Fare management
-   System-wide reports & summaries
-   Printer configuration
-   System settings & controls

------------------------------------------------------------------------

# 💻 System Requirements

## Minimum Requirements

-   Windows OS (Recommended: Windows 10/11)
-   PHP 7.4
-   MySQL (via XAMPP)
-   Apache Server
-   Git

## Recommended Installation Path

D:`\xampp`{=tex}

------------------------------------------------------------------------

# 🚀 Installation Guide

## 1️⃣ Install Git

Verify installation:

git --version

------------------------------------------------------------------------

## 2️⃣ Install XAMPP (MANDATORY)

Install to:

D:`\xampp`{=tex}

------------------------------------------------------------------------

## 3️⃣ Enable Required PHP Extension (intl)

Open:

D:`\xampp`{=tex}`\php`{=tex}`\php`{=tex}.ini

Find:

;extension=intl

Change to:

extension=intl

Restart Apache.

------------------------------------------------------------------------

## 4️⃣ Clone the Project

cd D:`\xampp`{=tex}`\htdocs  `{=tex} git clone
https://github.com/rrl-katch/rrl.git

Configure Git:

git config --global user.name "rrl-katch"\
git config --global user.email "rrl.katch@gmail.com"

Run:

setup.bat

Project must be located at:

D:`\xampp`{=tex}`\htdocs`{=tex}`\rrl`{=tex}

------------------------------------------------------------------------

# 🗄 Database Configuration

1.  Start Apache & MySQL\
2.  Open http://localhost/phpmyadmin/\
3.  Create database: rrl\
4.  Import rrl_database.sql

------------------------------------------------------------------------

# ▶️ Application Launch

Station Panel:\
http://localhost/rrl/

Admin Panel:\
http://localhost/rrl/admin

------------------------------------------------------------------------

# 📁 Project Structure

rrl/ │ ├── application/ ├── public/uploads/qrcode/ ├── start_app.bat ├──
setup.bat └── rrl_database.sql

------------------------------------------------------------------------

# 🛠 Daily Development Workflow

git fetch origin\
git reset --hard origin/main

------------------------------------------------------------------------

# 🔄 Troubleshooting

Apache Not Starting: - Check Port 80 conflict - Stop IIS

MySQL Not Starting: - Ensure no other MySQL service is running

Database Error: - Confirm database name is rrl - Ensure MySQL is running

intl Error: - Ensure extension=intl is enabled - Restart Apache

------------------------------------------------------------------------

# 📦 Environment Specifications

PHP: 7.4\
Framework: CodeIgniter\
Server: Apache\
Environment: Localhost

------------------------------------------------------------------------

# ✅ Setup Checklist

✔ Git Installed\
✔ XAMPP Installed\
✔ intl Extension Enabled\
✔ Project Cloned\
✔ Database Created\
✔ SQL Imported\
✔ Apache Running\
✔ MySQL Running\
✔ Application Accessible

------------------------------------------------------------------------

# 🚌 RRL Bus Ticketing System

Professional • Secure • Reliable
