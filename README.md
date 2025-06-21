# Market_Basket_Analysis
Online Retail Data Analysis and Market Basket Analysis
This notebook performs an exploratory data analysis and market basket analysis on the Online Retail II dataset. The dataset contains transactional data from a UK-based online retail store.

**Objectives:**

> Load and clean the online retail dataset.

> Perform exploratory data analysis (EDA) to understand key trends and patterns, including:

> Top selling products

> Top customers by purchase volume

> Monthly and hourly sales trends

> Sales by country

> Implement Sequential Pattern Mining (using PrefixSpan) to identify frequent sequences of purchases.

> Implement Frequent Itemset Mining (using Apriori and FP-Growth) to find product combinations that frequently appear together in transactions.

> Generate and analyze association rules from the frequent itemsets to identify product recommendations.

> Visualize the results, including association rules as network graphs and heatmaps of itemset support.

**Dataset**:

The dataset used is "Online Retail II" from Kaggle: https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci

**Notebook Structure**

The notebook is organized into the following sections:

**Kaggle Dataset Download in Colab:**
Steps to download the dataset directly in Google Colab.

**Data Cleaning:**
Handles missing values, removes invalid entries, and prepares the data for analysis.
Exploratory Data Analysis: Visualizes various aspects of the sales data, such as top products, customers, and temporal trends.
Temporal Analysis: Further explores monthly, weekly, hourly, and daily sales patterns using Plotly for interactive visualizations.
Sequential Pattern Mining: Uses the PrefixSpan algorithm to find frequent sequences of purchased items.
Create the Transaction Basket Format: Transforms the data into a format suitable for frequent itemset mining.
Frequent Itemset Mining (Apriori & FP-Growth): Applies Apriori and FP-Growth algorithms to identify frequent itemsets.
Association Rule Generation: Generates association rules (antecedent -> consequent) from the frequent itemsets.
Visualization of Association Rules: Visualizes the association rules as network graphs and Sankey diagrams.
Heatmaps of Itemsets: Visualizes the support of frequent itemsets using heatmaps.
Plotly Dashboard (Attempted): An attempt to create a combined Plotly dashboard (note: combining Sankey and other plot types in make_subplots can be complex, separate figures are shown).

**Export Results:** Exports the frequent itemsets, association rules, and key sales summaries to CSV files.

**Getting Started**
To run this notebook:

Open the notebook in Google Colab.
Follow the steps to download the dataset from Kaggle (requires a Kaggle account and API key).
Run all the cells sequentially.
Dependencies
The notebook uses the following libraries:

pandas

numpy

matplotlib

seaborn

plotly

mlxtend

prefixspan

networkx

These dependencies will be installed automatically when you run the !pip install commands in the notebook.

**Key Findings (Based on Notebook Output)**
The dataset contains transactional data with details on invoices, products, quantities, dates, prices, customer IDs, and countries.
Data cleaning involved handling missing Customer IDs and Descriptions, removing transactions with zero or negative quantities, and standardizing product descriptions.
EDA revealed insights into top-selling products, high-value customers, and temporal sales patterns (e.g., peak sales hours/months).
Sequential pattern mining identified frequent sequences of items purchased in the same invoice.
Frequent itemset mining and association rule generation identified product combinations that are likely to be bought together (e.g., "strawberry ceramic trinket box" and "sweetheart ceramic trinket box" have a high lift). These rules can be used for product recommendations and store layout optimization.
Visualizations like heatmaps help understand the co-occurrence of different products.

**Future Work:**

Further explore different minimum support and confidence thresholds for association rule mining.

Implement clustering techniques to group customers based on their purchase history.

Build a more comprehensive and interactive dashboard using Dash or other visualization libraries.

Perform time series forecasting on the monthly sales data.
