# Task 2 – Data Analysis and Visualization

## 📌 Introduction

This project analyzes the **Sample Superstore dataset** using Python data analysis and visualization libraries.

The main focus is on understanding business data through charts and statistical analysis.

## 🎯 Aim

To perform exploratory data analysis on the Sample Superstore dataset and create meaningful visualizations for sales, profit, discount, and numerical relationships.

## 📚 Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

## 🔄 Data Preparation

The dataset is loaded using Pandas:

```python
df = pd.read_csv("samplesuperstore.csv")
```

The Order Date and Ship Date columns are converted to datetime format.

A new column called `Delivery Days` is calculated:

```python
df['Delivery Days'] = (df['Ship Date'] - df['Order Date']).dt.days
```

The dataset is also checked for missing values and unique categories.

## 📊 Visualizations

### Bar Plot

Bar plots are created to compare:

* Profit by Category
* Sales by Category

The purpose is to identify differences in sales and profit among categories.

### Box Plot

Box plots are used to analyze profit distribution and variation across categories.

They help identify:

* Median
* Data distribution
* Outliers
* Variation

### Scatter Plot

A scatter plot is created using:

```text
Discount → Profit
```

This visualization helps investigate whether discounts are associated with changes in profitability.

### Histogram

A histogram is used to visualize the distribution of Sales values.

### Correlation Heatmap

A correlation matrix is generated for numerical columns and visualized using a heatmap.

Correlation helps understand the relationship between numerical variables.

## 📁 Project Structure

```text
Task2/
│
├── task2.py
├── Task2.ipynb
├── samplesuperstore.csv
└── README.md
```

## ▶️ Execution

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn
```

Run the Python file:

```bash
python task2.py
```

Or open `Task2.ipynb` in Google Colab/Jupyter Notebook.

## 📌 Expected Output

The project generates:

* Sales by Category bar chart
* Sales distribution histogram
* Profit by Category bar chart
* Sales by Category visualization
* Profit distribution box plot
* Profit variation by Category box plot
* Discount vs Profit scatter plot
* Correlation heatmap

## ✅ Result

The project successfully demonstrates exploratory data analysis and visualization techniques using the Sample Superstore dataset.
