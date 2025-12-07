# IDS 2025 Project - Hotel Reservations

### Authors
- Jan Erik Jakstein
- Mattias Rahnu

### [Kaggle Dataset](https://www.kaggle.com/datasets/ahsan81/hotel-reservations-classification-dataset)
### [Project Report](https://github.com/Jantz/ids-2025-hotel_reservations/blob/main/E7_report.pdf)

## Introduction
This project focuses on Exploratory Data Analysis (EDA) and classification of hotel reservation cancellations. The goal is to predict whether a customer will cancel their booking based on various features.

The project aims to provide insights into the factors that influence hotel reservation cancellations. 

## Dataset
- **File**: `Hotel Reservations.csv`
- **Shape**: 36,275 rows, 19 columns

### Key Features
- `lead_time`: Number of days between booking and arrival.
- `no_of_special_requests`: Total number of special requests made by the customer.
- `market_segment_type`: Market segment designation (e.g., Online, Offline).
- `avg_price_per_room`: Average price per day of the reservation.

## Technologies Used
- **Python**
- **Pandas**, **NumPy**
- **Matplotlib**, **Plotnine**
- **Scikit-learn**
- **XGBoost**

## Models & Analysis
The following machine learning models were implemented and evaluated:
1.  **Logistic Regression**
2.  **Random Forest Classifier**
3.  **XGBoost Classifier**
4.  **Lasso Regression**

### Key Findings
- **Feature Importance**: `lead_time`, `no_of_special_requests`, `avg_price_per_room` and `market_segment_type` were identified as significant predictors of cancellation.
- **Financial Impact**: The models were evaluated on their ability to mitigate revenue loss from cancellations. Random Forest and XGBoost performed best, mitigating approximately **65%** of potential revenue loss.

## How to Run
1.  Install the required libraries:
    ```
    pip install pandas numpy matplotlib plotnine scikit-learn xgboost
    ```
2.  Place `Hotel Reservations.csv` in the project directory.
3.  Open and run `project.ipynb` in Jupyter Notebook.
