# 🕵️‍♀️ Crime Data Analysis & Visualization

Welcome to the **Crime Data Analysis** project! This repository explores a real-world crime dataset through powerful data cleaning and visualizations. The goal is to uncover patterns in crime frequency, types, and locations to support better understanding and decision-making.

---

## 📦 Dataset Overview

This dataset contains detailed records of crime incidents reported to the police. Each entry includes metadata such as date, time, location, crime description, and weapon used (if any).

🗓️ **Timeframe**: Varies  
🌍 **Location**: Based on the dataset, likely a city in the U.S.  
📈 **Purpose**: Analyze crime trends, identify frequent crime types, visualize patterns

---

## 🧽 Data Cleaning Process

To ensure accurate analysis, the following cleaning steps were applied in the notebook:

- ✅ Converted `DATE OCC` and `Date Rptd` columns to proper `datetime` format
- ✅ Dropped rows with invalid or missing date values
- ✅ Checked and handled missing values in key columns (e.g., crime type, area name)
- ✅ Verified data types (e.g., numeric for time, latitude, longitude)
- ✅ Used only the necessary columns for visualizations to reduce clutter

These steps improved data quality and ensured reliable visual output.

---

## 📊 Visualization Summary

The notebook includes clear and informative charts to help readers understand crime patterns:

### 📅 1. Monthly Crime Trend  
A time-series line plot showing how crime volume fluctuates month-by-month.  
🔍 **Insight**: Helps identify seasonal or temporal spikes in crime.

### 🔟 2. Top 10 Crime Types  
A bar chart showing the most frequently reported crimes in the dataset.  
🔍 **Insight**: Useful for understanding what types of crimes are most common.

📌 You can easily extend this with:
- Geographic maps (heatmaps by location)
- Weapon usage analysis
- Time-of-day crime frequency
- Victim demographics

---

## 🧾 Column Descriptions

| Column Name         | Description |
|---------------------|-------------|
| `DR_NO`             | Unique ID for each crime report |
| `Date Rptd`         | Date the crime was reported |
| `DATE OCC`          | Date the crime actually occurred |
| `TIME OCC`          | Time of the incident (24-hour format) |
| `AREA`              | Numeric area code |
| `AREA NAME`         | Name of the police reporting area |
| `Rpt Dist No`       | Reporting district number |
| `Part 1-2`          | Indicates crime severity: Part I (serious) or Part II |
| `Crm Cd`            | Crime code |
| `Crm Cd Desc`       | Description of the crime (e.g., "BURGLARY") |
| `Mocodes`           | Modus operandi codes |
| `Vict Age`          | Victim's age |
| `Vict Sex`          | Victim's gender (M, F, X) |
| `Vict Descent`      | Victim’s descent/ethnicity |
| `Premis Cd`         | Premise type code |
| `Premis Desc`       | Premise description |
| `Weapon Used Cd`    | Weapon code (if applicable) |
| `Weapon Desc`       | Description of weapon used |
| `Status`            | Case status code |
| `Status Desc`       | Status description (e.g., "Investigation Continued") |
| `Crm Cd 1/2/3`      | Additional crime codes if multiple incidents reported |
| `LOCATION`          | Street-level address |
| `LAT`, `LON`        | Latitude and Longitude of the incident |
| `Month`             | Extracted month from `DATE OCC` for trend analysis |

---

## 🛠️ Tech Stack

- **Python 3.x**
- `pandas` – Data handling
- `matplotlib`, `seaborn` – Visualizations
- `jupyter` – Notebook environment
