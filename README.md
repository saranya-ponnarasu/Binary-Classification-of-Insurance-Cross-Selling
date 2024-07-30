# Predicting Insurance Cross-Selling

### Problem Statement:
The objective of this project is to predict which customers will respond positively to an automobile insurance offer. Using a dataset provided for the [2024 Kaggle Playground Series](https://www.kaggle.com/competitions/playground-series-s4e7), we will perform data cleaning and preliminary exploratory analysis to understand the features influencing customer responses. The aim is to develop a robust predictive model that accurately identifies potential customers for cross-selling insurance products.

### Libraries Used:
- **Numpy:** For data manipulation and handling missing values.
- **Pandas:** For data manipulation and cleaning.
- **Matplotlib:** For data visualization.
- **Seaborn:** For data visualization.
- **Scikit-learn:** For building and evaluating machine learning models.

### Steps Involved:
1. Importing the Libraries
2. Importing the Dataset
3. Data Understanding
    - Description of dataset features and their definitions.
4. Data Cleaning
5. Exploratory Data Analysis
6. Data Preparation for Modeling
  - 6.1. Binary encoding
    - 6.1.1. One-Hot Encoding
    - 6.1.2. Ordinal Encoding
  - 6.2. Splitting the Train and Test data: Splitting the data for training and testing purposes.
  - 6.3. Addressing Class Imbalance
      - 6.3.1. Undersampling
      - 6.3.2. SMOTE
7. Building the Decision Tree
   - 7.1. Decision Tree Visualization
   - 7.2. ROC Curve
8. Predicting on the Actual Test set
9. Submission
