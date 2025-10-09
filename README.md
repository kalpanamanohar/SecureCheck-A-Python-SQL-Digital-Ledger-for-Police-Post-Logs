# 🚔 SECURE CHECK: A Python + SQL Digital Leader For Police Post Logs

## 📌 Project Overview
Police check posts require a centralized system for logging, tracking, and analyzing vehicle movements. Currently, manual logging and inefficient databases slow down security processes. This project aims to build an SQL-based check post database with a Python-powered dashboard for real-time insights and alerts.

---
![Streamlit](https://img.shields.io/badge/Framework-Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Python](https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![MySQL](https://img.shields.io/badge/Database-MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

---
## 🎯 Features
- 🔹 **Real-time Logging** of vehicles and personnel at check posts.  
- 🔹 **Automated Suspect Identification** using SQL queries.  
- 🔹 **Check Post Efficiency Monitoring** with Python analytics.  
- 🔹 **Crime Pattern Analysis** with data science workflows.  
- 🔹 **Centralized Database** for multi-location check post management.  

---

## ⚙️ Tech Stack

| Component | Technology |
|------------|-------------|
| 💻 **Frontend/UI** | Streamlit |
| ⚙️ **Backend** | Python |
| 🗄️ **Database** | MySQL |
| 📊 **Visualization** | Plotly Express |
| 🧮 **Data Handling** | Pandas |
| ⏱️ **Datetime Management** | datetime |

---
## 🚨 Key Features

### 🔹 1. **Introduction Page**
> Overview of the project with visuals and highlights of its purpose.

### 🔹 2. **Full Data Table**
> Displays the **complete SQL dataset** directly from the `Traffic_Stops.digital_ledger` table.

### 🔹 3. **Key Metrics Dashboard**
> Real-time statistics and dynamic charts:
- 🚦 Total Police Stops  
- 🚓 Total Arrests  
- ⚠️ Total Warnings  
- 💊 Drug-Related Stops  
- 🧍 Gender Distribution  
- 📈 Monthly Trends and 📊 Hourly Heatmaps  

### 🔹 4. **Advanced Insights**
> A collection of pre-defined **SQL analytical queries** with instant visualization:
- Arrest rate by **age**, **race**, and **gender**  
- Night vs. Day arrest comparison  
- Top 10 drug-related vehicles  
- Common violations among young drivers  
- Country-wise stop analysis  
- Violation trends and arrest rate breakdowns  

### 🔹 5. **Predictive Outcome Form**
> Interactive Streamlit form that simulates a police stop scenario and predicts:
- Stop description  
- Violation type  
- Outcome summary (Ticket, Arrest, Warning)  

---
## 🗄️ Database Schema
The application connects to a MySQL database named `Traffic_Stops`, which contains a table called `digital_ledger`.

### Table: digital_ledger
| Column Name | Description |
|--------------|-------------|
| `stop_date` | Date when the traffic stop occurred |
| `stop_time` | Time of the stop (formatted as HH:MM:SS) |
| `driver_age` | Age of the driver involved |
| `driver_gender` | Gender of the driver (Male/Female) |
| `driver_race` | Race of the driver |
| `violation` | Reason or type of traffic violation |
| `search_conducted` | Indicates if a search was conducted (1 = Yes, 0 = No) |
| `is_arrested` | Indicates if an arrest was made (1 = Yes, 0 = No) |
| `drugs_related_stop` | Indicates if the stop was drug-related (1 = Yes, 0 = No) |
| `stop_duration` | Duration category of the stop (e.g., 0-15 Min, 16-30 Min, 30+ Min) |
| `stop_outcome` | Result of the stop (Ticket, Arrest, Warning) |
| `country_name` | Name of the country where the stop occurred |
| `vehicle_number` | Vehicle registration number involved in the stop |

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
## 📊 Visualization Types

| Type | Description |
|------|--------------|
| 📈 **Line Chart** | Monthly traffic stop trends |
| 🥧 **Pie Chart** | Gender distribution |
| 📊 **Bar Chart** | Arrest & violation rates |
| 🌡️ **Heatmap** | Stop frequency by hour & weekday |

---

## 🧩 How It Works

1. Establishes a **secure MySQL connection** using `pymysql`.  
2. Fetches real-time records into a **Pandas DataFrame**.  
3. Processes and visualizes using **Plotly Express**.  
4. Displays dynamic results through **Streamlit** pages.  
5. Allows SQL-based deep dives through the *Advanced Insights* page.

---

## ⚙️ Installation & Setup

# Clone the repository
git clone https://github.com/kalpanamanohar/securecheck.git
cd securecheck

---

2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook SECURE_CHECK.ipynb

---

![image alt](https://github.com/kalpanamanohar/SecureCheck-A-Python-SQL-Digital-Ledger-for-Police-Post-Logs/blob/af1c31b2777532f75bb7197c7023342711988925/Introduction.jpeg)
![image alt](https://github.com/kalpanamanohar/SecureCheck-A-Python-SQL-Digital-Ledger-for-Police-Post-Logs/blob/af1c31b2777532f75bb7197c7023342711988925/Full_table.jpeg)
![image alt](https://github.com/kalpanamanohar/SecureCheck-A-Python-SQL-Digital-Ledger-for-Police-Post-Logs/blob/af1c31b2777532f75bb7197c7023342711988925/KEYmetric.jpeg)
![image alt](https://github.com/kalpanamanohar/SecureCheck-A-Python-SQL-Digital-Ledger-for-Police-Post-Logs/blob/af1c31b2777532f75bb7197c7023342711988925/keymetric2.jpeg)
![image alt](https://github.com/kalpanamanohar/SecureCheck-A-Python-SQL-Digital-Ledger-for-Police-Post-Logs/blob/af1c31b2777532f75bb7197c7023342711988925/keymetric3.jpeg)
![image alt](https://github.com/kalpanamanohar/SecureCheck-A-Python-SQL-Digital-Ledger-for-Police-Post-Logs/blob/af1c31b2777532f75bb7197c7023342711988925/keymetric4.jpeg)
![image alt](https://github.com/kalpanamanohar/SecureCheck-A-Python-SQL-Digital-Ledger-for-Police-Post-Logs/blob/af1c31b2777532f75bb7197c7023342711988925/advancedinsights.jpeg)
![image alt](https://github.com/kalpanamanohar/SecureCheck-A-Python-SQL-Digital-Ledger-for-Police-Post-Logs/blob/af1c31b2777532f75bb7197c7023342711988925/advancedinsights2.jpeg)
![image alt](https://github.com/kalpanamanohar/SecureCheck-A-Python-SQL-Digital-Ledger-for-Police-Post-Logs/blob/af1c31b2777532f75bb7197c7023342711988925/predictionoutcome.jpeg)
![image alt](https://github.com/kalpanamanohar/SecureCheck-A-Python-SQL-Digital-Ledger-for-Police-Post-Logs/blob/af1c31b2777532f75bb7197c7023342711988925/predictionoutcome2.jpeg)

