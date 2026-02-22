 🚢 Titanic Survival Prediction – Data Analysis & Machine Learning

 📌 Project Overview

This project is based on the famous Titanic Dataset from Kaggle.  
The goal is to analyze passenger survival patterns and build a Machine Learning model to predict whether a passenger survived or not.

This project demonstrates:

- Data Cleaning & Preprocessing  
- Feature Engineering  
- Data Visualization  
- Missing Value Imputation  
- Random Forest Modeling  
- Model Evaluation using OOB Error  
- Feature Importance Analysis  

---

 📂 Dataset

Dataset used: Titanic – Machine Learning from Disaster  
Source: Kaggle Titanic Competition

The dataset contains passenger details such as:

- PassengerId  
- Pclass (Passenger Class)  
- Name  
- Sex  
- Age  
- SibSp (Siblings/Spouses aboard)  
- Parch (Parents/Children aboard)  
- Ticket  
- Fare  
- Cabin  
- Embarked  
- Survived (Target Variable)

---

 🛠️ Technologies & Libraries Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Missingno  
- Statsmodels  
- Scikit-learn  

---

 🔎 Project Workflow

 1️⃣ Data Loading
- Loaded `train.csv` and `test.csv`
- Combined datasets for feature engineering

 2️⃣ Data Cleaning

- Filled missing Embarked values using fare analysis
- Filled missing Fare using group median (Pclass + Embarked)
- Imputed missing Age using Random Forest Regressor

 3️⃣ Feature Engineering

Created powerful features:

- Title (Extracted from Name)
- Surname
- Family Size (Fsize)
- Family Category (Singleton / Small / Large)
- Child (Age < 18)
- Mother (Female + Parch > 0 + Age > 18 + Not Miss)

These engineered features significantly improved model performance.

4️⃣ Data Visualization

Created visualizations to analyze survival patterns:

- Survival by Gender (Bar Chart)
- Survival by Passenger Class
- Age Distribution Histogram
- Family Size vs Survival (Bar & Mosaic Plot)
- Fare Distribution by Embarked Port
- Age Distribution by Sex & Survival

---

 🤖 Machine Learning Model

 Model Used:
Random Forest Classifier

 Why Random Forest?

- Handles non-linear relationships
- Works well with categorical + numerical features
- Provides Feature Importance
- Robust to overfitting

 Model Evaluation:

- Used Out-of-Bag (OOB) Error
- Trained model incrementally up to 500 trees
- Plotted OOB Error vs Number of Trees

---

 📊 Feature Importance

Top Important Features:

1. Age  
2. Fare  
3. Sex  
4. Title  
5. Pclass  

This confirms:

- Women had higher survival rates  
- Younger passengers had better survival chances  
- Social class strongly influenced survival  

---

 📁 Final Output

Generated prediction file:

`rf_mod_solution_python.csv`

Contains:
- PassengerId  
- Predicted Survival (0 or 1)

---

 📈 Key Insights

- Females survived more than males  
- 1st class passengers had higher survival rates  
- Small families (2–4 members) had better survival chances  
- Large families and single travelers had lower survival rates  
- Titles (Mr, Mrs, Miss, Master) were strong survival indicators  

---

 🎯 What I Learned

- Real-world data cleaning techniques  
- Advanced Feature Engineering  
- Predictive Imputation using Random Forest  
- Model evaluation using OOB error  
- Importance of visualization in Data Science  
- End-to-end ML pipeline development  


 🚀 How to Run

1. Clone this repository  
2. Install required libraries:

   pip install pandas numpy matplotlib seaborn missingno statsmodels scikit-learn

3. Place `train.csv` and `test.csv` in the project directory  
4. Run the notebook or Python script  

