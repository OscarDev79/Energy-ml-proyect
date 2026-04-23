# 🏢 Energy Efficiency Prediction with Machine Learning

## 📌 Project Overview
This project focuses on predicting the **heating load (energy efficiency)** of buildings using Machine Learning techniques.

The goal is to analyze how different architectural features impact energy consumption and build a predictive model with high accuracy.

---

## 📊 Dataset
- Source: UCI Machine Learning Repository  
- Instances: 768  
- Features: 8 input variables related to building design  
- Targets:
  - Heating Load (used in this project)
  - Cooling Load  

---

## ⚙️ Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-Learn  
- Matplotlib  

---

## 🔍 Workflow

1. **Data Loading & Preprocessing**
   - Import dataset from UCI
   - Rename columns for clarity

2. **Exploratory Setup**
   - Feature selection
   - Target variable definition

3. **Model Training**
   - Random Forest Regressor
   - Train/Test split (80/20)

4. **Model Evaluation**
   - Mean Absolute Error (MAE)
   - R² Score

5. **Hyperparameter Tuning**
   - GridSearchCV with cross-validation (cv=5)
   - Optimization of:
     - `n_estimators`
     - `max_depth`

6. **Feature Importance Analysis**
   - Identification of most influential variables

---

## 📈 Results

### 🔹 Base Model
- R²: **0.989**

### 🔹 Optimized Model (GridSearchCV)
- R²: **0.997**
- MAE: **0.356**

### 🔹 Best Hyperparameters
```python
{'max_depth': 10, 'n_estimators': 100}
