# Data Exploration and Logistic Analysis of Import-Export Dataset

### Project Overview
This project focuses on the **exploration** and **causal analysis** of an **import-export dataset** using Python. The dataset includes information about international trade transactions, categorized by variables such as **Country**, **Product**, **Shipping Method**, **Quantity**, **Value**, and **Weight**. The project applies **descriptive**, **inferential**, and **causal statistics** to uncover insights that can help improve trade strategies, logistics, and decision-making processes.

### Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Key Objectives](#key-objectives)
- [Tools & Libraries Used](#tools--libraries-used)
- [Project Structure](#project-structure)
- [Analysis Overview](#analysis-overview)
  - [Categorical Data Analysis](#categorical-data-analysis)
  - [Non-Categorical Data Analysis](#non-categorical-data-analysis)
  - [Causal Analysis](#causal-analysis)
- [Managerial Insights](#managerial-insights)
- [Instructions to Run](#instructions-to-run)
- [Contributors](#contributors)

---

### Dataset
The dataset contains the following variables:
- **Transaction_ID**: Unique identifier for each transaction.
- **Country**: The country involved in the transaction.
- **Product**: The type of product traded.
- **Import/Export**: Whether the transaction was an import or export.
- **Quantity**: The number of units traded in the transaction.
- **Value**: The total value of the transaction in monetary terms.
- **Weight**: The weight of the goods in kilograms.
- **Shipping Method**: The method used to transport the goods (Air, Sea, etc.).
- **Category**: A higher-level grouping of the product (e.g., Electronics, Clothing, Machinery).

The dataset is cross-sectional and was sourced from [Kaggle Imports-Exports Dataset](https://www.kaggle.com/datasets/chakilamvishwas/imports-exports-1).

---

### Key Objectives
1. **Explore and Analyze Data**: Identify key trends and relationships in trade transactions.
2. **Perform Inferential Statistics**: Uncover significant relationships between variables such as product categories and transaction value.
3. **Conduct Causal Analysis**: Model and predict outcomes such as the likelihood of a transaction being classified as an import or export using logistic regression.
4. **Provide Managerial Insights**: Deliver actionable recommendations to optimize logistics and trade strategies.

---

### Tools & Libraries Used
- **Pandas**: For data manipulation and exploration.
- **Numpy**: For numerical operations.
- **Matplotlib & Seaborn**: For data visualization.
- **Statsmodels**: For statistical analysis, including regression models.
- **Scipy**: For inferential tests such as t-tests, ANOVA, and Chi-squared tests.
- **Sklearn**: For encoding and regression models.
  
---

### Project Structure

```bash
├── data/
│   └── Imports_Exports_Dataset.csv   # Dataset used in the project
├── notebooks/
│   └── Project_1.ipynb               # Jupyter Notebook containing the code and analysis
├── reports/
│   └── README.md                     # This README file
└── insights/
    └── Managerial_Insights.pdf        # PDF with managerial insights and recommendations
```

---

### Analysis Overview

#### 1. Categorical Data Analysis
- **Descriptive Statistics**: Examined frequency distributions for variables like `Country`, `Product`, and `Shipping Method`. Identified the most common countries and products involved in trade.
- **Inferential Analysis**: Conducted Chi-squared tests to explore relationships between variables such as `Country` and `Shipping Method`, finding statistically significant relationships.
- **Causal Analysis**: Logistic regression was applied to predict whether a transaction is an import or export based on variables like `Country`, `Product`, and `Shipping Method`.

#### 2. Non-Categorical Data Analysis
- **Descriptive Statistics**: Summarized key numerical variables (`Quantity`, `Value`, `Weight`) using metrics such as mean, median, and standard deviation. 
- **Inferential Analysis**: Performed ANOVA tests to compare transaction values across product categories and identified significant differences.
- **Causal Analysis**: Linear and polynomial regression models were used to predict transaction `Value` based on `Quantity` and `Weight`.

#### 3. Causal Analysis
- **Logistic Regression**: Modeled the probability of a transaction being an import or export based on categorical and continuous variables such as `Country`, `Shipping Method`, `Quantity`, and `Weight`.

---

### Managerial Insights
Some key insights and recommendations derived from the analysis include:
- **Optimize Shipping Methods**: Air shipping should be prioritized for high-value goods like electronics, while sea shipping can be used for bulkier items.
- **Focus on High-Value Products**: Electronics and Machinery are driving the most significant trade activity and should be a focus for expansion.
- **Tailor Trade Strategies**: Specific countries have unique trade behaviors. For example, China and India are more likely to export, while the USA is more focused on imports.
- **Leverage Predictive Models**: Use logistic and linear regression models to predict future trends in trade and optimize decision-making.

---

### Instructions to Run
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/imports-exports-analysis.git
   ```
2. **Install Dependencies**:
   Make sure you have Python 3 installed. Then install the necessary packages using `pip`:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the Jupyter Notebook**:
   Open the `Project_1.ipynb` notebook in Jupyter:
   ```bash
   jupyter notebook notebooks/Project_1.ipynb
   ```

4. **Explore the Data**:
   Load and explore the dataset, following the steps in the Jupyter notebook.

---

### Contributors
- **Your Name** – Data Analyst and Project Lead

For questions or collaborations, feel free to reach out at [your.email@example.com](mailto:your.email@example.com).

---

This README file gives an overview of the project, helping others understand the purpose, structure, and steps required to run the analysis.
