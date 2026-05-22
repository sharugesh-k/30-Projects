# Sales Data Cleaning Project using Python & Pandas

## 📌 Project Overview

This project focuses on cleaning and preprocessing raw sales transaction data using Python and Pandas. The dataset contained missing values, duplicate records, invalid entries, and incorrect data types. The goal of this project was to transform messy raw data into a clean and analysis-ready dataset.

This project demonstrates practical Data Analytics and Data Engineering skills including:

* Data Cleaning
* Data Preprocessing
* Data Validation
* Handling Missing Values
* Removing Duplicates
* Data Type Conversion
* CSV File Processing using Pandas

---

## 🚀 Technologies Used

* Python
* Pandas
* NumPy
* Jupyter Notebook
* CSV Dataset

---

## 📂 Project Structure

```bash
├── sales.csv                 # Raw sales dataset
├── cleaned_sales.csv         # Cleaned dataset after preprocessing
├── Sales_data_Cleaning.ipynb # Jupyter notebook containing full workflow
└── README.md                 # Project documentation
```

---

## 🧹 Data Cleaning Steps Performed

### ✅ 1. Loaded Raw Dataset

Imported the sales dataset using Pandas.

### ✅ 2. Inspected Data

Used:

```python
 df.info()
 df.head()
```

to understand dataset structure and detect issues.

### ✅ 3. Handled Missing Values

Removed rows containing null values.

```python
df = df.dropna()
```

### ✅ 4. Removed Duplicate Records

Detected and removed duplicate entries.

```python
df = df.drop_duplicates()
```

### ✅ 5. Removed Invalid Entries

Filtered rows containing invalid values such as:

* UNKNOWN
* ERROR

```python
df = df[~df.isin(["UNKNOWN", "ERROR"]).any(axis=1)]
```

### ✅ 6. Converted Data Types

Converted columns into proper formats for analysis.

```python
df['Quantity'] = df['Quantity'].astype(int)
df['Price Per Unit'] = df['Price Per Unit'].astype(float)
df['Total Spent'] = df['Total Spent'].astype(float)
df['Transaction Date'] = pd.to_datetime(df['Transaction Date'])
```

---

## 📊 Skills Demonstrated

This project demonstrates real-world industry skills relevant for:

* Data Analyst Roles
* Junior Data Engineer Roles
* Business Intelligence Roles
* Data Cleaning & ETL Workflows

Key skills covered:

* Data preprocessing with Pandas
* Working with structured datasets
* Data quality improvement
* Building clean datasets for analytics
* Preparing datasets for dashboards and machine learning

---

## 🎯 Project Outcome

After preprocessing:

* Missing values were removed
* Duplicate rows were cleaned
* Invalid entries were filtered
* Data types were standardized
* The dataset became ready for:

  * SQL Analysis
  * Power BI Dashboards
  * Machine Learning
  * ETL Pipelines

---

## 📈 Future Improvements

Potential future enhancements:

* Automate cleaning pipeline using ETL tools
* Upload cleaned data into PostgreSQL or BigQuery
* Build Power BI dashboard from cleaned dataset
* Perform exploratory data analysis (EDA)
* Create automated data quality reports

---

## 🔍 Keywords

Python Data Cleaning Project, Pandas Data Cleaning, Sales Data Analysis, Data Analyst Portfolio Project, Data Engineering Project, CSV Cleaning using Python, ETL Project using Pandas, Python for Data Analytics, Data Preprocessing Project, Real World Data Cleaning Project, Beginner Data Engineering Project, GitHub Data Analytics Project.

---

## 👨‍💻 Author

**Sharugesh K**
Aspiring Data Analyst | Junior Data Engineer | BI Developer
Passionate about Data Analytics, Data Engineering, Machine Learning, and Business Intelligence.


If you found this project useful, feel free to star the repository.
