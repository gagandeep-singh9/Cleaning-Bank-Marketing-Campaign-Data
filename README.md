# 📊 Bank Marketing Data Cleaning & Structuring  
_A clean, structured dataset ready for database import & analysis_  

## ✨ Highlights  
- 🔍 **Transformed raw marketing data** into three tidy, analysis-ready datasets (`client.csv`, `campaign.csv`, `economics.csv`).  
- 🧼 **Robust cleaning applied**: handled missing values, standardized categorical variables, and converted fields to proper data types.  
- 🗄️ **Database-ready format**: structured to match PostgreSQL schema requirements for seamless future imports.  
- 📅 **Smart feature engineering**: constructed a proper `last_contact_date` field from separate day/month/year columns.  
- ⚡ **Boolean conversions**: converted marketing outcomes, credit defaults, and mortgages into clean boolean flags for analysis.  

## ℹ️ Overview  
This project cleans and reformats the **bank_marketing.csv** dataset collected from a personal loan marketing campaign. The goal is to ensure the data is tidy, consistent, and compatible with the bank’s PostgreSQL database so that future campaign data can be integrated effortlessly.  

The cleaned outputs (`client.csv`, `campaign.csv`, and `economics.csv`) are designed with explicit typing, clear column naming, and standardized formats. This makes downstream analysis, visualization, and machine learning much easier and more reliable.  

Personal loans are a major source of revenue for banks, and this project directly supports the bank’s ability to evaluate campaign performance and plan more effective strategies.  

## 🛠 Tech Stack  
- **Python** – main language for data wrangling  
- **Pandas** – data cleaning, transformation, and splitting  
- **NumPy** – handling missing values & type conversions  


These tools were chosen for their speed, readability, and strong ecosystem support for data processing.  

## 🧩 Project Structure  

- **client.csv** → demographic and financial info (job, marital status, credit, mortgage).  
- **campaign.csv** → campaign contact history and outcomes, including `last_contact_date`.  
- **economics.csv** → external macroeconomic indicators.  

## ⚡ Optimizations  
- Replaced `"unknown"` with `NaN` for clarity and future imputation.  
- Standardized categorical variables (`job`, `education`) by replacing `.` with `_`.  
- Converted binary responses into **booleans**, reducing storage footprint and improving query efficiency.  
- Engineered `last_contact_date` to enable time-series analysis of campaign efforts.  

## 📚 Lessons Learned  
- 🗃️ Importance of **structuring raw data** for real-world database integration.  
- 🔄 Learned how **data type enforcement** (e.g., booleans, datetimes) improves downstream usability.  
- 🧩 Reinforced how **splitting data into logical subsets** (client, campaign, economics) makes analysis cleaner and more scalable.  

---

🚀 With this project, the bank’s data is now **clean, structured, and ready for advanced analytics or predictive modeling.**  
