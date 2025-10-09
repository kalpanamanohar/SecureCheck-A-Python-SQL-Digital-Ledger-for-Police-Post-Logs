# 🚔 SECURE CHECK: A Python + SQL Digital Leader For Police Post Logs

## 📌 Project Overview
Police check posts need a unified, real-time digital log for tracking vehicle and personnel movements. This project leverages a MySQL-backed database and a Python-powered Streamlit dashboard for instant insights, advanced analytics, and automated alerts. Data is efficiently queried via SQL and visualized with Plotly in Streamlit, delivering actionable metrics for law enforcement.

---

![Streamlit](https://img.shields.io/badge/Framework-Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![Python](https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![MySQL](https://img.shields.io/badge/Database-MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

---

## 🎯 Features

- **Real-time Logging** of vehicles and personnel at check posts.
- **Automated Suspect Identification** using SQL queries.
- **Check Post Efficiency Monitoring** (key metrics) with dashboard analytics.
- **Crime Pattern Analysis** powered by SQL+Python workflows.
- **Centralized Database** for multi-location check post management.
- **Instant Data Visualization** with dynamic Streamlit dashboard and Plotly charts.

---

## ⚙️ Tech Stack

| Component        | Technology          |
|------------------|--------------------|
| **Frontend/UI**  | Streamlit          |
| **Backend**      | Python             |
| **Database**     | MySQL              |
| **Visualization**| Plotly Express     |
| **Data Handling**| Pandas             |
| **Datetime**     | datetime           |
| **SQL Adapter**  | PyMySQL            |

---

## 🚨 Key Features

### 1. Introduction Page
- Project overview and Streamlit-driven visual highlights.

### 2. Full Data Table
- Live, comprehensive data table from the MySQL `Traffic_Stops.digital_ledger` table.

### 3. Key Metrics Dashboard
- Real-time metrics like:
  - Total Police Stops
  - Total Arrests
  - Total Warnings
  - Drug-Related Stops
  - Gender Distribution
  - Traffic Stop Trends
  - Hourly Heatmaps

### 4. Advanced Insights
- Predefined SQL analytical queries with instant Plotly-based visualization:
  - Arrest rates (by age, race, gender)
  - Night vs. day arrest analysis
  - Top 10 drug-linked vehicles
  - Most common violations for young drivers
  - Country-wise statistics
  - Violation and arrest trend breakdowns

### 5. Predictive Outcome Form
- Interactive form that predicts violation types & stop outcomes based on scenario simulation (input values).

---

## 🗄️ Database Schema

| Column Name         | Description                                    |
|---------------------|------------------------------------------------|
| `stop_date`         | Date of the traffic stop                       |
| `stop_time`         | Time of stop (HH:MM:SS)                        |
| `driver_age`        | Age of the driver                              |
| `driver_gender`     | Gender of the driver                           |
| `driver_race`       | Race of the driver                             |
| `violation`         | Traffic violation type                         |
| `search_conducted`  | Was a search conducted (1 = Yes, 0 = No)       |
| `is_arrested`       | Was an arrest made (1 = Yes, 0 = No)           |
| `drugs_related_stop`| Is the stop drug-related (1 = Yes, 0 = No)     |
| `stop_duration`     | Duration category (e.g., 0-15 Min, 16-30 Min)  |
| `stop_outcome`      | Outcome (Ticket, Arrest, Warning)              |
| `country_name`      | Country                                        |
| `vehicle_number`    | Vehicle registration number                    |

---

## 📑 Approach

- **Data Collection & Loading:** Import CSV data to MySQL (using Pandas, PyMySQL).
- **Preprocessing & Cleaning:** Checked and filled missing data, standardized the schema.
- **Exploratory Data Analysis:** Used Pandas; all dashboard visualizations built with Plotly Express inside Streamlit.
- **SQL Integration:** All vehicle, suspect, and trend analysis performed via SQL queries using PyMySQL.
- **Real-Time Dashboard:** Streamlit app presents key tables, filters, and advanced SQL-driven metrics and visualizations.
- **Centralized Monitoring:** Every query and analytic is rendered instantly via Streamlit/Plotly.
- **No use of Matplotlib or NumPy for dashboard or core analytics.**

---

## 📊 Visualization Types

| Type      | Description                            |
|-----------|----------------------------------------|
| Line      | Monthly traffic stop trends            |
| Pie       | Gender distribution                    |
| Bar       | Arrest & violation rates               |
| Heatmap   | Stop frequency (by hour & weekday)     |

---

## 🧩 How It Works

1. Connects securely to MySQL (via PyMySQL).
2. Fetches real-time records into Pandas DataFrames.
3. Generates analytics and visuals with Plotly Express.
4. Serves the dashboard interactively through Streamlit.
5. Advanced, parameterized SQL queries for deep insights.

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

