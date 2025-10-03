# 🚔 SECURE CHECK: A Python + SQL Digital Leader For Police Post Logs

## 📌 Project Overview
Police check posts require a centralized system for logging, tracking, and analyzing vehicle movements. Currently, manual logging and inefficient databases slow down security processes. This project aims to build an SQL-based check post database with a Python-powered dashboard for real-time insights and alerts.

---

## 🎯 Features
- 🔹 **Real-time Logging** of vehicles and personnel at check posts.  
- 🔹 **Automated Suspect Identification** using SQL queries.  
- 🔹 **Check Post Efficiency Monitoring** with Python analytics.  
- 🔹 **Crime Pattern Analysis** with data science workflows.  
- 🔹 **Centralized Database** for multi-location check post management.  

---

## 🛠️ Tech Stack
- **Programming Language:** Python (Jupyter Notebook)  
- **Libraries Used:**  
  - `pandas` – data handling  
  - `numpy` – numerical computations  
  - `matplotlib` – data visualization  
- **Database:** MySQL (for structured queries and suspect detection)  
- **Dataset:** Example dataset `Traffic_Stops.csv`  

---

## 📑 Approach:

1. **Data Collection & Loading**  
   - Imported the dataset `Traffic_Stops.csv` using Python (Pandas).  
   - Created an SQL-compatible structure to store vehicle stop details.

2. **Data Preprocessing & Cleaning**  
   - Checked for missing values and inconsistencies.  
   - Cleaned column names and standardized the dataset for analysis.  

3. **Exploratory Data Analysis (EDA)**  
   - Displayed first few records for verification.  
   - Analyzed trends in vehicle stops, violations, and officer activity.  
   - Used **Pandas & NumPy** for data summaries.  

4. **SQL Integration**  
   - Designed SQL queries to:  
     - Search for specific vehicles.  
     - Identify **suspect vehicles** based on predefined conditions.  
     - Generate reports for multiple check posts.  

5. **Data Visualization**  
   - Used **Matplotlib** to create charts/graphs showing:  
     - Frequency of vehicle stops.  
     - Distribution of violations.  
     - Efficiency of check post operations.  

6. **Analysis & Insights**  
   - Highlighted patterns in traffic stops.  
   - Demonstrated how SQL + Python can be combined for **crime pattern detection**.  
   - Provided a framework for **centralized monitoring** of all check posts.  

---

## ⚙️ Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/kalpanamanohar/SECURE_CHECK.git
   cd SECURE_CHECK

---

2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook SECURE_CHECK.ipynb

---

## 📊 Example Workflow

Here’s how the system works step by step:

### 1. Load Dataset
```python
import pandas as pd

# Load traffic stop records
df = pd.read_csv("Traffic_Stops.csv")
df.head()

### 2. Basic Data Exploration
```python
# Check missing values
df.isnull().sum()

# Summary statistics
df.describe()

### 3. Store & Query with SQL
import pymysql
myconnection = pymysql.connect(host = '127.0.0.1',user='root',password='Mirthi@26')
cur = myconnection.cursor()
cur.execute("create database Traffic_Stops")

# Example query:  Display Top 10 vehicle_Number involved in drug-related stops
cur.execute("""select vehicle_number,count(*) as count from Traffic_Stops.digital_ledger
where drugs_related_stop=TRUE
group by vehicle_number
order by count desc
limit 10""")

a=cur.fetchall()
from tabulate import tabulate
print(tabulate(a,headers=[i[0] for i in cur.description],tablefmt='mysql'))



