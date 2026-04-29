# 📊 Sales Data Analysis & Prediction Project

## 🚀 Overview

This project focuses on **Sales Data Analysis and Prediction** using Python.
It includes:

* Data cleaning & preprocessing
* Exploratory Data Analysis (EDA)
* Data visualization
* Machine Learning (Logistic Regression)
* Sales growth prediction

The goal is to extract meaningful insights and predict **High Sales vs Low Sales**.

---

## 📁 Dataset

* File used: `updated_csv_v2.csv`
* Key columns:

  * Order Date
  * State, City
  * Category, Sub-Category
  * Quantity
  * Amount (Sales)
  * Profit
  * Payment Mode

---

## ⚙️ Technologies Used

* Python 🐍
* NumPy
* Pandas
* Seaborn
* Matplotlib
* Scikit-learn

---

## 🧹 Data Preprocessing

* Removed duplicate records
* Converted `Order Date` to datetime format
* Created new column:

  * `Month` (for time-based analysis)
  * `High_Sales` (binary classification target)

```python
df['High_Sales'] = (df['Amount'] > df['Amount'].median()).astype(int)
```

---

## 📊 Exploratory Data Analysis (EDA)

### 🔹 1. Sales by State

* Visualized number of sales across states
* Identified top-performing regions

### 🔹 2. Quantity by Category

* Compared total quantity sold across categories

### 🔹 3. Sales by City & Sub-Category

* Heatmaps used to analyze:

  * Top cities per sub-category
  * Overall distribution of sales

### 🔹 4. Top 3 Cities per Category

* Used FacetGrid to visualize best-performing cities

### 🔹 5. Profit by Month

* Time-series analysis of profit trends

### 🔹 6. Profit by Sub-Category

* Identified most and least profitable sub-categories

### 🔹 7. Payment Mode Analysis

* Pie chart showing quantity distribution by payment method

---

## 📈 Key Metrics

* Total Sales 💰
* Total Profit 📊
* Total Quantity 📦

---

## 🤖 Machine Learning Model

### 🔹 Model Used:

* Logistic Regression

### 🔹 Features:

* Quantity
* Profit

### 🔹 Target:

* High Sales (1) / Low Sales (0)

### 🔹 Train-Test Split:

* 80% Training
* 20% Testing

---

## 📊 Model Evaluation

* Accuracy
* Precision

```python
Accuracy: XX%
Precision: XX%
```

---

## 🔮 Sales Prediction (2024)

* Compared:

  * Actual Sales (2023)
  * Predicted High Sales (2024)

### 📌 Logic:

* Predict high-sales transactions for 2024
* Sum predicted sales
* Calculate growth %

```python
Sales Growth = ((Predicted_2024 - Sales_2023) / Sales_2023) * 100
```

---

## 📌 Results

* Identified top-performing states, cities, and categories
* Visualized sales and profit trends
* Built a predictive model for sales classification
* Estimated **future sales growth**

---

## 📂 Project Structure

```
├── updated_csv_v2.csv
├── analysis.ipynb / main.py
├── README.md
```

---

## ▶️ How to Run

1. Clone the repository:

```bash
https://github.com/vaibhavsable18/data_science
```

2. Install dependencies:

```bash
pip install numpy pandas seaborn matplotlib scikit-learn
```

3. Run the script:

```bash
python main.py
```

---

## 📌 Future Improvements

* Use advanced models (Random Forest, XGBoost)
* Add dashboard (Streamlit / Power BI)
* Improve feature engineering
* Hyperparameter tuning

---

## 🙌 Author

**Vaibhav Sable**
Final Year Computer Engineering Student

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!
