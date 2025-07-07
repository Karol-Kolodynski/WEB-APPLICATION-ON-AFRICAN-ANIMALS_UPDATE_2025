# Web Application on African Animals

## 🐘 Description

Project created as part of an engineering thesis entitled. **‘Web application about African animals ’**. The application contains educational content about African fauna and an extensive social network-like user system. Everything runs on a local XAMPP server with web application security.

---

## ⚙️ Technologies used

- **Frontend**: HTML, CSS
- **Backend**: PHP
- **Database**: MySQL (phpMyAdmin)
- **Security**: reCAPTCHA, PHPMailer
- **Running environment**: Local XAMPP server

---

## 🔐 Main functions and security

### 1. user registration
- Data transmitted in **XML** format.
- Protection against **XML Injection** and **SQL Injection**.
- Passwords are **hashed** before being stored in the database.
- Default user role: `guest`.

### 2. User login
- Data verification via **safe SELECT**.
- Resistance to **SQL Injection** and **dictionary attack**.
- ‘Forgot password’ option. - sending a reset form.
- Notification system for the administrator.

### 3. Password reset.
- Check for the existence of an e-mail in the database.
- Secure link with **two-step verification** (2FA).
- Protection against **account emulation**, **time attacks** and **phishing**.

### 4 User file management
- Registered users can add, download, edit and delete their files.
- Support for graphics (.jpg, .png, .svg) and PDF files.
- File thumbnails in the user gallery.
- Protection against **Remote Code Execution (RCE)** and **Command Injection**.

### 5 Downloading files.
- Users can download the files of others.
- Interface with thumbnails and search engine.
- Protection against **DOM XSS** and **Path Traversal**.

### 6. Comments
- Option to add a comment under another user's gallery.
- Comments can only be deleted by the administrator.
- Protection against **Stored XSS**, **Code Injection** and **Cookie Theft**.

### 7 Welcome and personalisation
- Personalised greeting upon login.
- Ability to change the appearance of the page and message settings.
- Protection against **SSTI (Server-Side Template Injection)**.

### 8. Conversion of image files.
- Users can provide a URL to an image which will be converted to `.jpg` format.
- Image added to profile after processing.
- Protection against **SSRF (Server-Side Request Forgery)**.
