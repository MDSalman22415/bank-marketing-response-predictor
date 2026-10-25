# Bank Marketing Response Prediction using ANN

## Project Overview

This project focuses on predicting whether a bank customer will subscribe to a term deposit based on customer information and marketing campaign data.

The project follows a machine learning workflow, including Exploratory Data Analysis (EDA), data preprocessing, feature engineering, feature transformation, feature scaling, and Artificial Neural Network (ANN) model development.

The main objective is to understand customer behavior and build a neural network classification model that predicts the likelihood of term-deposit subscription.

## Problem Statement

Banks conduct marketing campaigns to encourage customers to subscribe to term deposits. Contacting every customer without understanding their likelihood of subscribing can lead to inefficient use of resources.

This project uses historical marketing campaign data to develop an ANN classification model that predicts whether a customer is likely to subscribe to a term deposit.

## Dataset Description

The project uses the Bank Marketing dataset, which contains customer demographics, financial information, contact details, and previous marketing campaign outcomes.

Important features include:

- `age` — Customer age
- `job` — Type of occupation
- `marital` — Marital status
- `education` — Education level
- `default` — Credit default status
- `balance` — Account balance
- `housing` — Housing loan status
- `loan` — Personal loan status
- `contact` — Contact communication type
- `day` and `month` — Date of the last contact
- `duration` — Duration of the last contact
- `campaign` — Number of contacts during the current campaign
- `pdays` — Days since the previous contact
- `previous` — Number of previous contacts
- `poutcome` — Outcome of the previous campaign
- `Target` — Whether the customer subscribed to a term deposit

The original target variable `y` was represented as `Target` during data preparation.

## Project Workflow

### 1. Data Understanding

- Inspected dataset dimensions, column names, data types, and statistical summaries.
- Studied the meaning of customer and marketing campaign features.
- Identified the target variable and formulated the classification problem.

### 2. Exploratory Data Analysis (EDA)

- Analyzed numerical and categorical features.
- Examined distributions and relationships between features and the target.
- Investigated correlations between numerical variables.
- Studied customer groups and their subscription patterns.
- Examined the relationship between contact duration and subscription outcomes.

### 3. Data Preprocessing

- Prepared the dataset for model training.
- Converted categorical information into numerical representations.
- Checked feature data types and prepared model input features.
- Separated input features from the target variable.

### 4. Feature Engineering and Transformation

- Transformed categorical variables into machine-readable features.
- Applied categorical encoding and feature transformation.
- Prepared numerical and categorical features for ANN training.
- Examined feature relationships and multicollinearity using correlation and Variance Inflation Factor (VIF) analysis.

### 5. Feature Scaling

- Applied `StandardScaler` to scale numerical model inputs.
- Prepared features for neural network training.

### 6. ANN Model Development

- Developed an Artificial Neural Network using TensorFlow/Keras.
- Configured the model for binary classification.
- Trained the network using the prepared dataset.
- Saved the trained model as `model.h5`.

## Technologies Used

- **Programming Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Feature Processing:** Scikit-learn
- **Deep Learning:** TensorFlow, Keras
- **Model Format:** HDF5 (`.h5`)
- **Development Environment:** Jupyter Notebook

## Current Project Status

**Completed:**
- Exploratory Data Analysis (EDA)
- Data preprocessing
- Feature engineering and transformation
- Feature scaling
- ANN model training
- Saving the trained model as `model.h5`

**Not implemented yet:**
- Streamlit web interface
- End-user prediction webpage
- Complete reusable preprocessing artifact pipeline for inference

The current repository contains the model development workflow. A web application has not yet been completed.

## Key Learnings

- Understanding and analyzing real-world banking data.
- Performing EDA to identify meaningful patterns.
- Preparing categorical and numerical features for ANN models.
- Applying feature scaling during model development.
- Building and training an ANN classification model.
- Understanding the importance of saving preprocessing objects and maintaining consistent feature order between training and inference.

## Future Improvements

- Save the complete preprocessing pipeline and fitted transformation objects.
- Build a Streamlit interface for interactive predictions.
- Integrate preprocessing and model inference into a reusable pipeline.
- Add classification evaluation metrics and visualizations.
- Improve reproducibility through modular code and automated tests.

## Conclusion

This project provided hands-on experience with the end-to-end development of an ANN classification model using banking marketing data. It covers data exploration, feature engineering, preprocessing, scaling, and model training.

The next stage is to develop a web interface and integrate the model with a reproducible preprocessing pipeline.

---

**Author:** MD Salman  
**Project:** Bank Marketing Response Prediction using ANN  
**Task:** Binary Classification  
**Model:** Artificial Neural Network (ANN)  
**Status:** Model Development Completed; Web Interface Pending
