# 📊 Data Analytics Project

## 📌 Overview

This project demonstrates an end-to-end **Data Analytics workflow**, starting from raw dataset loading and data cleaning to Exploratory Data Analysis (EDA), SQL analysis, interactive dashboard creation, and final business reporting.

The project uses **Python, PostgreSQL, MySQL, SQL Server, and Power BI** to analyze the dataset and extract meaningful insights. A presentation was also created using **Gamma** to communicate the findings in a clear and professional format.

---

## 🎯 Project Objectives

* Load and understand the raw dataset.
* Perform data cleaning and preprocessing.
* Conduct Exploratory Data Analysis (EDA) using Python.
* Analyze the data using SQL queries.
* Work with multiple SQL databases:

  * PostgreSQL
  * MySQL
  * SQL Server
* Identify important trends and patterns.
* Create an interactive Power BI dashboard.
* Generate a structured analytical report.
* Present the key findings using a professional PPT created with Gamma.

---

## 📂 Dataset

The project uses a customer shopping behavior dataset containing information related to customer purchases and shopping patterns.

Typical attributes include:

* Customer information
* Age
* Gender
* Category
* Item purchased
* Purchase amount
* Location
* Season
* Review rating
* Discount information
* Subscription status
* Shipping type
* Purchase frequency

The dataset is initially loaded into Python for inspection, cleaning, and analysis.

---

## 🛠️ Tools & Technologies

| Tool / Technology    | Purpose                             |
| -------------------- | ----------------------------------- |
| **Python**           | Data loading, cleaning and EDA      |
| **Pandas**           | Data manipulation and analysis      |
| **NumPy**            | Numerical operations                |
| **Matplotlib**       | Data visualization                  |
| **Seaborn**          | Statistical visualization           |
| **PostgreSQL**       | SQL-based data analysis             |
| **MySQL**            | SQL queries and analysis            |
| **SQL Server**       | SQL queries and analysis            |
| **Power BI**         | Interactive dashboard               |
| **Gamma**            | Presentation/PPT creation           |
| **Jupyter Notebook** | Python-based analysis               |
| **Git & GitHub**     | Version control and project hosting |

---

# 🔄 Project Workflow

```text
Raw Dataset
     ↓
Data Loading
     ↓
Data Understanding
     ↓
Data Cleaning
     ↓
Exploratory Data Analysis (EDA)
     ↓
SQL Analysis
 ┌───┼───────────────┐
 ↓   ↓               ↓
PostgreSQL  MySQL  SQL Server
 └───┼───────────────┘
     ↓
Business Insights
     ↓
Power BI Dashboard
     ↓
Analytical Report
     ↓
Gamma Presentation
```

---

# 🐍 1. Data Loading & Python Analysis

The dataset is loaded into Python using **Pandas**.

```python
import pandas as pd

df = pd.read_csv("customer_shopping_behavior.csv")

df.head()
```

Initial analysis is performed to understand:

* Number of rows and columns
* Data types
* Missing values
* Duplicate records
* Statistical summary
* Unique values
* Data distributions

---

# 🧹 2. Data Cleaning

The raw dataset is cleaned before performing analysis.

Major cleaning activities include:

* Handling missing values
* Removing duplicate records
* Correcting data types
* Standardizing column names
* Handling inconsistent values
* Checking outliers
* Creating derived columns where required

Example:

```python
df.info()
df.isnull().sum()
df.duplicated().sum()
df.describe()
```

The cleaned dataset is then used for further analysis.

---

# 📈 3. Exploratory Data Analysis (EDA)

EDA is performed using Python to identify patterns, trends, and relationships within the data.

Key analysis areas include:

* Customer demographics
* Purchase behavior
* Product categories
* Sales distribution
* Customer segmentation
* Subscription behavior
* Discounts
* Ratings
* Seasonal purchasing patterns

Visualizations are created using:

```python
import matplotlib.pyplot as plt
import seaborn as sns
```

---

# 🗄️ 4. SQL Analysis

After cleaning and preparing the dataset, it is loaded into relational databases for SQL analysis.

### Databases Used

* PostgreSQL
* MySQL
* SQL Server

SQL queries are used to answer business-oriented questions such as:

* What are the highest-performing product categories?
* Which products generate the highest sales?
* What is the average purchase amount?
* Which customer segments contribute the most revenue?
* How does customer behavior vary by location?
* What is the relationship between discounts and purchases?
* How does subscription status affect purchasing behavior?

Example SQL:

```sql
SELECT 
    category,
    SUM(purchase_amount) AS total_sales
FROM customer_shopping
GROUP BY category
ORDER BY total_sales DESC;
```

---

# 📊 5. Power BI Dashboard

The cleaned and analyzed data is used to create an interactive **Power BI dashboard**.

The dashboard provides a visual summary of important business metrics and customer behavior.

### Dashboard Components

* Total Sales
* Total Customers
* Average Purchase Amount
* Average Rating
* Category-wise Sales
* Customer Demographics
* Purchase Trends
* Subscription Analysis
* Location-based Analysis
* Interactive filters and slicers

The dashboard allows users to explore the data interactively and identify important patterns.

---

# 📋 6. Analytical Report

A detailed report is created to document the complete analysis.

The report includes:

1. Project Introduction
2. Business Problem
3. Dataset Description
4. Data Cleaning
5. Exploratory Data Analysis
6. SQL Analysis
7. Power BI Dashboard
8. Key Findings
9. Business Insights
10. Conclusion

---

# 🎤 7. Presentation using Gamma

A professional presentation is created using **Gamma** to communicate the project findings.

The presentation covers:

* Project Overview
* Business Problem
* Dataset
* Methodology
* Python Analysis
* SQL Analysis
* Power BI Dashboard
* Key Insights
* Business Recommendations
* Conclusion

---

# 📌 Key Results

The analysis provides insights into:

* Customer purchasing patterns
* Product/category performance
* Revenue contribution
* Customer demographics
* Subscription behavior
* Discount utilization
* Customer ratings
* Seasonal trends
* Location-based purchasing behavior

These insights can help businesses better understand customers and support **data-driven decision-making**.

---

# 🚀 How to Run the Project

## 1. Clone the Repository

```bash
git clone <your-github-repository-url>
```

```bash
cd <project-folder>
```

## 2. Install Python Dependencies

```bash
pip install pandas numpy matplotlib seaborn
```

## 3. Open Jupyter Notebook

```bash
jupyter notebook
```

Open the project notebook and execute the cells sequentially.

## 4. Dataset

Place the dataset in the appropriate project directory.

Example:

```text
project/
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── notebooks/
│   └── data_analysis.ipynb
│
├── sql/
│   ├── postgresql_queries.sql
│   ├── mysql_queries.sql
│   └── sql_server_queries.sql
│
├── powerbi/
│   └── customer_analysis.pbix
│
├── report/
│   └── data_analysis_report.pdf
│
├── presentation/
│   └── project_presentation.pdf
│
└── README.md
```

## 5. SQL Setup

Import the cleaned dataset into your preferred database:

* PostgreSQL
* MySQL
* SQL Server

Execute the SQL scripts provided in the `sql` folder.

## 6. Power BI

Open the `.pbix` file using **Microsoft Power BI Desktop**.

If required, update the data source connection and refresh the dataset.

---

# 📁 Project Structure

```text
Data-Analytics-Project/
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── notebooks/
│   └── data_analysis.ipynb
│
├── sql/
│   ├── postgresql_queries.sql
│   ├── mysql_queries.sql
│   └── sql_server_queries.sql
│
├── powerbi/
│   └── dashboard.pbix
│
├── report/
│   └── analysis_report.pdf
│
├── presentation/
│   └── project_presentation.pdf
│
└── README.md
```

---

# 💡 Skills Demonstrated

This project demonstrates practical experience in:

* Data Cleaning
* Data Preprocessing
* Exploratory Data Analysis
* Python for Data Analytics
* Pandas & NumPy
* Data Visualization
* SQL
* PostgreSQL
* MySQL
* SQL Server
* Power BI
* Dashboard Development
* Business Intelligence
* Data Storytelling
* Report Writing
* Presentation Development

---

# 🏁 Conclusion

This project demonstrates a complete **end-to-end data analytics pipeline**, from raw data preparation and exploratory analysis to SQL-based analysis, interactive Power BI visualization, and business reporting.

It showcases the ability to transform raw data into meaningful insights using multiple industry-relevant analytics tools and communicate those insights effectively to stakeholders.

---

##

---

⭐ If you find this project useful, consider giving the repository a star.
