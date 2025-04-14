#Secure File Hiding System with OTP Verification (Java + MySQL)
This is a Java-based desktop application that enables users to securely hide, reveal, and manage sensitive files with OTP-based email verification. The application employs JavaMail API for email services, MySQL for data storage, and Maven as the build tool, ensuring a secure and structured approach to file management.

## Features

- User registration and login with OTP verification via email
- Secure file hiding using encryption and database storage
- File restoration to the original path upon unhide
- Email-based OTP functionality using JavaMail API and Gmail App Password
- Persistent storage of user and file data using MySQL
- Built using Maven for efficient dependency management

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
