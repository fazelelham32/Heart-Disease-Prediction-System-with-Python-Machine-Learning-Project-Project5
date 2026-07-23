# Heart-Disease-Prediction-System-with-Python-Machine-Learning-Project-Project5

Learn how to build a heart disease prediction system using Python and machine learning techniques. This step-by-step tutorial covers data preprocessing, model training, and evaluation. Perfect for beginners and experts alike!

بله. این یک **README حرفه‌ای برای GitHub** پروژه شماست:

---

# Heart Disease Prediction System

A machine learning-based web application for predicting the 10-year risk of heart disease using personal health data.  
The project includes data preprocessing, feature scaling, model training, performance evaluation, and deployment through a **Flask web application**.

## Project Overview

Heart disease is one of the leading causes of death worldwide.  
This project aims to build an intelligent prediction system that helps estimate whether a person is likely to develop heart disease within the next 10 years based on key health indicators.

The final model is integrated into a Flask-based web interface where users can enter their health information and receive a prediction result instantly.

## Features

- Data preprocessing and cleaning
- Handling missing values
- Feature scaling using normalization/standardization
- Train-test split
- Classification model training
- Model evaluation with:
  - Confusion Matrix
  - Classification Report
  - Accuracy Score
- Flask web application integration
- User-friendly prediction form
- Real-time heart disease risk prediction

## Dataset Features

The dataset includes the following attributes:

- `male`
- `age`
- `education`
- `currentSmoker`
- `cigsPerDay`
- `BPMeds`
- `prevalentStroke`
- `prevalentHyp`
- `diabetes`
- `totChol`
- `sysBP`
- `diaBP`
- `BMI`
- `heartRate`
- `glucose`
- `TenYearCHD`

## Machine Learning Workflow

### 1. Data Preprocessing
- Imported the dataset using `pandas.read_csv()`
- Handled missing values
- Removed unnecessary columns if required
- Filled binary categorical missing values using mode
- Filled numerical missing values using median/appropriate strategy

### 2. Feature Scaling
Since the dataset contains features with different ranges, scaling was applied to ensure fair model performance.

Used techniques:
- **Standardization**
- **Normalization (Min-Max Scaling)**

### 3. Data Splitting
The dataset was split into:
- Training set
- Testing set

### 4. Model Training
Multiple classification algorithms were used, such as:
- Logistic Regression
- Decision Tree
- Random Forest

### 5. Model Evaluation
The trained model was evaluated using:
- Confusion Matrix
- Classification Report
- Accuracy

## Flask Web Application

The project includes a Flask-based web application with:

- Input form for all required health features
- Backend connection to the trained ML model
- Prediction output displayed on the webpage

### User Flow
1. User enters health-related details in the form
2. Data is passed to the trained model
3. Model predicts heart disease risk
4. Result is displayed on the screen

## Project Structure

```bash
Heart-Disease-Prediction-System/
│
├── app.py
├── model.pkl
├── scaler.pkl
├── requirements.txt
├── data/
│   └── heart_disease.csv
├── templates/
│   ├── index.html
│   └── result.html
├── static/
│   └── style.css
└── README.md
```

## Requirements

```bash
pip install pandas numpy scikit-learn flask
```

## How to Run the Project

```bash
git clone <repository-link>
cd Heart-Disease-Prediction-System
pip install -r requirements.txt
python app.py
```

Then open your browser and go to:

```bash
http://127.0.0.1:5000/
```

## Notes

- The dataset contains missing values, so proper preprocessing is essential.
- Binary features were handled separately using mode-based imputation.
- Scaling was applied to numerical features for better model performance.
- The final model was deployed using Flask for interactive predictions.

## Future Improvements

- Add more advanced models
- Improve UI design
- Deploy on cloud platforms like Render or Heroku
- Add data visualization dashboards.
