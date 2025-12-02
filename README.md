# AutoML-System
🚀 Mini Project: Intelligent AutoML Pipeline for Model Training &amp; Deployment

📌 Project Title
AutoML System: Automated ML Model Training, Selection & Deployment Pipeline


📘 Problem Statement
   Build a system that automatically:

  1️⃣ Cleans and preprocesses any tabular dataset
  2️⃣ Trains multiple ML models
  3️⃣ Performs hyperparameter tuning
  4️⃣ Selects the best model based on metrics
  5️⃣ Logs everything into MLflow
  6️⃣ Deploys the chosen model using FastAPI


🧠 Tech Stack
  Component	  -------> Technology
  Preprocessing ---->	Pandas, Scikit-learn
  Models	----> RandomForest, XGBoost, SVM, Logistic Regression
  AutoML ----> Search	GridSearchCV / Optuna
  Experiment Tracking	----> MLflow
  Deployment	----> FastAPI + Uvicorn
  Packaging	----> Docker

  

⭐ Features
🔹 1. Automated Data Pipeline

  Load & clean CSV files
  
  Handle missing values
  
  Encode categorical features
  
  Scale numerical features
  
  Train/validation/test split

🔹 2. Automated Model Training

   The system trains multiple ML models:

   Random Forest

   XGBoost

   Logistic Regression

   Support Vector Machine

   Each model is wrapped into a single unified training pipeline.

🔹 3. AutoML + Hyperparameter Tuning

   Uses Optuna to automatically search and identify the best hyperparameters.

🔹 4. Automatic Model Selection

   The model with the best F1-score is selected as the final model.

🔹 5. MLflow Experiment Tracking

   Model versioning
  
   Metrics logging
  
   Parameter logging
  
   Model Registry support

🔹 6. FastAPI Prediction Server

   A REST API to make predictions using the best trained pipeline.

🔹 7. Docker Support

   Deploy the API easily in any environment using Docker.

   

📁 Project Structure
automl-pipeline/
├─ data/
│  └─ sample.csv
├─ src/
│  ├─ config.py
│  ├─ data_processing.py
│  ├─ features.py
│  ├─ models.py
│  ├─ train.py
│  ├─ mlflow_utils.py
│  └─ serve.py
├─ models/
├─ requirements.txt
├─ Dockerfile
├─ README.md
└─ .gitignore

