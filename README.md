# Weather Prediction using SVM - 83% Accuracy

## Project Overview
This project implements a Support Vector Machine (SVM) model to predict weather conditions using historical data from Seattle. The model achieves 83% accuracy in classifying different weather types.

## Features
- Data preprocessing and cleaning
- Feature engineering with temporal data
- Multiple SVM kernel comparisons (Linear, RBF, Polynomial, Sigmoid)
- Hyperparameter tuning using GridSearchCV
- Model evaluation and visualization

## Dataset
The dataset contains 1,461 daily weather records with features:
- Precipitation amount
- Maximum and minimum temperature  
- Wind speed
- Weather condition (target variable)

Weather conditions include: rain, drizzle, sun, fog, and snow.

## Model Performance
After testing different SVM kernels, the linear kernel performed best:

**Linear Kernel Results:**
- Best parameters: {'C': 50, 'kernel': 'linear'}
- Cross-validation accuracy: 85.28%
- Test accuracy: 83.28%

Other kernels showed slightly lower performance, with polynomial at 82.94%, RBF at 82.25%, and sigmoid at 75.43%.

## Key Features
- Cyclical encoding of day-of-year using sine/cosine transformations
- Standard scaling for feature normalization
- Comprehensive model comparison
- Performance visualization

## Requirements
- Python 3.11+
- pandas, numpy, scikit-learn, matplotlib

## Usage
Run the Jupyter notebook `weather-prediction-svm-83-accuracy.ipynb` to:
1. Load and explore the data
2. Preprocess features
3. Train and evaluate SVM models
4. View performance results

The project demonstrates effective use of SVM for multi-class weather prediction with strong results across different weather conditions.
