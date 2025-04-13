# Expense Tracker (Mini Project -1)

## Overview

The Personal Expense Tracker is an end-to-end SQL-based project built to empower users in managing, analyzing, and visualizing their personal financial data. This project merges robust database design with advanced querying and an interactive dashboard interface to provide both technical learning and practical financial insights.

It serves a dual purpose:

### 🎓 Educational Resource:

It’s designed for learners and professionals to strengthen their understanding of SQL database management, from table design and data normalization to complex analytical queries using aggregations, joins, and window functions.

### 💰 Financial Management Tool:

As a real-world personal finance application, it enables users to track income and expenses, categorize financial transactions, and visualize trends over time — making it a valuable tool for personal budgeting and decision-making.

## 🔍Core Features:
A relational SQL database with normalized schema for managing expenses and income

### Scripts for:

* Database creation

* Sample data insertion (manual + Faker-generated)

* Basic and advanced SQL queries

### A Streamlit-powered interactive dashboard for:

* Filtering transactions

* Viewing summaries and statistics

* Visualizing trends and categories

### Real-world insights like:

* Monthly income vs. expenses

* Category-wise spending

* Anomaly detection in financial behavior

## 🛠️ Tech Stack:
* SQL (SQLite or PostgreSQL) – Core database logic

* Python – For scripting, data generation, and analytics

* Streamlit – Interactive UI/UX for the dashboard

* Faker – For realistic data simulation

* Matplotlib/Seaborn – For visual insights

* Pandas – Data wrangling and aggregation

## 🛠️ Data Generation Using Faker Library
To simulate realistic expense tracking scenarios, the Faker library was utilized to generate synthetic financial data for both expenses and income. Faker is a Python library that allows you to generate fake data such as names, addresses, dates, and numerical values, which is particularly useful for testing and prototyping applications without relying on sensitive or real user data.

### 🎯 Purpose of Using Faker
Testing Functionality: Generating varied and large volumes of data helped test SQL queries, visualizations, and analytics features across different categories and timeframes.

Realistic Simulation: Randomized dates, amounts, descriptions, and categories closely mimic real-world spending and earning patterns, enhancing the authenticity of analysis.

Safe Demonstration: By avoiding real financial data, this method ensures privacy and security while showcasing how the tracker functions with real-like inputs.

## 🗄️ Integration with SQLite3
To ensure lightweight, efficient, and portable data storage and querying, this project uses SQLite3 — a self-contained, serverless SQL database engine that is built into Python. It offers the full power of SQL without the overhead of installing and managing a full-fledged database server.

### 💡 Why SQLite3?
Zero Configuration: No server installation or setup required. Perfect for standalone applications and prototyping.

Lightweight & Fast: Ideal for personal finance projects and small-to-medium datasets.

Native Python Support: Comes bundled with Python’s standard library, allowing seamless integration using the sqlite3 module.

### 🧩 How It Was Integrated
* A new database file (e.g., expense_tracker.db) was created automatically on script execution.

* Python’s sqlite3 module was used to:

  - Establish database connections

  - Create tables for Expenses, Income, Categories, and IncomeSources

  - Insert generated data from the Faker library

  - Execute analytical SQL queries for insights and visualization

* Transactions were managed using cursors, with changes committed and the connection closed cleanly after operations.

### 🧮 Real-time Querying for Analytics
All data analysis — including category-wise expenses, monthly income vs expenses, and time-series trends — is powered by live SQL queries run on the SQLite database. These results are displayed interactively within the Streamlit dashboard, offering a robust and responsive experience.

### 🔗 Benefits of SQLite in This Project
* Simplifies the backend setup, especially for beginners.

* Enables smooth local development and testing.

* Makes it easy to move, copy, or back up the entire database (just one .db file).

* Compatible with tools like DB Browser for SQLite for visual database exploration.

## 📊 Streamlit App
To provide a user-friendly interface for visualizing and interacting with the personal finance data, this project includes a Streamlit dashboard built on top of the SQLite3 database. The app transforms raw financial data into meaningful charts, tables, and summaries — all rendered in real-time.

### 🎯 Purpose of the Streamlit App
The Streamlit app acts as the frontend layer of the project, allowing users to:

* View summaries of their monthly expenses and income

* Explore category-wise spending trends

* Analyze income vs. expense over time

* Filter data based on custom date ranges

* Gain insights using dynamic visualizations

### 🛠️ Key Features
* Dashboard Layout: A clean, modern interface with intuitive navigation and interactive elements.

* Live Data Querying: Direct connection to the SQLite3 database allows real-time data updates.

* Visualizations:

  - Line charts for tracking trends over time

  - Bar and pie charts for category breakdowns

  - Tables with formatted financial entries

* Interactive Filters:

  - Date range selector

  - Category dropdown

  - Toggle between expenses and income views

* Summarized Insights: Total spending, savings, top categories, and comparisons displayed with KPIs and metrics.

### ⚙️ How It Works
* When the app is launched using streamlit run, it connects to the SQLite database.

* SQL queries are executed based on user interactions (e.g., selected dates or categories).

* Data is processed and visualized using tools like Pandas and Plotly/Matplotlib.

* Results are displayed instantly in an interactive web interface hosted locally.

### 🧪 User Experience
No command-line knowledge is required to use the app. Users simply launch the dashboard and start interacting with their financial data using sliders, buttons, and dropdowns. All data is displayed in a way that is digestible and visually engaging.

### 📷 Sample Dashboard Screenshots:
**Project Introduction Page:**



