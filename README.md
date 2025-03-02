# ✈️ Flight Delay Prediction using Machine Learning  

**Author:** Zohaib Gujjar  
**Technologies:** Python, Machine Learning, Data Science, Decision Tree, XGBoost, SVM, Logistic Regression  

---

## Project Overview  
Flight delays are a significant challenge in the aviation industry, affecting passengers, airlines, and airport management. This project aims to **predict flight delays** using **historical flight data (2018-2020)** and **machine learning models**.  

A flight is considered **delayed** if the arrival delay (`ARR_DELAY`) is **greater than 15 minutes**. A new binary variable **`IS_DELAY`** was introduced for classification:  
- **1** → Delayed  
- **0** → Not Delayed  

The goal is to build a **high-accuracy predictive model** to assist stakeholders in decision-making and optimizing flight schedules.

---

## Dataset  

- **Source:** Historical flight records (2018-2020)  
- **Format:** CSV  
- **Key Features:**
  - `FL_DATE` → Flight Date  
  - `OP_CARRIER` → Operating Carrier  
  - `ORIGIN`, `DEST` → Airport codes  
  - `DEP_TIME`, `ARR_TIME` → Actual departure & arrival times  
  - `DEP_DELAY`, `ARR_DELAY` → Delay durations  
  - `CANCELLED`, `DIVERTED` → Flight cancellation & diversion info  

---

## Data Preprocessing  

✅ **Data Cleaning**  
- Handled missing values  
- Removed irrelevant columns  
- Converted `FL_DATE` to datetime format
- Converted Categorical data to Numerical for better processing

✅ **Feature Engineering**  
- Created `IS_DELAY` column based on arrival delay (`ARR_DELAY > 15`)  
- Encoded categorical features (`OP_CARRIER`, `ORIGIN`, `DEST`, etc.)  

✅ **Final Dataset Preparation**  
- Merged data from **2018, 2019, and 2020**  
- Scaled and normalized data for machine learning  

---

## Machine Learning Models  

| Model     
| **Decision Tree**
| **Logistic Regression**
| **Support Vector Machine (SVM)** 
| **XGBoost**

**Evaluation Metrics:**
- **Training Accuracy**: Performance on training data  
- **Testing Accuracy**: Performance on unseen data  
- **Overfitting Check**: Difference between training and testing accuracy
- 
---
