🛒 Zepto E-commerce SQL Data Analyst Portfolio Project
This is a real-world Data Analyst portfolio project based on an e-commerce inventory dataset scraped from Zepto, one of India’s fastest-growing quick-commerce companies.

The project simulates the workflow of a real data analyst, starting from raw data exploration to business-focused data analysis using SQL. It demonstrates how SQL can be used to transform raw inventory data into meaningful business insights.

This is also my first SQL Data Analyst portfolio project, created to practice real-world analytical thinking and build a strong data portfolio.
Project Overview

The main objective of this project is to simulate how data analysts in e-commerce companies analyze product and inventory data using SQL.

Through this project, I performed tasks such as:

✅ Setting up a structured database from a raw dataset

✅ Performing Exploratory Data Analysis (EDA) to understand the dataset

✅ Cleaning messy data and handling missing values

✅ Writing business-driven SQL queries to extract meaningful insights

Tools Used

The analysis in this project was performed using:

MySQL

Dataset Source: Kaggle

Dataset Overview

The dataset contains product inventory data similar to what an e-commerce platform would maintain.

Each row represents a unique product SKU (Stock Keeping Unit). Some product names appear multiple times because the same product may exist in different sizes, weights, or package quantities, which is common in real e-commerce catalogs.

Columns in the Dataset

sku_id – Unique identifier for each product

name – Product name

category – Product category (Fruits, Snacks, Beverages, etc.)

mrp – Maximum Retail Price of the product

discountPercent – Discount percentage applied

discountedSellingPrice – Final selling price after discount

availableQuantity – Units available in inventory

weightInGms – Product weight in grams

outOfStock – Indicates whether the product is out of stock

quantity – Number of items per package

Project Workflow
1. Database & Table Creation

First, I created a SQL table with appropriate data types to store the dataset.

CREATE TABLE zepto (
  sku_id INT PRIMARY KEY,
  category VARCHAR(120),
  name VARCHAR(150),
  mrp FLOAT,
  discountPercent FLOAT,
  availableQuantity INT,
  discountedSellingPrice FLOAT,
  weightInGms INT,
  outOfStock BIT,
  quantity INT
);
2. Data Import

The dataset was imported from a CSV file into the SQL database.

3. Data Exploration (EDA)

During the exploration stage, I analyzed the dataset to understand its structure and patterns.

Key analysis included:

Counting total number of products

Identifying different product categories

Checking for missing or null values

Comparing in-stock vs out-of-stock products

Identifying duplicate product names with different SKUs

4. Data Cleaning

To ensure accurate analysis, the dataset was cleaned by:

Removing rows with invalid price values

Handling missing or inconsistent data

Standardizing price formats where necessary

5. Business Insights Using SQL

Several SQL queries were written to extract meaningful business insights from the dataset.

Examples include:

Identifying top discounted products

Finding high-price products currently out of stock

Calculating average price per product category

Identifying products offering the best value for money

Ranking categories with the highest average discounts

Analyzing inventory distribution across categories
Why This Project Matters

This project demonstrates how SQL can be used to analyze real-world business data. It highlights the types of tasks data analysts perform in industries such as e-commerce, retail, and product analytics.

Since this is my first SQL portfolio project, the focus was on applying SQL concepts to solve realistic business problems and generate actionable insights.


About Me

I am an aspiring Data Analyst passionate about working with data and solving business problems using SQL and analytics.

This project is part of my journey to build practical experience and a strong data analytics portfolio.



