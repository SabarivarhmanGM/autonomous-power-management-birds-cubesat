# Autonomous CubeSat Power Management System

Machine learning based CubeSat telemetry analytics platform for solar power prediction, power state classification, and eclipse detection using real on-orbit Electrical Power System (EPS) telemetry data from the TSURU CubeSat mission.

---

## Project Overview

Power management is one of the most critical subsystems in small satellites. CubeSats operate under strict power constraints due to limited battery capacity and varying solar energy availability during orbital operations.

This project investigates the application of machine learning techniques for autonomous power management by analyzing real on-orbit telemetry from the TSURU CubeSat. The system focuses on predicting solar power generation, identifying operational power states, and detecting eclipse conditions to support intelligent onboard decision-making.

---

## Objectives

* Predict solar power generation using regression models.
* Classify operational power states using machine learning classifiers.
* Detect eclipse conditions from onboard telemetry data.
* Compare the performance of multiple regression and classification algorithms.
* Analyze feature importance and power system behavior using real satellite telemetry.

---

## Dataset

This project uses the **TSURU CubeSat telemetry dataset** from the BIRDS CubeSat constellation Electrical Power System (EPS) dataset.

### Dataset Citation

Jara, A., & Lepcha, P. (2022).

*On-orbit Electrical Power System Dataset of 1U CubeSat constellation for Machine Learning Models.*

Mendeley Data, Version 1.

DOI: https://doi.org/10.17632/8kp25ycf63.1

### Dataset Information

* Satellite Used: TSURU
* Mission Family: BIRDS CubeSat Constellation
* Institution: Kyushu Institute of Technology (Kyutech)
* Orbit: Low Earth Orbit (~400 km altitude)
* Data Source: TSURU.xlsx
* Data Type: Electrical Power System (EPS) Telemetry

### Telemetry Parameters

* Solar Panel Voltage
* Solar Panel Current
* Solar Panel Temperature
* Battery Voltage
* Battery Current
* Battery Temperature

### License

The original dataset is distributed under the Creative Commons Attribution 4.0 International (CC BY 4.0) License.

The dataset itself is not redistributed in this repository. Users wishing to reproduce the experiments should obtain the dataset directly from the original source.

---

## Methodology

### 1. Exploratory Data Analysis (EDA)

* Dataset inspection
* Statistical analysis
* Missing value analysis
* Correlation analysis
* Telemetry trend visualization

### 2. Data Preparation

* Data cleaning
* Feature engineering
* Feature selection
* Target generation
* Dataset splitting

### 3. Regression Modeling

Solar power prediction was performed using multiple regression algorithms.

#### Models Evaluated

* Linear Regression
* Multiple Linear Regression
* Polynomial Regression
* Ridge Regression
* Lasso Regression
* ElasticNet Regression
* K-Nearest Neighbors Regressor
* Decision Tree Regressor
* Random Forest Regressor
* AdaBoost Regressor
* Gradient Boosting Regressor
* Support Vector Regressor (SVR)

### 4. Classification Modeling

Classification models were developed for eclipse and power state prediction.

#### Models Evaluated

* Logistic Regression
* K-Nearest Neighbors (KNN)
* Support Vector Machine (SVM)
* Decision Tree Classifier
* Random Forest Classifier
* AdaBoost Classifier
* Gradient Boosting Classifier
* Naïve Bayes Classifier
* Multi-Layer Perceptron (MLP) Neural Network

### 5. Model Evaluation

Regression Metrics:

* R² Score
* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)

Classification Metrics:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

---

## Repository Structure

```text
autonomous-power-management-birds-cubesat/

├── Dataset Preparation and Analysis/
│   ├── EDA.ipynb
│   └── TSURU_Data_Preparation.ipynb
│
├── TSURU - Regressor/
│   ├── Linear_Regression.ipynb
│   ├── RandomForest_Regressor.ipynb
│   ├── Gradient_Boosting_Regressor.ipynb
│   └── ...
│
├── TSURU - Classifier/
│   ├── Logistic_Regression_Classifier.ipynb
│   ├── Random_Forest_Classifier.ipynb
│   ├── Neural_Network_MLP_Classifier.ipynb
│   └── ...
│
└── Results and Analysis/
    ├── Regression Results
    ├── Classification Results
    ├── Feature Importance
    ├── Correlation Analysis
    └── Performance Visualizations
```

---

## Key Outputs

* Solar power prediction models
* Eclipse state prediction models
* Power state classification models
* Feature importance analysis
* Correlation studies
* Comparative model benchmarking
* Mission telemetry visualizations

---

## Applications

* Autonomous satellite power management
* CubeSat mission planning
* Onboard decision support systems
* Fault detection and diagnosis
* Telemetry analytics
* Spacecraft health monitoring

---

## Future Work

* Real-time onboard machine learning inference
* Power demand forecasting
* Satellite anomaly detection
* Reinforcement learning based power scheduling
* Edge AI deployment on CubeSat flight computers
* Multi-satellite telemetry learning frameworks

---

## Acknowledgements

The telemetry dataset used in this work was provided by the BIRDS Program and the Kyushu Institute of Technology (Kyutech). The authors of the original dataset are Adolfo Jara and Pooja Lepcha.

---

## Author

Sabarivarhman G M

Computer Science and Electrical Engineering

Amrita Vishwa Vidyapeetham
