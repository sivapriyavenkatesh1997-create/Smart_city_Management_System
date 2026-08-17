# Smart_city_Management_System
The Smart City Management System is a centralized database management project developed using MySQL to manage and analyze essential city services.

The system integrates multiple government departments and provides a structured platform for managing:

Citizens
Properties
Property Tax
Water Supply
Electricity Consumption
Waste Collection
Public Complaints
Traffic Violations
Government Service Requests
Employees and Departments
The project demonstrates how SQL can be used to manage large-scale government data and generate meaningful business insights for smart-city administration.

Business Objective

The Smart City Corporation needs a centralized system to monitor:

Citizen distribution across zones
Property ownership and valuation
Property tax collection
Water consumption and billing
Electricity consumption and billing
Waste collection efficiency
Complaint resolution
Traffic violations and fines
Government service requests
Employee and department performance
Overall city revenue
The project uses SQL analytics to transform this operational data into useful management information.

Technologies Used

Technology| Purpose MySQL| Database Management MySQL Workbench| SQL Development SQL| Data Management & Analytics Power BI| Dashboard & Visualization GitHub| Project Version Control

Database Structure

The database contains the following major tables:

SMART_CITY │ ├── ZONE ├── CITIZEN ├── PROPERTY ├── PROPERTY_TAX ├── WATER_CONNECTION ├── ELECTRICITY_CONNECTION ├── WASTE_COLLECTION ├── COMPLAINT ├── TRAFFIC_VIOLATION ├── SERVICE_REQUEST └── EMPLOYEE

Main Relationships

ZONE │ └── CITIZEN │ └── PROPERTY │ └── PROPERTY_TAX │ ├── WATER_CONNECTION │ └── ELECTRICITY_CONNECTION

CITIZEN ├── COMPLAINT ├── TRAFFIC_VIOLATION └── SERVICE_REQUEST

ZONE └── WASTE_COLLECTION

EMPLOYEE └── EMPLOYEE (Self Join / Manager Relationship)

Dataset

The project contains sample data for:

Entity| Records Zones| 10 Citizens| 200 Properties| 150 Property Tax Records| 150 Water Connections| 100 Electricity Connections| 100 Waste Collection Records| 100 Complaints| 150 Traffic Violations| 100 Service Requests| 150 Employees| 50

SQL Concepts Implemented

Basic SQL

CREATE DATABASE
CREATE TABLE
INSERT
SELECT
UPDATE
Constraints
Primary Keys
Foreign Keys
UNIQUE
NOT NULL
CHECK
SQL Functions

UPPER()
LOWER()
LEFT()
LENGTH()
MONTH()
MONTHNAME()
MAX()
MIN()
AVG()
SUM()
COUNT()
SQL Analytics

GROUP BY
HAVING
ORDER BY
Aggregate Functions
JOIN Operations

INNER JOIN
LEFT JOIN
RIGHT JOIN
FULL OUTER JOIN equivalent using UNION
SELF JOIN
CROSS JOIN
Multi-table JOIN
Subqueries

Single-row Subqueries
Multiple-row Subqueries
Nested Subqueries
Correlated Subqueries
Advanced SQL

EXISTS
NOT EXISTS
UNION
UNION ALL
INTERSECT
EXCEPT
Views
Indexes
Regular Expressions
Date & Time

CURRENT_DATE()
CURRENT_TIMESTAMP()
TIMESTAMPDIFF()
DATEDIFF()
YEAR()
MONTH()
MONTHNAME()
Database Administration

CREATE USER
ALTER USER
GRANT
REVOKE
DROP USER
INFORMATION_SCHEMA
👁️ Views Created

CITIZEN_PROFILE_VIEW

Provides:

Citizen Name
Zone Name
Property Type
Property Address
Property Value
TAX_COLLECTION_VIEW

Provides:

Zone Name
Total Tax Collected
COMPLAINT_STATUS_VIEW

Provides:

Citizen Name
Complaint Type
Complaint Status
Smart City Analytics

The project generates analytical reports including:

Top 10 Zones by Tax Collection
Identifies zones generating the highest property-tax revenue.

Zone-wise Citizen Distribution
Analyzes the number of citizens living in each zone.

Complaint Resolution Analysis
Measures Open, In Progress, and Resolved complaints.

Utility Consumption Analysis
Analyzes water and electricity consumption.

Traffic Fine Collection
Analyzes violations and total fines collected.

Service Request Performance
Measures government service requests by status.

Water Consumption Dashboard
Analyzes water consumption and billing by zone.

Electricity Consumption Dashboard
Analyzes electricity usage and billing by zone.

Waste Collection Efficiency
Measures waste collection volume and collection activity.

Smart City Revenue Dashboard
Combines major revenue sources such as:

Property Tax
Traffic Fines
Water Bills
Electricity Bills
Power BI Dashboard

The MySQL database can be connected directly to Power BI for visualization.

Recommended dashboard pages:

City Overview

Total Citizens
Total Properties
Total Tax Collected
Total Complaints
Total Service Requests
Total City Revenue
Utilities & Operations

Water Consumption by Zone
Electricity Consumption by Zone
Waste Collection by Zone
Utility Revenue
Citizen Services

Complaint Status
Complaint Categories
Service Request Status
Service Types
Traffic Violations
Traffic Fine Collection
How to Run the Project

Step 1 — Install MySQL

Install MySQL Server and MySQL Workbench.

Step 2 — Create Database

CREATE DATABASE SMART_CITY;

USE SMART_CITY;

Step 3 — Run SQL Script

Open:

SQL/smart_city_management.sql

Run the script in MySQL Workbench.

Step 4 — Verify Tables

SHOW TABLES;

Step 5 — Verify Records

SELECT COUNT() FROM CITIZEN; SELECT COUNT() FROM PROPERTY; SELECT COUNT(*) FROM COMPLAINT;

Step 6 — Connect to Power BI

Open Power BI Desktop:

Get Data ↓ MySQL Database ↓ Server: localhost ↓ Database: SMART_CITY ↓ Load Tables

Project Structure

Smart-City-Management-System/ │ ├── README.md │ ├── SQL/ │ └── smart_city_management.sql │ ├── Screenshots/ │ ├── database_tables.png │ ├── query_results.png │ └── dashboard.png │ └── Dashboard/ └── smart_city_dashboard.pbix

Key Business Insights

This project can help city management answer questions such as:

Which zones generate the highest tax revenue?
Which zones have the highest citizen population?
Which complaint category occurs most frequently?
What percentage of complaints are resolved?
Which zones consume the most water?
Which zones consume the most electricity?
Which traffic violations generate the highest fines?
Which government services receive the most requests?
Which zones generate the most waste?
What is the total smart-city revenue?
Learning Outcomes

Through this project, the following skills were developed:

Relational Database Design
SQL Programming
Data Cleaning
Data Generation
Database Constraints
Joins
Subqueries
Advanced SQL
Data Analysis
Business Intelligence
Power BI Dashboard Development
Database Administration
GitHub Project Management
Project Author

R.SIVAPRIYA
BE-ECE,
sivapriyavenkatesh1997@gmail.com

Project

Smart City Management System

Technologies

"MySQL" "SQL" "Power BI" "GitHub"

Future Enhancements

Future versions of the project can include:

Real-time IoT utility monitoring
AI-based complaint classification
Predictive traffic violation analysis
Water demand forecasting
Electricity consumption forecasting
Automated tax collection alerts
Mobile application for citizens
Real-time smart-city monitoring dashboard
Machine Learning-based city service prediction
License

This project is created for educational and portfolio purposes.
