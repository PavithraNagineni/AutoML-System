# AutoML Pipeline

Run:
1. python src/train.py --data data/sample.csv --trials 20
2. uvicorn src.serve:app --reload


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
Component	----> Technology
Preprocessing	----> Pandas, Scikit-learn
Models	----> RandomForest, XGBoost, SVM, Logistic Regression
AutoML Search	----> GridSearchCV / Optuna
Experiment Tracking ---->	MLflow
Deployment ---->	FastAPI + Uvicorn
Packaging ---->	Docker



🏗 High-Level Architecture
Raw Data → Preprocessing → Model Training → Hyperparameter Tuning → 
Model Comparison → Best Model → MLflow Logging → API Deployment

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



