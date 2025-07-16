# 🕵️‍♀️ Crime Data Analysis & Visualization

Welcome to the **Crime Data Analysis** project! This repository explores a real-world crime dataset through data cleaning and insightful visualizations. The goal is to uncover patterns in frequency, geography, and types of crimes to support better understanding and informed decision-making.

---

## 📦 About the Dataset

This dataset contains detailed records of reported crime incidents. Each row represents one crime report and includes various attributes like the time, date, crime category, location, weapon used, and victim details.

- Each row = one reported crime
- Rich metadata about the incident and surroundings
- Enables crime pattern analysis by time, type, and location

---

## 📁 Files in This Repository

- `Crime_Data.csv`: The **raw dataset** directly as obtained from the source.
- `crime_data_cleaned.csv`: The **cleaned and processed dataset**, ready for analysis.
- `crime_analysis.ipynb`: The **Jupyter Notebook** with all code for cleaning, visualizations, and insights.
- `README.md`: You're reading it – the complete documentation for this project.

---

## 🧽 Data Cleaning Process

To ensure accurate and consistent analysis, the following steps were applied:

- Converted `DATE OCC` and `Date Rptd` into proper datetime formats
- Removed rows with missing or invalid date/time values
- Verified and corrected data types for numerical and string columns
- Extracted `Month` from `DATE OCC` for time-series analysis
- Cleaned up unnecessary columns (like unnamed index)

All cleaned data is stored in `crime_data_cleaned.csv`.

---

## 📊 Visualizations Included

The Jupyter Notebook contains clear, informative plots:

1. **Monthly Crime Trend**  
   - A line plot showing how crimes fluctuate across different months.
   - Helps identify seasonal or monthly spikes in criminal activity.

2. **Top 10 Crime Types**  
   - A bar chart showcasing the most frequently reported crime categories.
   - Provides insights into what types of crimes are most prevalent.

These charts can easily be extended with:
- Crime density maps by location (heatmaps)
- Time-of-day crime distribution
- Analysis by victim demographics
- Weapon usage trends

---

## 📘 Column Descriptions

Here’s what some of the key columns represent:

- `DR_NO`: Unique crime report ID.
- `Date Rptd`: Date the crime was reported to the police.
- `DATE OCC`: Actual date the crime occurred.
- `TIME OCC`: Time of the incident in 24-hour format.
- `AREA NAME`: The name of the police reporting district.
- `Crm Cd Desc`: Description of the crime (e.g., THEFT, ROBBERY).
- `Vict Age`, `Vict Sex`, `Vict Descent`: Victim's age, gender, and descent.
- `Weapon Desc`: Type of weapon used, if any.
- `Status Desc`: The current status of the investigation (e.g., Arrest Made, Investigation Ongoing).
- `LAT`, `LON`: Location coordinates for mapping and geographic analysis.
- `Month`: Extracted from `DATE OCC` for time-based trends.

---


