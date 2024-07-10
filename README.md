## Comprehensive-Predictive-Modeling-of-Ames-House-Prices

## Dataset Introduction
The Ames Housing dataset, compiled by Dean De Cock in 2011 for educational purposes, encompasses comprehensive data on residential properties in Ames, Iowa. The dataset's primary goal is to predict housing prices, offering valuable insights into various factors that influence home values. These factors include neighborhood attributes, building materials, and property amenities, making the dataset a rich resource for industries such as real estate, property management, and urban planning.

## Exploratory Data Analysis (EDA)
EDA revealed that the target variable, ```SalePrice```, is right-skewed. Numerical features exhibited various degrees of correlation with the target variable, necessitating the consideration of multicollinearity and skewness in further analysis. Categorical features, visualized for cardinality, highlighted significant variations that could impact modeling.

## Data Preprocessing
Key preprocessing steps included outlier removal using the IQR method, handling missing values with suitable imputation techniques, and label encoding for categorical variables. The data was split into training and testing sets to prevent data leakage. Log transformation was applied to address skewness in the target variable, followed by feature selection using filter and wrapper methods to enhance model performance.

## Modeling
Several candidate models were evaluated:

•	Linear Regression: Exhibited strong fit but potential overfitting.
•	Ridge Regression: Balanced fit and generalization, mitigating multicollinearity.
•	Random Forest Regression: Captured complex interactions but with moderate accuracy.
•	LGBM Regressor: Efficient with high accuracy and minimal overfitting.
•	XGB Regressor: Strong fit but suffered from overfitting.
•	Neural Network: Handled intricate patterns, with potential for higher accuracy with more epochs.
•	Voting Regressor: Combined Ridge and LGBM for enhanced accuracy.

## Conclusion
Ridge and LGBM Regressor models were selected for their superior accuracy and generalization. These models provide reliable predictions for property pricing, aiding stakeholders in making informed decisions. Future work includes enhancing the interpretability of LGBM and optimizing Ridge's parameters to further stabilize and improve model performance across different datasets and scenarios.


