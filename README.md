# Home-Harbor-Database

HomeHarbor-Essentials-Database-SQL-Project

This project involves the creation and population of a relational database for HomeHarbor Essentials, an online retail business specializing in Home and Kitchen products. The database is designed to efficiently store and manage crucial information such as Stock, Customer Details, Orders, Suppliers, Payments, and Returns.

Table of Contents

Overview
Database Structure
Entity-Relationship Diagram (ERD)
Key Entities and Relationships
Database Population
Queries and Views
Triggers
DataMart Integration
Database Structure

Entity-Relationship Diagram (ERD)

The ERD serves as the blueprint for the database, outlining the relationships between various entities within the system. The main entities include:

Customer
Supplier
Orders
OrderItems
Stock
Payments
Returns
Key Entities and Relationships

Customer and Suppliers: Separate entities with no direct relationship.
Orders and Customers: One-to-many relationship.
OrderItems and Stock: Many-to-one relationship.
Orders and OrderItems: One-to-many relationship.
Payments and Orders: One-to-many relationship.
Returns and Orders/Stock: Two one-to-many relationships.
Screenshot 2024-04-26 at 18 15 10
Database Population

The database is populated with dummy data to simulate real-world operations. This ensures the integrity and functionality of the database design.

Queries and Views

Key Queries

Weekly Transactions View: Shows all transactions for a given week.
Stock Levels by Supplier: View of stock purchased by supplier.
Total Stock Sold by Supplier: View of total stock sold, grouped by supplier.
Monthly Sales Transactions: Details and totals of all sales for the month-to-date.
Yearly Sales Transactions: Details and totals of all sales for the year-to-date.
Sales Growth Percentage: Displays the growth in sales/services from the first month of opening until now.
Returns to Date: Displays all returns to date.
Views

Specific views from the above queries are added to the HomeHarbor DataMart for enhanced analytical capabilities.

Triggers

A trigger is created to update stock levels whenever a sale takes place, ensuring real-time inventory management.

DataMart Integration

The project includes the creation of a DataMart, integrating views from queries 1, 3, and 4 to facilitate efficient data analysis.

Please find SQL Project Script: https://github.com/mohamedabdelnasser414/HomeHarbor-Essentials-Database-SQL-Project/blob/main/ProjectScript.sql
