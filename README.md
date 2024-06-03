# AutoPricePro
A Cutting-Edge Solution for Car Price Prediction

## Introduction
This repository explores the implementation and optimization of machine learning models for predicting car prices. It covers various aspects including data preprocessing, feature engineering, and model training using RandomForestRegressor and LogisticRegression.

## Purpose
The main goals of this repository are to:
- Implement and optimize machine learning models for car price prediction.
- Understand and apply data preprocessing and feature engineering techniques.
- Experiment with different model architectures and hyperparameters.
- Manage computational constraints effectively during model training.

## Technical Summary

### Data Preprocessing
1. **Loading Data**: The dataset is loaded from a CSV file (`cars.csv`).
2. **Data Cleaning**: Dropped unnecessary columns, handled missing values by filling or dropping them, and transformed categorical variables into numerical formats.
3. **Feature Engineering**: Extracted new features from existing ones, such as splitting `mpg` into `mpg_lower` and `mpg_upper`, and standardizing numerical columns using `StandardScaler`.
4. **Outlier Removal**: Used Interquartile Range (IQR) method to remove outliers from the dataset.

### Models Implemented
- **RandomForestRegressor**: Used for predicting car prices.
- **LogisticRegression**: Applied for binary classification tasks (not shown in provided code but mentioned for completeness).

### Training Strategy
Due to limited computational resources, the following strategies were employed:
- **Model Simplification**: Adjusted the model complexity to fit within memory constraints.
- **Max Sequence Length Reduction**: Reduced the sequence length for efficient processing.
- **Batch Size Adjustment**: Used smaller batch sizes to manage memory usage.

### Performance and Evaluation
- **RandomForestRegressor**: Achieved a training score of ~0.991 and a testing score of ~0.935, indicating good model performance.
- **Evaluation Metrics**: Used R-squared score to evaluate the model's performance.

## Results
The repository includes:
- Trained models (`trainedModel.sav`).
- Scripts for data preprocessing, feature engineering, and model training.
- Example outputs demonstrating the model's performance.

## Conclusion
This repository demonstrates effective techniques for implementing and optimizing machine learning models for car price prediction. It highlights the challenges of managing computational constraints and provides solutions for efficient model training.
