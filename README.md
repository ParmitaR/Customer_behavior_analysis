# Customer_behavior_analysis
# Customer Behavior Analysis Project

## 📌 Overview
This project analyzes customer purchasing behavior to uncover patterns in spending, subscription status, purchase frequency, and customer demographics. The workflow covers the full data analytics lifecycle — from raw data cleaning in Python, to SQL-based analysis, to an interactive Power BI dashboard, and finally a summarized report and presentation for stakeholders.

The goal is to help a business understand **who its customers are**, **how they spend**, and **what drives repeat purchases and subscriptions**.

## 📂 Dataset
- **Source:** [Add dataset source, e.g., Kaggle / company data / synthetic dataset]
- **Format:** CSV
- **Size:** ~3,900 customer records
- **Key columns:**
  - `Customer ID`
  - `Age`
  - `Gender`
  - `Purchase Amount (USD)`
  - `Location`, `Size`, `Color`, `Season`
  - `Review Rating`
  - `Subscription Status`
  - `Shipping Type`
  - `Discount Applied`, `Promo Code Used`
  - `Previous Purchases`
  - `Payment Method`
  - `Frequency of Purchases`

## 🛠️ Tools & Technologies
| Category | Tools |
|---|---|
| Programming | Python (Pandas, NumPy, Matplotlib/Seaborn) |
| Database | PostgreSQL / MySQL / SQL Server |
| Visualization | Power BI |
| Reporting | Microsoft Word / PDF |
| Presentation | Gamma (AI-powered slide generator) |
| Environment | Jupyter Notebook |

## 🔄 Project Steps

1. **Data Loading**
   - Imported the raw dataset into Python using Pandas.

2. **Exploratory Data Analysis (EDA)**
   - Reviewed data structure, types, and summary statistics.
   - Identified missing values, duplicates, and outliers.
   - Visualized distributions (age groups, purchase amounts, review ratings).

3. **Data Cleaning**
   - Handled missing/inconsistent values.
   - Standardized categorical fields (e.g., subscription status, payment method).
   - Created derived columns, such as:
     - `age_group` (Young Adult / Adult / Middle-Aged / Senior) using `pd.qcut`
     - `purchase_frequency_days` (mapped purchase frequency text to numeric days)

4. **SQL Analysis**
   - Loaded the cleaned dataset into PostgreSQL/MySQL/SQL Server.
   - Wrote queries to answer business questions, e.g.:
     - Average purchase amount by category/location
     - Customer segmentation by subscription status
     - Top spending customer segments

5. **Power BI Dashboard**
   - Connected Power BI to the cleaned dataset/SQL database.
   - Built DAX measures (e.g., `Average Purchase Amount`, `Average Review Rating`).
   - Designed an interactive dashboard with KPI cards, charts, and filters.

6. **Reporting**
   - Summarized key findings and business insights in a written report.

7. **Presentation**
   - Created a stakeholder-facing slide deck using Gamma to communicate insights visually.

## 📊 Dashboard
The Power BI dashboard ("Customer Behavior Dashboard") includes:
- **KPI Cards:** Number of Customers, Average Purchase Amount, Average Review Rating
- **Subscription Status Breakdown:** Donut chart showing % of subscribed vs. non-subscribed customers
- **[Add additional visuals, e.g., Purchase Amount by Category, Sales Trend by Season]**

*(Add a screenshot of the dashboard here once finalized)*

## 📈 Results & Key Insights
- Average purchase amount across customers: **$59.76**
- Average customer review rating: **3.75 / 5**
- **73%** of customers are not currently subscribed, while **27%** are subscribed — highlighting a potential opportunity for subscription growth.
- [Add 2–3 more key insights specific to your analysis, e.g., top-performing category, most common payment method, seasonal trends]

## ▶️ How to Run

### 1. Clone the repository
```bash
git clone https://github.com/your-username/customer-behavior-analysis.git
cd customer-behavior-analysis
```

### 2. Set up the Python environment
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Run the analysis notebook
```bash
jupyter notebook customer_behavior_analysis.ipynb
```

### 4. Load data into your SQL database
- Import the cleaned CSV into PostgreSQL/MySQL/SQL Server using your preferred client (e.g., pgAdmin, MySQL Workbench, SSMS).
- Run the queries provided in `/sql/queries.sql`.

### 5. Open the Power BI dashboard
- Open `customer_behavior.pbix` in Power BI Desktop.
- Refresh the data source connection if needed.

### 6. View the report and presentation
- Report: `/reports/customer_behavior_report.pdf`
- Slides: `/presentation/customer_behavior_slides.pdf` (created with Gamma)

## 📁 Project Structure
```
customer-behavior-analysis/
├── data/
│   └── customer_data.csv
├── notebooks/
│   └── customer_behavior_analysis.ipynb
├── sql/
│   └── queries.sql
├── dashboard/
│   └── customer_behavior.pbix
├── reports/
│   └── customer_behavior_report.pdf
├── presentation/
│   └── customer_behavior_slides.pdf
└── README.md
```
Data analytics project showcasing customer behavior analysis using python, sql, and power Bi.
