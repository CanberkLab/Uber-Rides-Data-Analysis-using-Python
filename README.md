# 🚗 Uber Trips Data Analysis Project

## 📌 Overview

This project focuses on analyzing an Uber trips dataset using Python. The goal is to clean, preprocess, and explore the data to uncover patterns related to trip categories, purposes, time distribution, and mileage.

The analysis includes data preprocessing, feature engineering, visualization, and correlation analysis.

---

## 📂 Dataset

The dataset used in this project contains information about Uber trips, including:

* Start and end dates
* Trip category (Business/Personal)
* Purpose of the trip
* Distance (miles)

---

## ⚙️ Technologies Used

* Python
* Pandas → Data manipulation
* NumPy → Numerical operations
* Matplotlib & Seaborn → Data visualization
* Scikit-learn → Encoding categorical variables

---

## 🧹 Data Preprocessing

The following steps were applied:

* Loaded dataset using Pandas
* Handled missing values:

  * `PURPOSE` filled with `"NOT"`
* Converted date columns:

  * `START_DATE` and `END_DATE` → datetime format
* Extracted new features:

  * `date` (only date)
  * `time` (hour)
  * `day-night` (Morning, Afternoon, Evening, Night)
* Removed:

  * Missing values (`dropna`)
  * Duplicate rows

---

## 🔧 Feature Engineering

Additional features created:

* **Time-based features**

  * Hour of trip
  * Day of week
  * Month

* **Categorical encoding**

  * One-Hot Encoding applied to:

    * `CATEGORY`
    * `PURPOSE`

---

## 📊 Data Visualization

Several visualizations were created:

### 1. Category Distribution

* Shows frequency of Business vs Personal trips

### 2. Purpose Distribution

* Displays why trips were taken

### 3. Day-Night Distribution

* Groups trips into:

  * Morning
  * Afternoon
  * Evening
  * Night

### 4. Category vs Purpose

* Compares trip purposes across categories

### 5. Monthly Analysis

* Number of trips per month
* Maximum miles traveled per month

### 6. Weekly Analysis

* Trip distribution across days of the week

### 7. Outlier Detection

* Boxplots used to analyze:

  * Overall miles
  * Miles under 100 (filtered)

### 8. Correlation Heatmap

* Shows relationships between numerical features

---

## 📈 Key Insights (Example)

* Business trips may dominate certain purposes
* Most trips occur during specific times of the day
* Some months have higher travel intensity
* Outliers exist in trip distances

---

## 🚀 How to Run

1. Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

2. Update dataset path:

```python
uber_data_set = "your_path/UberDataset.csv"
```

3. Run the script in Jupyter Notebook or Python environment

---

## 📌 Notes

* Make sure dataset path is correct
* Some visualizations may vary depending on dataset size
* One-Hot Encoding increases number of columns significantly

---

## 💡 Future Improvements

* Add machine learning model (prediction of trip category or distance)
* Perform clustering analysis
* Build dashboard (Power BI / Tableau)
* Optimize feature selection

---

## 👨‍💻 Author

Canberk Yılmaz

---
