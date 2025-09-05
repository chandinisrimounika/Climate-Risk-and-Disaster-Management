# 🌍 Climate Risk and Disaster Management

## 📌 Project Overview
This repository contains my submissions for the **Climate Risk and Disaster Management** project.  
The project is developed incrementally, with weekly milestones.  

- **Week 1:** Dataset understanding  
- **Week 2:** Exploratory Data Analysis (EDA), data transformation, and feature selection  
- (Further weeks will extend into modeling, evaluation, and insights)

---

## 📂 Dataset
- Source: [Kaggle — Climate Risk and Economic Losses](https://www.kaggle.com/datasets/thedevastator/global-climate-risk-index-and-related-economic-l)  
- File used: `climate-risk-index-1.csv` (downloaded and included locally)  
- Contains **182 countries** with climate risk indicators, human impacts, and economic losses.

### Key Columns
- `country` — Country name  
- `cri_rank`, `cri_score` — Climate Risk Index rank & score  
- `fatalities_total`, `fatalities_per_100k_total` — Human impacts  
- `losses_per_gdp__total`, `losses_usdm_ppp_total` — Economic impacts  

---

## 🛠️ Week 1 Contributions — Data Understanding
1. **Imported necessary libraries** (`pandas`, `numpy`)  
2. **Loaded dataset** into a Pandas DataFrame  
3. **Explored dataset** using:  
   - `.info()` — structure and data types  
   - `.describe()` — statistical summary  
   - `.isnull().sum()` — missing value check  

---

## 🛠️ Week 2 Contributions — EDA, Transformation, Feature Selection
1. **Exploratory Data Analysis (EDA)**  
   - Histograms for numeric variables (fatalities, losses, etc.)  
   - Value counts for categorical variables (`country`)  
   - Boxplots & scatter plots to explore relationships  
   - Correlation heatmap of numeric features  

2. **Data Transformation**  
   - Handled missing values with imputation (median for numeric, `Unknown` for categorical)  
   - Converted numeric-like columns to numeric  
   - Applied log-transform to skewed monetary columns (`damage_property_usd`, `damage_crops_usd`)  
   - Removed duplicates (if any)  

3. **Feature Selection**  
   - Used **correlation with target** (`losses_usdm_ppp_total` chosen as example)  
   - Applied **SelectKBest (F-test)** to rank most relevant predictors  
   - Built a **RandomForest model** to extract feature importances  
   - Consolidated selected features and exported:  
     - `selected_features_week2.csv`  
     - `cleaned_week2_selected.csv`  

---

## 📑 Files in this Repository
- `Week1_CRDM_DataUnderstanding.ipynb` → Week 1 notebook (data understanding)  
- `Week2_CRDM_EDA_FeatureSelection.ipynb` → Week 2 notebook (EDA, transformation, feature selection)  
- `climate-risk-index-1.csv` → Dataset file  
- `selected_features_week2.csv` → List of selected features (Week 2)  
- `cleaned_week2_selected.csv` → Cleaned dataset with selected features (Week 2)  
- `README.md` → Project documentation  

---
