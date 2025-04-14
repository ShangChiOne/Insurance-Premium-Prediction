Insurance Charges Prediction with Random Forest

This project demonstrates a complete machine learning pipeline in Python to predict insurance charges using demographic and health-related features. Built and executed in Google Colab, it explores data preprocessing, feature engineering, model training, evaluation, and hyperparameter tuning using a Random Forest Regressor.

📁 Dataset

File: insurance.csv

Source: Typically from Kaggle or similar repositories

Features:

age: Age of primary beneficiary

sex: Gender (male/female)

bmi: Body mass index

children: Number of children covered by health insurance

smoker: Smoking status (yes/no)

region: Residential region (northeast, southeast, etc.)

charges: Individual medical costs billed by health insurance

🚀 Workflow

1. Data Loading & Inspection

Uploads the dataset via Google Colab's files.upload()

Basic statistics using value_counts() and .info()

2. Data Preprocessing

Converts sex and smoker columns to binary

One-hot encodes the region column

Drops the original region column post-encoding

3. Exploratory Data Analysis

Histograms for feature distribution

Correlation heatmap to understand feature relationships

4. Model Training

Splits data into training and test sets

Trains a RandomForestRegressor

Evaluates using score(), RMSE, MAE

5. Visualization

Scatter plot of predicted vs actual charges

Feature importance bar plot

6. Hyperparameter Tuning

Uses GridSearchCV for tuning hyperparameters

Re-evaluates with optimized model

🧪 Requirements

This project runs in Google Colab with the following libraries:

pandas
numpy
matplotlib
seaborn
scikit-learn
google.colab

📊 Results

Initial Model: Evaluated with RMSE and MAE

Tuned Model: Improved performance with GridSearchCV

📷 Visuals

Correlation heatmap of features

Predicted vs Actual charges scatter plot

Feature importance bar chart

📌 How to Run

Open the notebook in Google Colab

Upload the insurance.csv file

Run each cell in sequence to follow the analysis and modeling

🧠 Future Improvements

Try other models (e.g., XGBoost, Linear Regression)

Explore deeper EDA (outliers, distributions)

Automate pipeline with Pipeline or sklearn.compose

Add cross-validation scores and model comparison
