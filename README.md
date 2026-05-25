# 📊 Exploratory Data Analysis (EDA) using Python

This project demonstrates Exploratory Data Analysis (EDA) using Python and Pandas. The main objective is to analyze a dataset, understand patterns and trends, calculate descriptive statistics, and identify outliers for better decision-making.

EDA is an important step in Data Analytics and Machine Learning because it helps understand the structure and quality of data before model building.

---

# 📌 Project Goal

Analyze a dataset to:
- Understand data patterns and distributions
- Calculate descriptive statistics
- Identify trends and outliers
- Generate meaningful insights

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- OpenPyXL

---

# 📂 Dataset Overview

The dataset contains structured sales/order-related information such as:
- Products
- Prices
- Quantities
- Order Status
- Customer details
- Total sales values

---

# ✅ Key Tasks Performed

## 1️⃣ Display Dataset Information

- Display first 5 rows
- View dataset shape
- Display column names
- Check dataset information

```python id="y2b6ko"
print(df.head())
print(df.shape)
print(df.columns)
print(df.info())
```

---

## 2️⃣ Check Missing Values

Identify null or missing values in the dataset.

```python id="5rzqgb"
df.isnull().sum()
```

---

## 3️⃣ Descriptive Statistics

Calculate:
- Count
- Mean
- Standard Deviation
- Minimum & Maximum values
- Percentiles

```python id="r8x2vh"
df.describe()
```

---

## 4️⃣ Calculate Mean & Median

Analyze average and central values of numeric columns.

```python id="x9k4na"
numeric_columns.mean()
numeric_columns.median()
```

---

## 5️⃣ Identify Top Products

Find products generating the highest revenue.

```python id="k8r0qm"
df.groupby('Product')['TotalPrice'].sum()
```

---

## 6️⃣ Analyze Order Status

Count frequency of different order statuses.

```python id="c3t1op"
df['OrderStatus'].value_counts()
```

---

## 7️⃣ Detect Outliers using IQR

Identify abnormal or extreme values using the Interquartile Range (IQR) method.

```python id="u9f2wr"
Q1 = df['TotalPrice'].quantile(0.25)
Q3 = df['TotalPrice'].quantile(0.75)
```

---

## 8️⃣ Generate Insights

Summarize important observations and trends from the dataset.

---

# ▶️ How to Run the Project

## Install Required Libraries

```bash id="t5v9ax"
pip install pandas numpy openpyxl
```

## Run the Program

```bash id="h8z1ck"
python filename.py
```

---

# 📊 Skills Demonstrated

- Exploratory Data Analysis
- Descriptive Statistics
- Data Interpretation
- Trend Analysis
- Outlier Detection
- Python Programming
- Pandas Data Analysis

---

# 🎯 Learning Outcomes

By completing this project, you will learn:

- How to analyze datasets effectively
- How to calculate statistical measures
- How to identify trends and anomalies
- How to generate business insights from data

---

# 🚀 Future Improvements

- Add visualizations using Matplotlib and Seaborn
- Create interactive dashboards
- Perform predictive analytics
- Build machine learning models

---

# 👨‍💻 Author

Developed as a beginner-friendly Data Analytics project for practicing Exploratory Data Analysis (EDA) techniques using Python and Pandas.

```
