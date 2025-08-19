EV Market Analysis — Final Insights & Modeling
Project Overview

This project analyzes the electric vehicle (EV) specifications dataset (electric_vehicles_spec_2025.csv). It consolidates data preprocessing, exploratory data analysis (EDA), feature engineering, regression, classification, clustering, and association rule mining as part of Deliverable 4.

The goal is to:

Explore EV specifications and relationships between performance features.

Predict vehicle range using regression models.

Classify vehicles by body type.

Segment the market into clusters using KMeans.

Discover associations between categorical and binned numerical features.

 Requirements

Install dependencies before running the script:

pip install pandas numpy matplotlib scikit-learn mlxtend

 Dataset

File: electric_vehicles_spec_2025.csv

Place the dataset in the same directory as the script before execution.

 Running the Code

Run the Python script:

python tushar_jitendrakumar_limbachiya.py


The script will:

Preprocess & clean the dataset.

Perform EDA (scatter plots, correlation heatmap).

Run regression models (Random Forest, SVR) to predict range_km.

Train classification models for car_body_type.

Perform clustering with KMeans.

Apply association rule mining using Apriori.

Save results (cluster summary & rules) in the artifacts/ folder.

Key Methods & Models
🔹 Regression

Random Forest Regressor (GridSearchCV tuned)

Support Vector Regressor (SVR baseline)

Metrics: R², RMSE, MAE

🔹 Classification

Random Forest Classifier

Support Vector Classifier (SVC)

Metrics: Accuracy, Confusion Matrix, Classification Report

🔹 Clustering

KMeans Segmentation

Used Elbow Method to find optimal k

Segmented market into ~4 groups (compact EVs, performance EVs, SUVs, luxury EVs)

🔹 Association Rule Mining

Binned numerical features (battery, range, acceleration, speed, cargo volume)

Extracted rules using Apriori

Evaluated rules by confidence and lift
