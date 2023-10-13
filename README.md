# Universal Login Authentication Project

This project provides a universal solution for user registration and login features that can be integrated into web development projects. It includes user registration, password hashing, and a secure login system.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Built With](#built-with)
- [Authors](#authors)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Prerequisites

- A web server or hosting environment with PHP and MySQL support.
- Access to a MySQL database or phpMyAdmin.

## Installation

1. **Create a Database:**

   Create a MySQL database using phpMyAdmin or your preferred method. Remember the database name for later use in the project.

2. **Create the Users Table:**

   Run the following SQL command to create a `users` table in your database. This table will store user information, including email and hashed passwords.

   ```sql
   CREATE TABLE users (
       id INT PRIMARY KEY AUTO_INCREMENT,
       email VARCHAR(255) NOT NULL,
       password VARCHAR(255) NOT NULL
   );
   ```

3. **Update Configuration:**

   - In the `signup.php` file at line 24, update the following line with the actual name of your database:

     ```php
     $dbname = "database"; // Replace "database" with your actual database name
     ```

   - Similarly, in the `index.php` file at line 21, replace "database" with your actual database name:

     ```php
     $dbname = "database"; // Replace "database" with your actual database name
     ```

   - In the `index.php` file at line 42, update the `header('Location: home.php');` line with the actual path you want users to go after a successful login.

4. **Deploy the Project:**

   Upload the project files to your web server or hosting environment.

## Usage

Users can now access your registration and login system through the `signup.php` and `index.php` pages. They can register an account and then log in using their credentials.

## Built With

- PHP
- MySQL

## Authors

- [Your Name](https://github.com/yourusername)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Bootstrap](https://getbootstrap.com/) for the front-end framework.
```

Feel free to replace the placeholders with actual data and links to your GitHub profile or other relevant resources.
