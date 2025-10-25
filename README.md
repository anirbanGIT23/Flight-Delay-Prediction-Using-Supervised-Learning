# ✈️ Flight Delay Prediction Using Machine Learning

## 🧩 Overview
This project predicts **flight delay duration (in minutes)** using historical flight and weather data. The model helps airlines and passengers estimate expected delays before departure, improving scheduling efficiency and passenger satisfaction.

The workflow includes **data preprocessing, feature engineering, model training, evaluation, and inference** using a large dataset (~3 million rows, 32 columns).

---

## 🗂️ Project Structure
```
├── flight_delay.ipynb        # Jupyter Notebook with full pipeline
├── README.md                 # Project documentation
├── data/                     # (optional) folder for raw/processed data
├── models/                   # trained models (if saved)
└── outputs/                  # evaluation metrics and inference results
```

---

## ⚙️ Tech Stack
- **Language:** Python 3.x  
- **Environment:** Jupyter Notebook  
- **Key Libraries:**
  - pandas, numpy – data manipulation  
  - matplotlib, seaborn – exploratory data analysis (EDA)  
  - scikit-learn – preprocessing, model training, evaluation  
  - joblib – model serialization (optional)

---

## 📊 Dataset
- **Size:** ~3,000,000 rows × 32 columns  
- **Target Variable:** `Delay` (minutes)  
- **Features:** flight schedule, carrier, origin, destination, distance, aircraft, weather, etc.  
- **Type:** Supervised regression  

> Note: The dataset used here is a **dummy dataset** for demonstration and methodology validation purposes.

---

## 🧠 Methodology

### 1. **Data Preprocessing**
- Handled missing and inconsistent values  
- Encoded categorical variables using label/one-hot encoding  
- Normalized numerical features where needed  
- Removed outliers and irrelevant columns  

### 2. **Exploratory Data Analysis (EDA)**
- Visualized distribution of delays, correlations, and feature importance  
- Identified peak delay times, routes, and carriers with the most delays  

### 3. **Feature Engineering**
- Created new temporal features (e.g., day of week, hour of day)  
- Derived weather-based and route-based delay indicators  
- Optimized feature set based on correlation and importance  

### 4. **Model Training**
- Compared multiple regression models:  
  - Linear Regression  
  - Decision Tree Regressor  
  - Random Forest Regressor *(final model)*  
- Tuned hyperparameters using grid search and cross-validation  

### 5. **Evaluation Metrics**
- **MAE (Mean Absolute Error)**  
- **RMSE (Root Mean Squared Error)**  
- **R² Score (Coefficient of Determination)**  

### 6. **Inference**
- Generated predictions on unseen (test) data  
- Saved model for later deployment or batch prediction  

---

## 🧪 Results
| Model | MAE | RMSE | R² |
|--------|------|------|----|
| Linear Regression | – | – | – |
| Decision Tree | – | – | – |
| **Random Forest (Final)** | **X.XX** | **X.XX** | **0.XX** |

*(Replace with actual metrics once finalized)*

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/<your-username>/flight-delay-prediction.git
cd flight-delay-prediction
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```


