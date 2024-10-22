# Pet Shop 🐾

## Overview

**Pet Shop** is an e-commerce web application designed for selling pet-related products such as food, accessories, toys, and more. The platform allows users to browse products, add them to their cart, and securely purchase them. This project is built using PHP, JavaScript, and MySQL as the database.

## Features

- User authentication and account management (Login, Register)
- Product catalog with categories and search functionality
- Shopping cart and checkout system
- Admin panel for managing products and orders
- Secure payment integration
- User-friendly design with responsive UI

## Tech Stack

- **Backend**: PHP
- **Frontend**: JavaScript, HTML, CSS
- **Database**: MySQL
- **Server**: Apache or Nginx (Localhost or Cloud-based)

## Installation and Setup Instructions

### Prerequisites

Before you begin, ensure you have the following installed on your local machine:

- [XAMPP](https://www.apachefriends.org/index.html) or [WAMP](https://www.wampserver.com/) (for running Apache and MySQL)
- PHP (v7.4 or higher)
- MySQL (v5.7 or higher)
- Composer (optional for managing PHP dependencies)

### Steps to Set Up the Project Locally

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/pet-shop.git
   cd pet-shop
   ```

2. **Set Up Database**

   - Open `phpMyAdmin` (usually available at `http://localhost/phpmyadmin`).
   - Create a new database:
     ```sql
     CREATE DATABASE petshop_db;
     ```
   - Import the SQL file located in the `database` folder (i.e., `petshop_db.sql`):
     - In phpMyAdmin, go to the database you created, then click on **Import** and upload the `petshop_db.sql` file.
  
3. **Configure the Project**

   - Open the project folder and locate the configuration file `config.php` (or `.env` if you're using one).
   - Update the database connection settings as per your MySQL credentials:
     ```php
     // config.php example
     $dbHost = 'localhost';
     $dbUser = 'root';
     $dbPass = '';
     $dbName = 'petshop_db';
     ```

4. **Start Apache and MySQL**

   - Open XAMPP/WAMP and start **Apache** and **MySQL** services.
   - Visit the application at `http://localhost/pet-shop` (or wherever your project is hosted locally).

5. **Install Dependencies (Optional)**

   If you are using any PHP libraries that require Composer, run:
   ```bash
   composer install
   ```

### Admin Login Details (Default)

- **Username**: `admin`
- **Password**: `admin123`

You can modify these credentials through the database under the `users` table.

## Usage

- **Browse Products**: Navigate to the homepage to explore available pet-related products.
- **Add to Cart**: Users can add items to their shopping cart and proceed to checkout.
- **Manage Products (Admin)**: Admins can log in to the admin panel to add, update, or delete products from the inventory.
- **Place an Order**: Users can complete their purchase by filling out their payment details.

## Contributing

Feel free to submit a pull request or raise an issue if you want to contribute or report bugs.
