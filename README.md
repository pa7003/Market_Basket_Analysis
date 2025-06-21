# 🧺 Market Basket Analysis with Association Rules

[![View Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://github.com/pa7003/Market_Basket_Analysis/blob/main/Market_Basket_Analysis.ipynb)

This project explores consumer purchase behavior through **Market Basket Analysis (MBA)** using association rule mining techniques. By applying algorithms like **Apriori**, we uncover meaningful item combinations and insights that can drive product bundling, store layout optimization, and personalized marketing strategies.

---

## 📁 Repository Contents

- `Market_Basket_Analysis.ipynb`: The complete Jupyter Notebook with data processing, analysis, visualizations, and insights.
- 💡 Embedded visualizations: Association networks, item frequency charts, Sankey diagrams, and more.
- 📂 Data Source: Sample retail transaction dataset (imported from Kaggle or simulated basket data).

---

## 📌 Key Features

### 🧹 1. Data Preprocessing & Transformation
- Handling missing values and duplicates
- Transactional format → Basket format transformation
- Country-wise filtering (if applicable)

### 📊 2. Exploratory Data Analysis
- Most frequently bought items
- Basket size distribution
- Temporal sales trends (if available)

### 🔍 3. Frequent Itemset Mining
- **Apriori algorithm** to extract itemsets with high support
- Parameters tuning: Support, Confidence, Lift

### 🔗 4. Association Rule Mining
- Generation of rules based on:
  - Support
  - Confidence
  - Lift
  - Leverage
- Visualization of association rules using:
  - Network graphs
  - Heatmaps
  - Parallel coordinates
  - Sankey diagrams

### 📈 5. Advanced Analysis (Extended in future work)
- **Temporal Market Basket Analysis**
- **Sequential Rule Mining (PrefixSpan / SPADE)**
- **Personalization with Lift & Confidence**
- **Product Recommendation Engine (Rule-based)**

---

## 📦 Tech Stack

- **Language**: Python 3.11+
- **Libraries**:
  - `mlxtend` – Frequent Itemset & Rule Mining
  - `pandas`, `numpy` – Data processing
  - `matplotlib`, `seaborn`, `plotly` – Visualization
  - `networkx`, `pyvis` – Rule network visualization
- **Platform**: Jupyter Notebook

---

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/pa7003/Market_Basket_Analysis.git
   cd Market_Basket_Analysis
2. Open the notebook:

   Use Jupyter Notebook locally, or

   Open directly in Google Colab

3. Run all cells in Market_Basket_Analysis.ipynb
