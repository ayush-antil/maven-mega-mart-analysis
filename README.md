# Maven Mega Mart: Transaction & Customer Analysis

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1QssuOdz0qw9P2x7bWPvk4ThOI-BFFTrm)

## Project Overview

This project analyzes over **2.1 million retail transaction records** from Maven Mega Mart to understand purchasing behavior, sales performance, discount patterns, product performance, and customer spending trends.

The analysis combines transaction, product, and demographic data to identify meaningful patterns and generate business-oriented insights.

---

## Business Problem

The objective is to understand how customers and products contribute to overall sales and how factors such as discounts, time, household characteristics, and demographics influence purchasing behavior.

The project focuses on transforming large-scale retail transaction data into actionable business insights.

---

## Key Questions

This analysis focuses on questions such as:

- What are the overall sales, quantity, and discount patterns?
- Which households contribute the most to total spending?
- Which products are the top performers?
- Are top-selling products discounted more heavily than average?
- How do sales patterns change over time?
- Which days generate the highest sales?
- Which demographic segments contribute the most revenue?
- How does household composition relate to spending?
- Which product departments are preferred by different age groups?

---

## Dataset

The project uses three datasets:

- `project_transactions.csv` — retail transaction-level data
- `product.csv` — product and department information
- `hh_demographic.csv` — household demographic information

The transaction dataset contains over **2 million transaction records** covering household, product, sales, quantity, store, and discount information.

The datasets are downloaded automatically when the notebook is executed in Google Colab.

---

## Analysis Performed

### Data Loading & Quality Check

- Loaded over 2 million transaction records
- Used optimized data types to reduce memory usage
- Checked dataset structure and data quality
- Examined missing values

### Feature Engineering

Created analytical features including:

- `total_discount`
- `percentage_discount`

### Sales & Transaction Analysis

Analyzed:

- Total sales
- Total units sold
- Total discounts
- Average basket value
- Average household spending
- Purchasing patterns

### Household Analysis

Analyzed customer purchasing behavior at the household level to identify:

- Highest-spending households
- Highest-volume households
- Frequent purchasing patterns
- Household contribution to overall sales

### Product Analysis

Analyzed product-level performance to identify:

- Top-selling products
- Product sales contribution
- Product quantity performance
- Discount behavior among top-selling products

### Time-Based Analysis

Analyzed sales trends across:

- Months
- Years
- Days of the week

### Demographic Analysis

Analyzed spending patterns across:

- Age groups
- Income groups
- Household composition

### Product & Demographic Analysis

Combined transaction, demographic, and product department data to understand how different customer segments distribute their spending across product categories.

---

## Key Findings

### Overall Performance

- **Total Sales:** $6,666,243.50
- **Total Units Sold:** 216,713,611
- **Average Basket Value:** $28.62
- **Average Household Spend:** $3,175.91
- **Overall Discount Rate:** approximately 17.68%

### Discounting

Top-selling products had a lower discount rate of approximately **10.33%**, compared with the overall store discount rate of approximately **17.68%**.

This indicates that strong-selling products did not require the same level of discounting to generate sales.

### Household Behavior

Spending is concentrated among a relatively small number of households, with certain households contributing significantly to overall quantity and revenue.

### Time Trends

Monthly sales increased substantially over the analyzed period and remained strong through the later periods of the dataset.

**Monday and Tuesday** were identified as the highest-selling days, indicating stronger early-week purchasing activity.

### Demographics

The **45–54 age group** and **$50K–$74K income segment** emerged as important revenue-driving customer groups.

The **19–24 age group** showed a strong concentration of spending in the **Grocery** department, suggesting an opportunity for cross-category growth.

---

## Business Recommendations

1. Focus customer retention and loyalty initiatives on the **45–54 middle-income segment**.

2. Schedule key promotions and marketing campaigns around **Monday and Tuesday**, when purchasing activity is strongest.

3. Avoid unnecessary heavy discounting on top-selling products because they already demonstrate strong sales performance with lower discounts.

4. Investigate the **19–24 customer segment** as a growth opportunity through cross-selling strategies beyond Grocery.

5. Monitor high-value households and develop targeted loyalty strategies to retain customers who contribute significantly to revenue.

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Exploratory Data Analysis
- Feature Engineering
- Data Visualization
- Customer Segmentation
- Time-Series Analysis

---

## Project Workflow

Data Loading
     ↓
Data Quality Check
     ↓
Feature Engineering
     ↓
Overall Sales Analysis
     ↓
Household Analysis
     ↓
Product Analysis
     ↓
Time-Based Analysis
     ↓
Demographic Analysis
     ↓
Product × Demographic Analysis
     ↓
Business Insights & Recommendations


## Run the Project

1. Open the notebook using the **Open in Colab** button above.
2. Run the notebook cells from top to bottom.
3. The required SQLite database is downloaded automatically during notebook execution.
4. No manual dataset upload is required.
