# 🌍 Week 1 Project — Climate Risk and Disaster Management

## 📌 Project Overview
This repository contains my **Week 1 submission** for the Climate Risk and Disaster Management project.  
The goal for Week 1 is to **understand the dataset** by performing basic exploratory checks.

## 📂 Dataset
- Source: [Kaggle — Climate Risk and Economic Losses](https://www.kaggle.com/datasets/thedevastator/global-climate-risk-index-and-related-economic-l)  
- File used: `/content/climate-risk-index-1.csv` (downloaded and included locally)  
- Contains **182 countries** with climate risk indicators, human impacts, and economic losses.

### Key Columns
- `country` — Country name  
- `cri_rank`, `cri_score` — Climate Risk Index rank & score  
- `fatalities_total`, `fatalities_per_100k_total` — Human impacts  
- `losses_per_gdp__total`, `losses_usdm_ppp_total` — Economic impacts  

## 🛠️ Tasks Completed
1. **Imported necessary libraries** (`pandas`, `numpy`)  
2. **Loaded dataset** into a Pandas DataFrame  
3. **Explored dataset** using:
   - `.info()` — structure and data types  
   - `.describe()` — statistical summary  
   - `.isnull().sum()` — missing value check  

## 📑 Files in this Repository
- `Week1_CRDM_DataUnderstanding.ipynb` → Jupyter Notebook with Week 1 exploration  
- `/content/climate-risk-index-1.csv` → Dataset file  
- `README.md` → Project documentation  
