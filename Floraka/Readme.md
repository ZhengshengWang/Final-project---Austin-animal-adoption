# Austin Animal Center Outcomes Analysis

## Overview
This project focuses on analyzing and predicting animal outcomes at the Austin Animal Center using historical data and machine learning models. The primary goal is to derive actionable insights to improve decision-making and operations at the shelter.

## Objectives
- Analyze and clean the Austin Animal Center Outcomes dataset.
- Identify significant predictors of animal outcomes.
- Train and optimize machine learning models to achieve high predictive accuracy.
- Provide insights into feature importance and model performance.

## Dataset
The dataset contains historical records of animals and their outcomes at the shelter. Key columns include:
- **Outcome Type**: The target variable representing the outcome for each animal (e.g., adoption, transfer).
- **Animal Type**, **Breed**, **Age upon Outcome**, and **Sex upon Outcome**: Features used for prediction.

## Methodology
### 1. Data Cleaning
- Removed irrelevant columns: `Name`, `Animal ID`, and `Outcome Subtype`.
- Handled missing values by dropping rows with significant missing data.
- Encoded categorical variables using `LabelEncoder`.

### 2. Data Preprocessing
- Standardized numerical features using `StandardScaler`.
- Split the dataset into training (80%) and testing (20%) sets.

### 3. Model Training
- Used a baseline **Random Forest Classifier** for initial model training.
- Evaluated the model with a confusion matrix and classification metrics.

### 4. Hyperparameter Optimization
- Performed hyperparameter tuning using **RandomizedSearchCV** for efficiency.
- Evaluated the optimized model to achieve improved accuracy.

### 5. Feature Importance Analysis
- Identified key predictors of animal outcomes based on feature importance scores.

## Results
- **Initial Model Accuracy**: ~72%.
- **Optimized Model Accuracy**: ~75%.
- Key predictors include `Breed`, `Animal Type`, `Sex upon Outcome`, and `Age upon Outcome`.

## Visualizations
- **Confusion Matrix**: Displays model performance across different outcome categories.
- **Feature Importance Graph**: Highlights the most influential predictors of animal outcomes.

## Conclusion
- The optimized Random Forest model improved accuracy to ~75%, providing better predictive insights.
- Feature importance analysis highlighted critical predictors for decision-making.

## Next Steps
1. Explore additional features such as geolocation or shelter-specific data.
2. Implement advanced machine learning models like Gradient Boosting or XGBoost.
3. Enhance interpretability and visualization for better stakeholder engagement.

## How to Run
1. Install required Python libraries: `pandas`, `numpy`, `scikit-learn`, `seaborn`, `matplotlib`.
2. Run the script to preprocess data, train the model, and visualize results.
3. Use the included `optimization_results.csv` file to explore hyperparameter tuning outcomes.

## Acknowledgements
- Dataset: Austin Animal Center Outcomes Dataset.
- Tools: Python, Scikit-learn, Matplotlib, Seaborn.
