## 📊 **Walmart Sales Data Analysis – SQL Project**

---

### 🧾 **Introduction**

This project focuses on analyzing Walmart’s sales data to identify the most successful branches and product lines, understand sales patterns, and gain deeper insights into customer behavior. The ultimate objective is to extract actionable intelligence that can drive smarter sales strategies and business decisions.

---

### 🎯 **Purpose of the Project**

The goal of this project is to derive meaningful insights from Walmart's retail data by investigating key variables that influence sales performance across different store locations. The insights gained will assist in evaluating and improving current business operations.

---

### 📦 **About the Dataset**

The data used in this project is sourced from the **Walmart Sales Forecasting on Kaggle**. It consists of transactional sales data.

The dataset includes **1,000 rows** and **17 columns**, with information ranging from purchase details to customer demographics and sales metrics.

---

### 📋 **Data Dictionary**

| **Column**         | **Description**                            | **Data Type**    |
| ------------------ | ------------------------------------------ | ---------------- |
| `invoice_id`       | Unique identifier for each sale            | `VARCHAR(30)`    |
| `branch`           | Branch code (A, B, or C)                   | `VARCHAR(5)`     |
| `city`             | City where the branch is located           | `VARCHAR(30)`    |
| `customer_type`    | Type of customer (Member or Normal)        | `VARCHAR(30)`    |
| `gender`           | Gender of the customer                     | `VARCHAR(10)`    |
| `product_line`     | Category of the purchased product          | `VARCHAR(100)`   |
| `unit_price`       | Price per unit of the product              | `DECIMAL(10, 2)` |
| `quantity`         | Number of units sold                       | `INT`            |
| `VAT`              | Value Added Tax applied                    | `FLOAT(6, 4)`    |
| `total`            | Total amount of the transaction            | `DECIMAL(12, 4)` |
| `date`             | Date of the transaction                    | `DATETIME`       |
| `time`             | Time of the transaction                    | `TIME`           |
| `payment`          | Payment method used                        | `VARCHAR(20)`    |
| `cogs`             | Cost of goods sold                         | `DECIMAL(10, 2)` |
| `gross_margin_pct` | Gross margin percentage                    | `FLOAT(11, 9)`   |
| `gross_income`     | Gross income from the transaction          | `DECIMAL(12, 4)` |
| `rating`           | Customer satisfaction rating (1.0 to 10.0) | `FLOAT(2, 1)`    |

------------------------------------
### 🔍 **Analysis Overview**

#### ✅ **Product Analysis**

* Analyze sales data across different product lines.
* Identify top-performing product lines based on revenue and volume.
* Highlight underperforming product lines for potential improvement.

#### ✅ **Sales Analysis**

* Examine sales trends over time (daily, weekly, monthly).
* Assess the effectiveness of current sales strategies.
* Recommend modifications to boost overall sales performance.

#### ✅ **Customer Analysis**

* Segment customers based on behavior and demographics.
* Identify purchasing patterns across different segments.
* Evaluate the profitability and value of each customer group.

---

### 🛠️ **Approach Used**

#### 1️⃣ **Data Wrangling**

* Checked for missing or NULL values in the dataset.
* Ensured data quality by applying `NOT NULL` constraints during table creation, effectively eliminating NULLs.

#### 2️⃣ **Feature Engineering**

* Created new columns to enrich the dataset and enhance analysis:

  * `time_of_day`: Categorized as Morning, Afternoon, or Evening to track peak sales times.
  * `day_name`: Extracted the weekday name (Mon–Sun) to analyze branch activity by day.
  * `month_name`: Extracted the transaction month (Jan–Dec) to find seasonal sales trends.

#### 3️⃣ **Exploratory Data Analysis (EDA)**

* Performed EDA to address core business questions and uncover actionable insights.

---

### ❓ **Business Questions Addressed**

#### 🏙️ **Generic Questions**

* How many unique cities are represented in the dataset?
* Which city is each branch located in?

---

#### 📦 **Product Analysis**

* How many unique product lines are there?
* What is the most frequently used payment method?
* Which product line has the highest number of sales?
* What is the total monthly revenue?
* Which month recorded the highest Cost of Goods Sold (COGS)?
* Which product line generated the most revenue?
* Which city achieved the highest overall revenue?
* Which product line paid the most in VAT?
* Categorize product lines as 'Good' or 'Bad' based on whether their sales exceed the average.
* Which branch sold more products than the average sales per branch?
* What is the most purchased product line by gender?
* What is the average customer rating for each product line?

---

#### 💰 **Sales Analysis**

* How many sales were made during each part of the day across weekdays?
* Which customer type brings in the most revenue?
* Which city has the highest VAT percentage?
* Which customer type pays the most VAT?

---

#### 👥 **Customer Analysis**

* How many unique customer types are in the dataset?
* How many distinct payment methods are used?
* What is the most frequent customer type?
* Which customer type purchases the most products?
* What is the most common gender among customers?
* How is gender distributed across different branches?
* At what time of day are most customer ratings given?
* During which time of day do customers leave the most ratings per branch?
* Which day of the week receives the highest average ratings overall?
* What is the best-rated day of the week for each branch?
