# Maven Mega Mart Transaction Analysis

## Overview
Analysis of 2M+ retail transactions for Maven Mega Mart, covering discount behavior, household and product 
performance, time-based sales trends, and demographic spending patterns.

## What I Did
- Optimized memory usage on a 2M+ row dataset using efficient dtype handling
- Engineered features including total discount, percentage discount (capped and normalized), and complaint count
- Analyzed household purchasing behavior, identifying highly skewed spending concentrated in a small number 
  of top households
- Investigated whether top-selling products carry higher discounts than average — found the opposite: top 
  products are discounted *less* than the norm
- Built time-series visualizations of monthly sales trends, including year-over-year comparisons and day-of-week 
  patterns
- Analyzed spending patterns by age, income, and household composition
- Joined transaction, product, and demographic data to study department-level spending by age group

## Key Results
- Identified a data-processing bug in an early discount-capping step that was silently zeroing out an entire 
  feature column — caught and fixed before it affected downstream analysis
- Found that the top 10 products by sales value carry a ~10% average discount, notably lower than the ~18% 
  store-wide average
- Uncovered a large outlier transaction (89,638 units) that turned out to be a legitimate gasoline purchase, 
  not a data error

## Tech Stack
Python, Pandas, NumPy, Matplotlib, Seaborn
