# Customer-Behavior-Analysis
This project focuses on analyzing customer purchasing patterns, engagement levels, and revenue behavior using a full data pipeline built with PostgreSQL, Python, and Power BI.
# Overview
This project analyzes customer shopping behavior using Python, SQL, and Power BI to uncover insights about spending patterns, product preferences, subscription behavior, and customer segments.
It follows a complete data analytics workflow — from data loading and cleaning to SQL-based analysis and dashboard creation.
A final PPT report was generated using Gamma.

# Dataset
Total Rows: 3,900 <br>
Columns: 18 <br>
Features include:<br>
Demographics: Age, Gender, Subscription Status <br>
Purchase details: Item Purchased, Category, Amount, Season, Size, Color<br>
Behavior: Discount Applied, Review Rating, Previous Purchases, Frequency, Shipping Type<br>
Missing values: 37 missing ratings handled during cleaning<br>
Raw Dataset : [![PDF](https://img.shields.io/badge/Open-File-red)](https://github.com/sammedah/Customer-Behavior-Analysis/blob/main/project.csv)

# Tools & Technologies
Python: Pandas, NumPy, Matplotlib/Seaborn <br>
SQL Databases: PostgreSQL server <br>
Power BI: Dashboard creation <br>
Jupyter Notebook / VS Code for coding and analysis <br>

## 4. Steps Followed

### Step 1 – Data Loading (Python)
Loaded dataset using Pandas<br>
Performed basic inspection using `.info()`, `.describe()`, `.isnull()`<br><br>

### Step 2 – Data Cleaning & Preparation
Filled missing review ratings using median per category<br>
Converted columns to snake_case<br>
Created new features:<br>
- age_group (young adult, adult, senior)<br>
- purchase_frequency_days<br>
Removed redundant columns such as `promo_code_used`<br><br>

### Step 3 – SQL Analysis (PostgreSQL / MySQL / SQL Server)
Loaded cleaned data into SQL and performed business analysis:<br>
- Revenue by gender<br>
- High-spending customers using discounts<br>
- Top-rated products<br>
- Shipping type comparison<br>
- Subscribers vs non-subscribers spend summary<br>
- Discount-dependent products<br>
- Customer segmentation (New / Returning / Loyal)<br>
- Top 3 products in each category<br>
- Revenue by age group (Young Adults contribute the most)<br><br>

### Step 4 – Dashboard (Power BI)
Designed an interactive dashboard including:<br>
- Total customers: 3.9K<br>
- Avg purchase amount: $59.76<br>
- Avg rating: 3.75<br>
- Subscription distribution (73% non-subscribers)<br>
- Revenue by category, age group, and segment (Page 7 dashboard)
- 📊 Customer Behavior Dashboard

## 5. Dashboard

Below is the Power BI dashboard built for analyzing customer behavior.

### 📊 Dashboard Overview
![Dashboard](https://github.com/sammedah/Customer-Behavior-Analysis/raw/main/Customer%20Analysis%20%20Dashboard.png)

### 🧾 Key Features

#### **KPIs**
- Total customer count  
- Average purchase amount  
- Average rating  

#### **Filters**
- Subscription status (Yes/No)  
- Gender  
- Category  
- Shipping Type  

#### **Visuals Included**
- Revenue by Category  
- Sales by Category  
- Revenue by Age Group  
- Sales by Age Group  
- Subscription Breakdown  


## 6. Results & Insights

### 🔍 Key Findings
- **Young Adults generate the highest revenue** among all age groups.  
- **Standard shipping is the most popular**, but Express shipping customers spend slightly more.  
- **Non-subscribers (73%) dominate**, but subscribers show stronger spending behavior.  
- **Clothing category leads** in both total revenue and sales volume.  
- Several product categories show **high dependence on discount usage**.
---
### 💼 Business Recommendations
*(Based on insights from the analysis)*

- **Promote subscription benefits** to increase subscriber count and long-term value.  
- **Implement loyalty programs** to retain repeat purchasers.  
- **Optimize discount strategy** to protect margins while still driving conversions.  
- **Highlight best-selling and top-rated products** in marketing campaigns.  
- **Target high-value age groups** such as Young Adults and Middle-aged consumers with personalized offers.

- Analysis Report : [![PDF](https://img.shields.io/badge/Open-File-red)](https://github.com/sammedah/Customer-Behavior-Analysis/blob/main/Customer%20Shopping%20Behavior%20Analysis.pdf)

- ## 7. How to Run the Project

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/customer-behavior-analysis.git


### 2️⃣ Install Dependencies
pip install -r requirements.txt


### 3️⃣ Run the Python Notebook
Open the Jupyter Notebook (.ipynb)
Load the dataset
Clean and preprocess the data
Perform EDA and feature creation
Export the cleaned dataset as a CSV file

### 4️⃣ Set Up the SQL Database
Create a new database in PostgreSQL / MySQL / SQL Server
Import the cleaned CSV into the database
Run business queries from the sql/ folder to generate insights

### 5️⃣ Open the Power BI Dashboard
Open the .pbix file in Power BI Desktop
Refresh the SQL database connection
Interact with the dashboard to explore insights







