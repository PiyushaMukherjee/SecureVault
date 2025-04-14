# Save the finalized README.md with all content merged into a single, formal document
full_readme = """
# 🔒 Secure File Hiding System with OTP Verification (Java + MySQL)

A Java-based desktop application designed to enable users to securely hide, reveal, and manage sensitive files with an additional layer of OTP-based email verification. This application leverages technologies such as JavaMail API, MySQL, and Maven to offer a robust and privacy-focused file management system.

---

## 📌 Features

- ✅ User registration and login secured with OTP verification via email
- 🔐 Encrypts and stores files securely in the database
- 📂 Allows users to unhide and restore files to their original location
- 📬 Sends OTP emails using JavaMail API and Gmail App Password
- 🗃️ Utilizes MySQL for storing user and file metadata
- ⚙️ Built with Maven for streamlined dependency management and portability

---

## 🛠️ Tech Stack

| Layer         | Technology         |
|---------------|--------------------|
| Language      | Java               |
| Database      | MySQL              |
| Email Service | JavaMail API (SMTP)|
| Build Tool    | Maven              |
| IDE           | IntelliJ IDEA      |

---

## 🔧 Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/secure-file-hider.git
cd secure-file-hider
CREATE DATABASE securefiledb;
USE securefiledb;

CREATE TABLE user (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100),
    email VARCHAR(100) UNIQUE
);

CREATE TABLE data (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(255),
    path VARCHAR(500),
    email VARCHAR(100),
    bin_data LONGTEXT
);
String url = "jdbc:mysql://localhost:3306/securefiledb";
String user = "root";
String password = "your_mysql_password";
return new PasswordAuthentication(from, "your_app_password");
mvn clean compile
