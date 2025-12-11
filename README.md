# UrbanRide: Cab Booking System Analysis 🚖

## 📌 Project Overview
**UrbanRide** is a relational database project designed to simulate and analyze the operations of a cab booking service. This project demonstrates the entire data lifecycle: from schema design and normalization to complex data extraction and business intelligence reporting.

The goal of this project is to use SQL to answer critical business questions regarding fleet management, customer behavior, and revenue optimization.

## 🛠️ Tech Stack
* **Database:** MySQL / SQL Server (Compatible with standard SQL syntax)
* **Language:** SQL
* **Concepts Used:**
    * DDL (Data Definition Language) & DML (Data Manipulation Language)
    * Joins (Inner, Left)
    * Aggregate Functions (`SUM`, `COUNT`, `AVG`)
    * Date & Time Manipulation (`TIMESTAMPDIFF`, `DATE_FORMAT`)
    * Common Table Expressions (CTEs)
    * Conditional Logic (`CASE WHEN`)

## 📂 Database Schema
The database `cab_booking` consists of 6 relational tables:

1.  **Customers**: Stores customer profiles and join dates.
2.  **Drivers**: Stores driver details.
3.  **Cabs**: Contains vehicle information including type (Sedan/SUV) and registration.
4.  **Bookings**: The core transactional table linking Customers, Drivers, and Cabs with booking status and fare.
5.  **TripDetails**: Stores operational metrics like trip start/end times and distance covered.
6.  **Feedback**: Captures customer ratings and comments for quality assurance.

## 📊 Key Business Insights
This project includes advanced SQL queries to solve the following business problems:

### 1. Customer Loyalty & Behavior
* Identified top customers based on booking frequency to potential loyalty programs.
* Analyzed feedback to correlate ratings with specific drivers.

### 2. Operational Efficiency
* **Wait Time Analysis:** Calculated the average time difference between booking and trip start to identify pickup locations with supply shortages.
* **Peak Time Analysis:** Determined the busiest days of the week to optimize driver shifts.

### 3. Revenue Intelligence
* **Fare Analysis:** Compared revenue generation between Cab Types (SUV vs. Sedan).
* **Trip Categorization:** Used CTEs to categorize trips into Short, Medium, and Long distances to see which segment drives the most revenue.
* **Weekend vs. Weekday:** Analyzed fare differences between weekend and weekday operations.

### 4. Route Optimization
* Identified the top 3 most frequently traveled routes (Pickup vs. Dropoff) to plan driver allocation.

## 📝 Code Structure
The SQL script is divided into two main parts:
1.  **Schema Creation & Data Insertion:** Creating tables and populating them with dummy data.
2.  **Data Analysis Queries:** A series of 10+ analytical queries answering specific business prompts.

## 🚀 How to Run
1.  **Prerequisite:** Ensure you have MySQL Workbench or any SQL client installed.
2.  **Create Database:** Run the `CREATE DATABASE cab_booking;` command.
3.  **Execute Script:** Copy and paste the full SQL script to create tables and insert records.
4.  **Run Queries:** Execute the analytical queries at the bottom of the script individually to view insights.

## 🔮 Future Improvements
* Implement a dashboard using Power BI or Tableau connected to this database.
* Add a `Payment` table to track payment methods (Cash, Card, Wallet).
* Create a stored procedure to automatically calculate fares based on distance.

---
