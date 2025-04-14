# Machine Learning Prediction App

This is an interactive machine learning web application built with Streamlit that allows users to upload their own datasets, visualize relationships, train a predictive model, and make real-time predictions.

Live App: https://khalid-machine-learning.streamlit.app/

## Features

- Upload any CSV dataset and select a target variable
- Visualize:
  - Average target value across categorical variables
  - Correlation of numerical features
- Train a model by selecting your own features
- Make live predictions by entering new data
- Supports flexible datasets and automatic preprocessing

## Machine Learning Capabilities

- Random Forest Regression model used as the core predictor
- Engineered pipeline includes:
  - Data preprocessing via `ColumnTransformer`
  - Imputation for missing data
  - One-hot encoding for categorical variables
- Performance Optimization:
  - Model tuned using Grid Search with Cross-Validation
  - Evaluation using R² score and RMSE
- Model Comparison (Behind the Scenes):
  - Benchmarked against Decision Tree and K-Nearest Neighbors (KNN) models
  - Chose Random Forest for superior performance on most datasets

## Tech Stack

- Frontend/UI: Streamlit
- Data Processing & ML: Pandas, NumPy, scikit-learn
- Visualization: Seaborn, Matplotlib

## Files in This Repository

- `machine_learning.py` – Main Streamlit application
- `requirements.txt` – Required packages for deployment
- `.gitignore` – Files and directories excluded from version control
- `README.md` – Project overview and documentation
