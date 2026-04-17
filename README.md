#  House Price Prediction using Machine Learning
Production-style ML pipeline with preprocessing, model selection, and evaluation.

---

##  Overview
This project builds an end-to-end Machine Learning pipeline to predict house prices based on features like size and number of bedrooms. It demonstrates real-world ML practices including preprocessing, model comparison, cross-validation, and hyperparameter tuning.

---

##  Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  

---

##  Problem
House price estimation is influenced by multiple factors and manual predictions are often inaccurate. A data-driven approach is required to improve reliability and consistency.

---

##  Solution
Designed a robust ML pipeline using **scikit-learn**:

### 🔹 Data Preprocessing
- Missing value handling using `SimpleImputer`  
- Feature scaling using `StandardScaler`  
- Categorical encoding using `OneHotEncoder`  
- Combined using `ColumnTransformer`  

### 🔹 Model Building
Trained and compared multiple regression models:
- Linear Regression  
- Ridge Regression  
- Lasso Regression  
- Random Forest Regressor  
- Histogram-based Gradient Boosting Regressor  

### 🔹 Model Evaluation
- Cross-validation using `KFold`  
- Metrics used:
  - Mean Absolute Error (MAE)  
  - Root Mean Squared Error (RMSE)  
  - R² Score  

### 🔹 Hyperparameter Tuning
- Performed using `GridSearchCV` to optimize model performance  

---

## Dataset
The dataset (`house_prices.csv`) includes:
- `Size` – Area of the house (sq ft)  
- `Bedrooms` – Number of bedrooms  
- `Price` – Target variable  

---

## Model Performance

| Model                          | MAE       | RMSE      | R² Score |
|--------------------------------|-----------|-----------|----------|
| HistGradientBoosting Regressor | 32298.302 | 48263.288 | 0.826    |
| Random Forest Regressor        | 32333.104 | 49416.213 | 0.817    |
| Ridge Regression               | 49664.331 | 68595.617 | 0.648    |
| Lasso Regression               | 49667.263 | 68603.233 | 0.648    |
| Linear Regression              | 49667.159 | 68604.163 | 0.648    |

