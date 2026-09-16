# Customer Shopping Behavior Analysis

## 📌 Overview

This project analyzes customer shopping behavior using **Python, SQL, PostgreSQL/MySQL/SQL Server, and Power BI**. The goal is to identify customer spending patterns, product preferences, customer segments, discount behavior, subscription trends, and revenue insights.

The project follows an end-to-end data analytics workflow:

**Dataset → Python EDA → Data Cleaning → SQL Analysis → Power BI Dashboard → Report → Presentation**

---

## 📊 Dataset

The dataset contains **3,900 customer purchase records and 18 columns** covering customer demographics, purchase information, product details, shopping behavior, ratings, discounts, subscriptions, and shipping information.

### Key Data Categories

* Customer demographics
* Product and category information
* Purchase amount
* Season and size
* Customer subscription status
* Discount and promotional activity
* Previous purchases
* Purchase frequency
* Review ratings
* Shipping type

The dataset contained **37 missing values in the Review Rating column**, which were handled during the data-cleaning process.

---

## 🛠️ Tools & Technologies

| Tool           | Purpose                                           |
| -------------- | ------------------------------------------------- |
| **Python**     | Data loading, cleaning, EDA & feature engineering |
| **Pandas**     | Data manipulation and analysis                    |
| **PostgreSQL** | Database storage and SQL analysis                 |
| **MySQL**      | SQL analysis                                      |
| **SQL Server** | SQL analysis                                      |
| **SQL**        | Business and customer analysis                    |
| **Power BI**   | Dashboard and data visualization                  |
| **Gamma**      | Project presentation                              |
| **GitHub**     | Project documentation and version control         |

---

## 🔄 Project Steps

### 1. Data Loading

The customer shopping dataset was loaded into Python using **Pandas** for initial analysis and preprocessing.

```python
import pandas as pd

df = pd.read_csv("customer_shopping_behavior.csv")

print(df.head())
print(df.info())
```

---

### 2. Exploratory Data Analysis

Initial EDA was performed to understand the structure and characteristics of the dataset.

Key activities included:

* Checking dataset shape
* Understanding column data types
* Generating descriptive statistics
* Identifying missing values
* Exploring customer and purchase patterns
* Checking data consistency

Python functions such as `info()` and `describe()` were used for initial exploration.

---

### 3. Data Cleaning & Feature Engineering

The dataset was cleaned and prepared for further analysis.

### Data Cleaning

* Checked for missing values
* Handled missing Review Rating values
* Standardized column names
* Checked data consistency
* Removed the redundant `promo_code_used` column

Missing review ratings were imputed using the **median rating of the respective product category**.

### Feature Engineering

Created additional features including:

* `age_group`
* `purchase_frequency_days`

These features helped improve customer segmentation and behavioral analysis.

---

### 4. SQL Analysis

The cleaned dataset was integrated with a relational database for SQL-based business analysis.

SQL queries were used to answer important business questions such as:

* Revenue by gender
* High-spending customers using discounts
* Top 5 products by average rating
* Standard vs. Express shipping spending
* Subscriber vs. non-subscriber revenue
* Products with high discount dependency
* Customer segmentation
* Top products by category
* Repeat buyers and subscription behavior
* Revenue contribution by age group

These queries can be implemented using **PostgreSQL, MySQL, or SQL Server** with appropriate syntax adjustments.

---

## 📈 Power BI Dashboard

An interactive **Power BI dashboard** was created to present the major findings from the analysis.

The dashboard focuses on:

* Customer behavior
* Revenue analysis
* Product performance
* Customer segmentation
* Subscription behavior
* Discount analysis
* Age-group revenue
* Shopping trends

The dashboard provides an interactive way to explore the results and communicate business insights.

---

## 📋 Project Report

A detailed project report was prepared covering:

1. Project Overview
2. Dataset Summary
3. Python EDA
4. Data Cleaning
5. Feature Engineering
6. SQL Business Analysis
7. Power BI Dashboard
8. Business Recommendations

---

## 🎤 Project Presentation

A project presentation was created using **Gamma** to summarize the workflow, analysis, dashboard, key findings, and business recommendations.

The presentation is designed to provide a concise overview of the complete data analytics project.

---

## 📌 Results & Business Insights

The analysis provided insights into:

* Customer spending behavior
* Revenue contribution across customer groups
* Product ratings and purchasing patterns
* Discount usage
* Subscription behavior
* Customer loyalty segments
* Shipping preferences
* Revenue contribution by age group

The analysis also supports business recommendations related to subscription promotion, loyalty programs, discount strategy, product positioning, and targeted marketing.

---

## ▶️ How to Run

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/customer-shopping-behavior-analysis.git
```

### Step 2: Navigate to the Project

```bash
cd customer-shopping-behavior-analysis
```

### Step 3: Install Required Python Libraries

```bash
pip install pandas numpy matplotlib seaborn
```

### Step 4: Run the Python Analysis

Open the Python notebook or script and execute the cells/scripts for:

* Data loading
* EDA
* Data cleaning
* Feature engineering

### Step 5: Database Analysis

Load the cleaned dataset into **PostgreSQL, MySQL, or SQL Server** and execute the SQL scripts available in the repository.

### Step 6: Power BI Dashboard

Open the Power BI `.pbix` file and refresh the data source if required.

### Step 7: Project Report & Presentation

Refer to the included **project report** and **Gamma presentation** for detailed findings and project explanation.

---

## 📁 Project Structure

```text
Customer-Shopping-Behavior-Analysis/
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── python/
│   └── customer_behavior_analysis.ipynb
│
├── sql/
│   ├── postgresql_queries.sql
│   ├── mysql_queries.sql
│   └── sql_server_queries.sql
│
├── powerbi/
│   └── customer_behavior_dashboard.pbix
│
├── report/
│   └── Customer_Shopping_Behavior_Analysis.pdf
│
├── presentation/
│   └── Customer_Shopping_Behavior_Analysis.pptx
│
└── README.md
```

---

## 🎯 Skills Demonstrated

**Python • Pandas • Data Cleaning • Exploratory Data Analysis • Feature Engineering • SQL • PostgreSQL • MySQL • SQL Server • Power BI • Data Visualization • Business Intelligence • Business Analysis**

---

## 👤 Project Type

**Data Analytics / Business Intelligence Project**

This project demonstrates an end-to-end approach to transforming raw customer transaction data into **clean data, SQL-based analysis, interactive dashboards, and actionable business insights**.
