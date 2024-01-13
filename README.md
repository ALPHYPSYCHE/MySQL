![Ali Amirshahi Banner](https://i.ibb.co/2WKr9HR/github-banner-small.png)

<a href="https://github.com/ALPHYPSYCHE">
    <div style="margin-bottom:1em;"> 
        <img style="margin-right:-.2em;" align="left" src="https://cdn.worldvectorlogo.com/logos/mysql-logo.svg" alt="php)" title="PHP" width="100" height="100"/>
    </div>
    <div style="margin-bottom:-1.5em;">
        <h1 display="display:inline;">
            <font size="+4">MySQL Tutorial</font>
        </h1>
    </div>
</a>

<div style="margin-left:5em;">
    <span style="vertical-align: middle;"><font size="+2">This MySQL tutorial covers the basics of setting up MySQL, performing CRUD (Create, Read, Update, Delete) operations, and some advanced concepts.
</font></span>
</div>
﻿

## 📚 Table of Contents

1. [Introduction](#introduction)
2. [Basic Commands](#basic-commands)
3. [Advanced Concepts](#advanced-concepts)

## Introduction
MySQL is a popular open-source relational database management system (RDBMS) that is widely used for web applications. It provides a robust and scalable platform for managing and manipulating data.

## Basic Commands
Connecting to MySQL
```bash
mysql -u username -p
```
Replace username with your MySQL username. You'll be prompted to enter the password.

Creating a Database
```sql
CREATE DATABASE tutorialDB;
```
Creating Tables
```sql
USE tutorialDB;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50),
    email VARCHAR(100)
);
```
Inserting Data
```sql
INSERT INTO users (username, email) VALUES ('user1', 'user1@example.com');
INSERT INTO users (username, email) VALUES ('user2', 'user2@example.com');
```
Querying Data
```sql
SELECT * FROM users;
```
Updating Data
```sql
UPDATE users SET email = 'newemail@example.com' WHERE id = 1;
```
Deleting Data
```sql
DELETE FROM users WHERE id = 2;
```
## Advanced Concepts
Indexing
```sql
CREATE INDEX idx_username ON users (username);
```
Joins
```sql
SELECT users.username, orders.order_id
FROM users
INNER JOIN orders ON users.id = orders.user_id;
```
Transactions
```sql
START TRANSACTION;
-- SQL statements
COMMIT;
```

