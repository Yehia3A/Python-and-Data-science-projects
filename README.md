# My Python and Data Science projects
# Online Retail Data Analysis

## Overview
Analyzes the Online Retail dataset using MongoDB and Cassandra for data storage, querying, and visualization. Preprocesses transactional data, performs aggregations (e.g., top products, revenue by country), and creates bar plots with Python.

**Tech Stack**: Python (pandas, matplotlib), MongoDB (pymongo), Cassandra (cassandra-driver)

## Dataset
- **Source**: [UCI Online Retail](https://archive.ics.uci.edu/ml/datasets/online+retail)
- **Details**: ~541,000 transactions (InvoiceNo, Quantity, UnitPrice, Country, etc.)

## Key Features
- **Preprocessing**: Cleans missing values, negative quantities/prices.
- **MongoDB**: Stores data, adds `TotalCost`/`DayTime`, queries top products, revenue, etc.
- **Cassandra**: Stores 3,000 rows, adds `total_cost`/`time_of_day`, runs similar queries.
- **Visualizations**: Bar plots of quantity purchased per country.

## Setup
1. Clone: `git clone https://github.com/your-username/your-repo-name.git`
2. Install: `pip install pymongo cassandra-driver pandas numpy matplotlib seaborn`
3. Add `Online Retail.csv` to `projects/online-retail/`.
4. Update MongoDB connection string and Cassandra bundle/credentials in `Online_Retail_Analysis.ipynb`.
5. Run: `jupyter notebook projects/online-retail/Online_Retail_Analysis.ipynb`

## Results
- **Top Products**: Stock codes `85123A`, `22423` lead sales.
- **Revenue**: UK dominates, followed by Netherlands.
- **Purchase Time**: Afternoon is most common.

## Notes
- Cassandra uses 3,000 rows for demo.
- See `Online_Retail_Analysis.ipynb` for details.
