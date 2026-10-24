# Credit Card Spending Analysis

Analysis of 50,000 credit card transactions (Jan to 14 Oct 2023) using Python (Pandas) and SQL.

## Tools
Python, Pandas, SQL (SQLite), Jupyter Notebook

## Dataset
Comprehensive Credit Card Transactions Dataset (Kaggle, author: rajatsurana979).
The dataset appears to be synthetic, so findings reflect patterns in this dataset only.

## What I did
- Cleaned data: fixed date formats, handled missing Gender (5,047 rows, labelled "Unknown"), standardised column names
- Created features: month, weekday, is_weekend, age, age_group, high_value flag (top 5% within each category)
- Wrote SQL queries for monthly trend, category share, age/gender analysis, weekend vs weekday and high-value transactions

## Key insights
- Travel contributes 58.36% of total spend; Electronics 19.88%; Restaurant only 2.10%
- Monthly spend stays stable (2.15M to 2.48M); October is partial (data till 14 Oct)
- Age group and gender show almost no difference in average ticket size (about 434 to 446)
- Weekdays have more transactions in raw count only because there are more weekdays; per-day volume is similar
- High-value flag is calculated per category, because a global top 5% would be entirely Travel

## Project structure
- `data/` cleaned dataset
- `notebooks/` Python analysis
- `main1.ipynb/` SQL queries

## Next steps
Power BI dashboard (in progress)