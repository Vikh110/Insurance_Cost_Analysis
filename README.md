# Insurance Cost Prediction

This project involves the analysis and prediction of insurance costs using various regression techniques. Through Exploratory Data Analysis (EDA), correlation, and model development (including Ridge Regression and Polynomial Regression), the aim is to identify the most influential factors affecting insurance costs and develop accurate predictive models.

## Project Overview

The project is divided into several stages:

### 1. Exploratory Data Analysis (EDA)
- **Correlation Matrix**: This highlights the relationships between various features such as age, BMI, smoker status, and insurance charges. Features with a high positive or negative correlation with insurance costs are critical for model building.
- **Boxplot**: Visualizes the distribution of insurance charges across different categories (e.g., smoker status, region, gender) and identifies outliers. It shows that smokers have significantly higher insurance charges compared to non-smokers.
- **Regression Plot**: Displays the linear relationship between BMI and insurance costs. This helps visualize the strength of the correlation and the linear trends in the data.

### 2. Model Development
- **Ridge Regression**: An initial model using Ridge regression was trained with a regularization parameter to control for overfitting. The model achieved an \(R^2\) score of 0.676, explaining 67.6% of the variance in insurance costs. This indicates that there may be non-linear relationships between features and insurance costs.
  
### 3. Model Refinement
- **Polynomial Features (Degree = 2)**: By incorporating polynomial features, the model performance improved significantly, achieving an \(R^2\) score of 0.784. This indicates that non-linear relationships are important to accurately capture the variance in the data and predict insurance costs.

### 4. Key Findings
- **Feature Importance**: Through correlation analysis, the most influential features identified are:
  - **Smoker Status**: Being a smoker has the highest impact on insurance costs.
  - **BMI**: Higher BMI values are strongly correlated with increased insurance costs.
  - **Age**: Older individuals tend to have higher insurance costs.
 
### 1. Regression Plot (BMI vs. Charges)

- **Relationship**: The scatterplot shows a weak positive linear relationship between BMI and insurance charges. The red regression line indicates that as BMI increases, insurance charges tend to increase slightly.
- **Spread**: There is significant variance in insurance charges for individuals with similar BMI values, especially for higher BMIs. This indicates that BMI alone may not fully explain variations in insurance charges.

### 2. Boxplot (Smoker Status vs. Charges)

- **Smoker vs Non-Smoker**: The boxplot clearly shows that smokers have higher insurance charges compared to non-smokers.
  - **Non-Smokers**: Have a lower median insurance charge, with a more compact range of costs, though there are some outliers.
  - **Smokers**: Have a broader range of insurance charges, with significantly higher median charges, indicating that smoking is a major factor influencing insurance costs.
  
- **Conclusion**: Smoking status is a critical predictor of higher insurance costs.

  
- **Non-linear Relationships**: Polynomial regression shows that non-linear relationships between features like BMI and age with insurance costs are essential for improving model performance.

## Technologies Used
- **Python**: For data preprocessing, analysis, and model building.
- **Libraries**:
  - `pandas` for data handling.
  - `seaborn` and `matplotlib` for data visualization.
  - `scikit-learn` for model development and evaluation.

## Results
- **Ridge Regression**: \(R^2\) score of 0.676.
- **Polynomial Regression (Degree=2)**: \(R^2\) score of 0.750, showing improved predictive performance by capturing non-linear relationships.

