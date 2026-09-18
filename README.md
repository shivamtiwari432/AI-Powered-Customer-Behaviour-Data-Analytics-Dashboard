# 👨🏻‍💻 AI-Powered Customer Behaviour Data Analytics Dashboard

> An end-to-end Data Analytics portfolio project that demonstrates how raw customer shopping data can be transformed into actionable business insights using **Excel, Power Query, Python, SQL, and Power BI**.

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![Python](https://img.shields.io/badge/Python-EDA-3776AB?logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-Database-336791?logo=postgresql&logoColor=white)
![Excel](https://img.shields.io/badge/Excel-Data%20Source-217346?logo=microsoft-excel&logoColor=white)

---

# 📌 Overview

This project simulates a real-world **Customer Behaviour Analytics** workflow followed by professional Data Analysts.

The objective is to collect customer shopping data, clean and transform it, perform Exploratory Data Analysis (EDA), build a relational database, create business queries using SQL, and design an interactive Power BI dashboard that helps stakeholders make data-driven decisions.

The project follows an industry-standard analytics pipeline from **data collection to business reporting**.

---

# 🎯 Business Problem Statement

A leading retail company wants to better understand customer purchasing behaviour to improve:

- Customer Engagement
- Product Performance
- Sales Growth
- Marketing Strategy
- Customer Loyalty

### Business Question

> **How can customer shopping behaviour be analyzed to identify purchasing trends, improve customer engagement, and optimize product and marketing strategies?**

---

# 📂 Dataset

The dataset contains customer shopping behaviour information, including:

- Customer ID
- Age
- Gender
- Location
- Product Category
- Purchase Amount
- Quantity
- Payment Method
- Season
- Discount Applied
- Review Rating
- Purchase Date

---

# 🛠️ Tools & Technologies

| Tool | Purpose |
|-------|----------|
| Microsoft Excel | Data Source |
| Power Query | Data Cleaning & Transformation |
| Python (Pandas, NumPy) | Data Preparation & EDA |
| SQL (MySQL/PostgreSQL) | Business Analysis |
| Power BI | Dashboard Development |
| DAX | KPI Calculations |
| GitHub | Version Control |

---

# 🚀 Project Workflow

## 1️⃣ Data Collection

- Imported Excel dataset
- Verified data quality
- Checked missing values

---

## 2️⃣ Data Cleaning (Power Query & Python)

Performed:

- Removed duplicates
- Removed null values
- Corrected data types
- Renamed columns
- Standardized category names
- Handled inconsistent values
- Feature engineering

---

## 3️⃣ Exploratory Data Analysis (EDA)

Performed analysis on:

- Customer Demographics
- Product Categories
- Seasonal Sales
- Purchase Behaviour
- Discount Impact
- Payment Methods
- Customer Ratings
- Revenue Distribution

---

## 4️⃣ SQL Business Analysis

Created SQL queries to answer business questions such as:

- Top spending customers
- Best-selling categories
- Seasonal trends
- Average purchase value
- Customer segmentation
- Revenue by payment method
- Discount analysis

---

## 5️⃣ Power BI Dashboard

Developed an interactive dashboard containing:

- KPI Cards
- Monthly Sales Trend
- Customer Segmentation
- Product Category Analysis
- Revenue Distribution
- Customer Reviews
- Interactive Filters
- Navigation Buttons

---

# 📊 Business Requirements

## KPI Requirements

### ✅ Total Sales

```DAX
Total Sales =
SUM(Sales[Purchase Amount])
```

---

### ✅ Total Customers

```DAX
Total Customers =
DISTINCTCOUNT(Sales[Customer ID])
```

---

### ✅ Average Purchase

```DAX
Average Purchase =
AVERAGE(Sales[Purchase Amount])
```

---

### ✅ Total Orders

```DAX
Total Orders =
COUNTROWS(Sales)
```

---

### ✅ Customer Rating

```DAX
Average Rating =
AVERAGE(Sales[Review Rating])
```

---

# 📈 Dashboard Requirements

### 📌 Monthly Sales Trend

**Visual**

- Line Chart

Purpose:

Monitor monthly revenue trends.

---

### 📌 Sales by Product Category

**Visual**

- Bar Chart

Purpose:

Identify highest-performing product categories.

---

### 📌 Sales by Season

**Visual**

- Column Chart

Purpose:

Understand seasonal purchasing behaviour.

---

### 📌 Payment Method Analysis

**Visual**

- Donut Chart

Purpose:

Compare customer payment preferences.

---

### 📌 Customer Demographics

**Visual**

- Pie Chart
- Bar Chart

Purpose:

Analyze age and gender distribution.

---

### 📌 Top Customers

**Visual**

- Table

Purpose:

Identify high-value customers.

---

# 📊 DAX Measures

## Revenue

```DAX
Revenue =
SUM(Sales[Purchase Amount])
```

---

## Total Quantity

```DAX
Total Quantity =
SUM(Sales[Quantity])
```

---

## Average Order Value

```DAX
Average Order Value =
DIVIDE([Revenue],[Total Orders])
```

---

## Customer Count

```DAX
Customer Count =
DISTINCTCOUNT(Sales[Customer ID])
```

---

## Revenue by Category

```DAX
Revenue by Category =
CALCULATE(
    [Revenue],
    ALLEXCEPT(
        Sales,
        Sales[Category]
    )
)
```

---

# 📷 Project Screenshots

## 📌 Project Workflow

![Workflow](Images/project-workflow.png)

---

## 📌 Business Problem Statement

![Problem Statement](Images/problem_statement.png)

---

## 📌 Deliverables

- Data Preparation
- Python EDA
- SQL Analysis
- Power BI Dashboard
- Business Report
- Presentation
- GitHub Repository

![Deliverables](Images/deliverables.png)

---

## 📌 Power BI Dashboard

![Dashboard](Images/dashboard.png)

---

# 📈 Key Insights

- Identified customer purchasing trends
- Analyzed seasonal shopping behaviour
- Found high-value customer segments
- Compared payment preferences
- Evaluated product category performance
- Built an interactive dashboard for business decision-making

---

# 📂 Repository Structure

```
AI-Powered-Customer-Behaviour-Data-Analytics-Dashboard
│
├── Dataset
│   └── Customer Shopping Trends.xlsx
│
├── Python
│   └── Customer_Shopping_Behavior_Analysis.ipynb
│
├── SQL
│   └── customer_behavior_sql_queries.sql
│
├── Dashboard
│   └── customer_behavior_dashboard.pbix
│
├── Images
│   ├── dashboard.png
│   ├── workflow.png
│   ├── deliverables.png
│   └── problem_statement.png
│
├── Reports
│   └── Project_Report.pdf
│
└── README.md
```

---

# ▶️ How to Run

### Step 1

Clone the repository

```bash
git clone https://github.com/shivamtiwari432/AI-Powered-Customer-Behaviour-Data-Analytics-Dashboard.git
```

---

### Step 2

Open the Jupyter Notebook

```
Customer_Shopping_Behavior_Analysis.ipynb
```

Perform:

- Data Import
- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering

---

### Step 3

Load cleaned data into SQL

- MySQL
- PostgreSQL
- SQL Server

---

### Step 4

Execute

```
customer_behavior_sql_queries.sql
```

Answer business questions using SQL.

---

### Step 5

Open

```
customer_behavior_dashboard.pbix
```

Refresh data and explore the interactive dashboard.

---

### Step 6

Review:

- Project Report
- Dashboard
- Presentation Deck

---

# 💼 Skills Demonstrated

- Excel
- Power Query
- Python
- Pandas
- NumPy
- SQL
- Power BI
- DAX
- Data Cleaning
- Data Modelling
- EDA
- Business Intelligence
- Dashboard Design
- Data Visualization
- Business Analysis
- Git & GitHub

---

# 🙏 Acknowledgement

This project was inspired by the excellent end-to-end Data Analytics tutorial created by **Amlan Mohanty**. The workflow and business case were used as a learning reference while developing this portfolio project. The implementation, documentation, analysis, and dashboard have been customized for educational and portfolio purposes.

---

# ⭐ Support

If you found this project useful:

⭐ Star this repository

🍴 Fork the project

💼 Connect with me on LinkedIn

📢 Share it with others learning Data Analytics

---

## 👨‍💻 Author

**Shivam Tiwari**

📧 Email: tiwarishivam281999@gmail.com

🔗 GitHub: https://github.com/shivamtiwari432

🔗 LinkedIn:https://www.linkedin.com/in/shivam-tiwari-929b7a261/?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base%3Bc6bYryApRnSfc%2Bn0X6EfXA%3D%3D
