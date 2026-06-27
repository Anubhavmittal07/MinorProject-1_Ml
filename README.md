# Real Estate Price Prediction

## Problem Statement

The goal of this project is to predict house prices in King County, USA using machine learning regression techniques based on features like 
size, location, condition, and grade of the house.

## Dataset

- **Name:** King County House Sales
- **Source:** Kaggle
- **Records:** 21,613
- **Features:** 21 columns including bedrooms, bathrooms, sqft_living, grade, condition, location, and price (target)

## Methodology

1. Dropped irrelevant columns (id, date)
2. Handled missing values using mean imputation
3. Removed outliers using IQR method
4. Split data into 80% training and 20% testing
5. Trained Linear Regression as baseline model
6. Applied Polynomial Features (degree=2) and trained Polynomial Regression
7. Evaluated both models using MSE and R2 Score

## Results

<img width="337" height="43" alt="image" src="https://github.com/user-attachments/assets/6043a018-ae3c-483b-a9b9-101c08764881" />
<img width="275" height="52" alt="image" src="https://github.com/user-attachments/assets/99b6b69b-c0d8-402f-b88c-b4e927847483" />


## Repository Structure

├── data/               - Dataset

├── notebook/           - Saved .pkl model files & Jupyter Notebook

├── results/            - Plots 

└── README.md

## Conclusion

This project demonstrates the use of machine learning regression techniques to predict house prices using the King County dataset. After preprocessing the data, removing outliers, and engineering polynomial features, two models were trained and evaluated.

Linear Regression served as the baseline model while Polynomial Regression (degree=2) improved the prediction accuracy by capturing non-linear relationships between features like sqft_living, grade, and location.

The results show that feature engineering plays an important role in improving model performance. With better algorithms like Random Forest or XGBoost and further feature selection, the accuracy can be improved even more.

Overall this project provided a good understanding of the end-to-end machine learning workflow including data cleaning, EDA, model training, evaluation, and saving trained models for future use.
