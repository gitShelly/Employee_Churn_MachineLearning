# 👨‍💼 Employee Churn Prediction System

### ✨ Developed by: Avishi Gupta & Bhavya Goyal

---

## 📌 Project Description

This project is designed to predict whether an employee will **stay** or **leave** the company based on various personal and professional attributes.

It applies supervised machine learning techniques—**some implemented from scratch**—to classify employee attrition, and evaluates models using cross-validation to find the best-performing one.

---

## 🚀 How to Use This Project

Follow these steps to run and explore the project:

### ✅ Step 1: Access the Code
- Open the notebook in **Google Colab**, **Jupyter Notebook**, or any other Python environment that supports `.ipynb` files.
- You can **fork**, **download**, or **copy** the code.

### ✅ Step 2: Get the Dataset
- Download the dataset `employee.csv` used in this project or
- [🔗 Click here to download the dataset](https://www.opendatabay.com/data/ai-ml/2900e244-81c8-42a2-9cf6-1ded6626e49f?utm_source=chatgpt.com)

### ✅ Step 3: Run the Notebook
- Upload the dataset to your working directory.
- Execute all cells in sequence to load, preprocess, train, and evaluate the models.

### ✅ Step 4: Custom Testing
- Enter custom employee data to test the model's prediction on new or hypothetical cases.

---

## 🗂️ Dataset Overview

The dataset contains various features including:

- `Age`
- `Department`
- `DistanceFromHome`
- `EducationField`
- `EnvironmentSatisfaction`
- `HourlyRate`
- `JobSatisfaction`
- `MaritalStatus`
- `MonthlyIncome`
- `NumCompaniesWorked`
- `OverTime`
- `PercentSalaryHike`
- `PerformanceRating`
- `TotalWorkingYears`
- `TrainingTimesLastYear`
- `WorkLifeBalance`
- and others...

**Target Variable:**  
- `Attrition`: `1` = Employee will leave  
- `0` = Employee will stay

---

## ⚙️ Preprocessing Steps

- Feature Selection  
- Null Value Check  
- Categorical Encoding (LabelEncoder)  
- Feature Scaling (MinMaxScaler)  
- Outlier Detection using Box Plots  
- Correlation Analysis using Heatmap  

---

## 🧠 Machine Learning Models

The following models were implemented:

### ✅ Logistic Regression (from scratch)
- Implemented using NumPy
- Uses gradient descent for optimization

### ✅ Random Forest
- Based on multiple Decision Trees from `sklearn`
- Bootstrap sampling implemented

### ✅ K-Nearest Neighbors (from scratch)
- Uses Euclidean distance
- Predicts by majority vote among neighbors

### ✅ Gaussian Naive Bayes (from scratch)
- Assumes features follow a normal distribution
- Calculates posterior probabilities

---

## 🧪 Model Selection

Used **GridSearchCV** for:
- Hyperparameter tuning
- Cross-validation (5-fold)
- Model comparison

The model with the highest validation accuracy is selected as the final model.

---

## 🔍 Example Output

Predictions: [1] -> Employee will leave.
             [0] -> Employee will not leave.

## 📈 Visualizations

- Histograms (Feature Distribution)
- Heatmap (Correlation Matrix)
- Boxplot (Outlier Detection)

## 🛠️ Tech Stack & Libraries

- Python pandas, numpy matplotlib, seaborn , scikit-learn
- Manual implementation of ML algorithms

## 💡 Future Enhancements

- Add GUI with Streamlit or Flask for user-friendly input
- Handle class imbalance using SMOTE or similar techniques
- Deploy as a web application
- Add model explainability using SHAP or LIME
