# Customer Churn Prediction

A machine learning project to predict customer churn for a telecommunications company using various classification algorithms.

## Overview

This project analyzes customer data to predict whether a customer will churn (leave) the service or not. The model helps identify at-risk customers, allowing the company to take proactive measures to retain them.

## Dataset

The dataset contains customer information including:
- Demographics (gender, senior citizen status)
- Account information (tenure, contract type)
- Services subscribed (phone, internet, streaming services)
- Billing information (monthly charges, total charges)
- Churn status (target variable)

## Features

- Data preprocessing and feature engineering
- Handling imbalanced data using SMOTE
- Multiple machine learning models (selecting best out of the below):
  - Decision Tree
  - Random Forest
  - XGBoost
- Model evaluation using:
  - Cross-validation
  - Accuracy metrics
  - Confusion matrix
  - Classification report
- Probability-based predictions for better decision making

## Project Structure

```
Customer-Churn-Prediction-ML/
├── codes_and_models/
│   └── main.ipynb          # Main analysis and modeling notebook
    └── customer_churn_model.pkl  # Saved best performing model
    └── encoders.pkl
├── dataset/
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv  # Dataset file
└── README.md
```

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- xgboost
- matplotlib
- seaborn
- imbalanced-learn

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/Customer-Churn-Prediction-ML.git
cd Customer-Churn-Prediction-ML
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Open and run the Jupyter notebook:
```bash
jupyter notebook codes_and_models/main.ipynb
```

2. The notebook contains:
   - Data loading and preprocessing
   - Exploratory data analysis
   - Model training and evaluation
   - Prediction generation

## Model Performance

The project implements multiple models and evaluates them using:
- 10-fold stratified cross-validation
- Accuracy metrics
- Confusion matrix analysis
- Classification reports

## Future Improvements

- Implement deep learning models
- Add feature importance analysis
- Create a web interface for predictions
- Add real-time prediction API
- Implement automated model retraining

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Dataset source: [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- Thanks to the open-source community for the amazing tools and libraries
