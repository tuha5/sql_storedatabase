Store Database Management System

A MySQL database project for managing customer orders, products, and sales data with practice queries and views.

📋 Project Overview

This project creates a complete relational database for an e-commerce store system with:

• Customer management

• Product catalog

• Order processing

• Sample data population

• SQL practice queries

• Custom database views

🛠️ Technologies Used

• MySQL / MariaDB

• SQL (DDL, DML, DQL)

• Database relationships (Primary Keys, Foreign Keys)

• JOIN operations

• Aggregate functions

• Database views

📁 Files Included

• store_db.sql - Complete database creation script with sample data

• history.sql - Execution history (not included in repository)

🚀 Getting Started

Prerequisites

• MySQL Server installed

• MySQL Workbench or similar client

• Basic understanding of SQL commands

Installation Steps

1. Create the database:
   mysql -u your_username -p < store_db.sql
   

2. Verify the database was created:
   SHOW DATABASES;
   USE store_db;
   SHOW TABLES;
   

3. Check sample data:
   SELECT * FROM customers LIMIT 5;
   SELECT * FROM products LIMIT 5;
   SELECT * FROM orders LIMIT 5;
   

📊 Database Schema

The database consists of three main tables:

1. Customers Table

• Stores customer information including names, contact details, and customer type

• Tracks total spending and registration date

• Uses ENUM for customer type (REGULAR/PREMIUM)

2. Products Table

• Contains product catalog with descriptions and pricing

• Tracks stock quantities and creation dates

• Organized by categories (Electronics, Home Appliances, etc.)

3. Orders Table

• Records customer orders with dates, amounts, and status

• Foreign key relationship with customers table

• Status tracking (PENDING, PROCESSING, SHIPPED, DELIVERED, CANCELLED)

🔍 Practice Queries

The script includes several practice queries demonstrating:

• INNER JOIN: List all orders with customer names

• LEFT JOIN: List all customers and their orders (including those without orders)

• Finding customers without orders: Using LEFT JOIN with IS NULL condition

• Counting orders per customer: Using GROUP BY and aggregate functions

• Premium customers analysis: Finding premium customers with their latest order

• Complex filtering: Customers who spent more than $100

📈 Advanced Features

Database Views

• customer_order_history: A comprehensive view showing customer details with their order history

• Includes status descriptions for better readability

• Can be queried like a regular table

Additional Analytics

• Monthly revenue analysis by date grouping

• Customer lifetime value calculation

• Premium customer performance metrics

📚 What I Learned

Through this project, I gained practical experience in:
. Database
1 Design: Creating normalized tables with proper relationships
2. SQL Syntax: Mastering DDL (Data Definition Language) and DML (Data Manipulation Language)
3. Table Relationships: Implementing primary and foreign keys effectively
4. JOIN Operations: Understanding INNER JOIN vs LEFT JOIN and their applications
5. Aggregate Functions: Using COUNT, SUM, MAX, and GROUP BY for data analysis
6. Database Views: Creating reusable query templates for complex reports
7. Data Filtering: Advanced WHERE clause usage with date ranges and conditions
8. Data Validation: Ensuring data integrity through constraints and proper data types
9. Query Optimization: Writing efficient queries for better performance
10. Real-world Application: Building a functional e-commerce database system

🎯 Key Takeaways

• Normalization: Understanding how to structure data efficiently

• Data Integrity: Using constraints to maintain quality data

• Query Efficiency: Learning to write queries that perform well with larger datasets

• Business Logic: Implementing features like customer types and order statuses

• Reporting: Creating views and aggregated data for business insights

📈 Future Enhancements

Potential improvements for this project:

• Add user authentication system

• Implement inventory management

• Create stored procedures for common operations

• Add triggers for automatic updates

• Build a simple front-end interface

• Add more complex reporting and analytics

• Implement payment processing integration

🤝 Contributing

Feel free to fork this repository and submit pull requests for improvements or additional features.

📝 License

This project is for educational purposes and personal learning.

Author: MOIN UDDIN TUHA 
Date: 04.03.2026 
GitHub: tuha5
