
# 📊 Customer Churn Analysis & Customer Intelligence

### By Shruti Vishnoi

**Python | Pandas | NumPy | SQL | SQLite | Matplotlib | Seaborn**

## 📌 Project Overview

Customer Churn Analysis & Customer Intelligence is a data analytics project focused on understanding customer churn, customer behavior, subscription plans, and support-related issues.

The project uses Python, SQL, and SQLite to clean customer data, combine multiple database tables, engineer meaningful features, and generate business insights that can support customer retention strategies.

## 🎯 Business Problem

Businesses may lose customers because of subscription issues, poor customer experience, complaints, or support-related problems.

The key business questions addressed in this project are:

- What percentage of customers have churned?
- What is the customer retention rate?
- Which subscription plan has a higher churn rate?
- How much monthly revenue is associated with churned customers?
- How are customer complaints and escalations related to churn?
- How can customer data be used to identify potential churn risks?

## 📂 Dataset Information

The project uses a customer churn database containing three main tables:

| Table | Purpose |
|---|---|
| `db_customer` | Customer demographic information |
| `db_subscription` | Subscription and cancellation details |
| `db_support` | Customer support and complaint information |

### Dataset Summary

- Customer records analyzed: 21
- Customer table records: 21
- Subscription table records: 21
- Support table records: 9
- Final analysis: Merged customer, subscription, and support information
- Churn flag: Created using cancellation date

> Note: This project uses a small dataset for learning and portfolio development. Results should not be generalized to a larger customer population.

## 🛠️ Tools & Technologies

- **Python:** Data cleaning, feature engineering, and analysis
- **Pandas:** Data manipulation and exploratory analysis
- **NumPy:** Feature creation and numerical operations
- **SQL:** Data querying and aggregation
- **SQLite:** Database management
- **Matplotlib:** Data visualization
- **Seaborn:** Statistical visualization
- **Google Colab:** Development environment

## 🔄 Project Workflow

1. Connect to the SQLite database
2. Identify available tables and columns
3. Load database tables into Pandas DataFrames
4. Check missing values and data types
5. Clean and standardize customer data
6. Convert date columns into appropriate formats
7. Create a `churn_flag` using cancellation dates
8. Calculate customer complaint counts
9. Merge customer, subscription, and support tables
10. Handle missing values
11. Create churn-related features
12. Perform exploratory data analysis
13. Calculate business metrics
14. Export the cleaned dataset as a CSV file

## 🧹 Data Cleaning & Preparation

The following data cleaning and transformation tasks were performed:

- Renamed the `name` column to `customer_name`
- Removed unnecessary columns such as `interests` and `pincode`
- Converted date columns into datetime format
- Standardized gender values such as `Men` and `Women`
- Filled missing country values using state-country mapping where possible
- Created a `churn_flag` based on customer cancellation dates
- Converted customer support information into complaint counts
- Removed unnecessary support columns
- Handled missing values in escalation, CSAT, and complaint fields
- Merged data using the common `customerid`

## 📈 Key Performance Results

| Metric | Result |
|---|---:|
| Churn Rate | 28.57% |
| Retention Rate | 71.43% |
| Average Revenue Per User (ARPU) | 18.85 |
| Average Customer Tenure | 1541.57 days |
| Revenue at Risk | 73.94 |
| Escalation Rate | 19.05% |
| Average Complaints per User | 0.43 |
| Escalation–Churn Correlation | 0.77 |

> Correlation indicates a relationship in this analyzed dataset. It does not prove that escalations directly cause customer churn.

## 📊 Churn Analysis by Subscription Plan

| Subscription Plan | Churn Rate |
|---|---:|
| Basic | 60.00% |
| Standard | 22.22% |
| Premium | 14.29% |

The Basic plan showed the highest churn percentage among the analyzed plans.

This result can help businesses investigate plan-specific customer experience, pricing, benefits, and support issues.

## 💡 Key Business Insights

- Approximately **28.57% of analyzed customers churned**.
- The retention rate was approximately **71.43%**.
- The Basic subscription plan had the highest observed churn rate.
- Churned customers represented approximately **73.94 in monthly revenue at risk**.
- Escalation and churn showed a positive correlation of **0.77** in the analyzed dataset.
- Complaint counts and support information can be used to identify customers who may require additional attention.
- Customer-level data can help businesses develop targeted retention strategies.

## 🧠 Problem-Solving Approach

### Problem 1: Missing and Inconsistent Data

**Solution:**
- Checked missing values in all database tables.
- Converted columns into appropriate data types.
- Standardized inconsistent gender values.
- Filled selected missing values using available information.

### Problem 2: Identifying Customer Churn

**Solution:**
- Created a `churn_flag` feature.
- Customers with a cancellation date were classified as churned.
- Customers without a cancellation date were classified as retained.

### Problem 3: Combining Data from Multiple Tables

**Solution:**
- Used `customerid` as the common key.
- Merged customer, subscription, and support tables.
- Preserved customer-level information for analysis.

### Problem 4: Measuring Customer Support Activity

**Solution:**
- Calculated complaint counts for each customer.
- Retained the latest support record per customer.
- Used escalation and complaint-related fields for churn analysis.

### Problem 5: Converting Analysis into Business Insights

**Solution:**
- Calculated churn and retention rates.
- Compared churn across subscription plans.
- Calculated revenue at risk and ARPU.
- Analyzed the relationship between escalation and churn.

## 📌 Project Outcome

This project helped me develop practical experience in:

- Data cleaning and preprocessing
- SQL and SQLite database handling
- Data merging and feature engineering
- Exploratory data analysis
- Customer churn metrics
- Business problem-solving
- Data visualization
- Generating actionable business insights

The analysis demonstrates how raw customer, subscription, and support data can be transformed into structured information for customer retention analysis.

## 🚀 Future Improvements

- Analyze a larger customer dataset
- Build a customer churn prediction model
- Create an interactive Power BI dashboard
- Perform detailed customer segmentation
- Analyze churn trends over time
- Develop a more advanced churn risk scoring system
- Compare churn across regions and customer segments

## 📁 Project Files

- `Untitled6.ipynb` – Google Colab project notebook
- `README.md` – Project documentation

## 👩‍💻 Author

**Shruti Vishnoi**

Aspiring Data Analyst

Skills: Python | SQL | Excel | Power BI | Data Cleaning | Data Analysis

GitHub: [shrurtivishnoi-png](https://github.com/shrurtivishnoi-png)
