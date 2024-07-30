# Summary
This analysis aims to predict which customers will respond positively to an automobile insurance offer using a dataset derived from Health Insurance Cross Sell Prediction Data. Below is a concise summary of the findings and actions taken:

### Objective:
The goal is to classify whether a customer will respond positively to an automobile insurance offer based on various features.

### Dataset Overview:
  - Features:
    - Includes age, gender, vehicle age, vehicle damage status, driving license status, region code, previous insurance status, annual premium, policy sales channel, vintage, and response (target variable).
    
  - Key Statistics:
    - Approximately 88% of the customers did not opt for insurance, while only 12% did.
    - Among the 12% of subscribers, males have a higher subscription rate (61%) compared to females (38%).
      
### Data Cleaning:
  - **Encoding:** Applied binary encoding and one-hot encoding to convert categorical variables into numeric format.
  - Train-Test Split:
    - Train Size: X (8,628,598, 10), y (8,628,598)
    - Test Size: X (2,876,200, 10), y (2,876,200)

### Addressing Class Imbalance:
  - **Initial Class Distribution:** 88% class 0 (non-subscribers) and 12% class 1 (subscribers).
  - Methods Attempted:
    - **SMOTE and ADASYN:** Encountered memory errors.
    - **Undersampling:** Resulted in lower accuracy.
    - **Weighted Logistic Regression:** Achieved only 64% accuracy.
    - **Final Approach:** Reduced training data for class 0 by half and applied `SMOTE` oversampling to balance the classes.

### Model Building:
  - **Decision Tree Model:** Trained and evaluated using the balanced dataset.
  - Performance Metrics:
    - **Kaggle Competition:** Secured a public score of `0.83607`.
       - **Precision:** 0.94 (class 0), 0.47 (class 1)
       - **Recall:** 0.73 (class 0), 0.84 (class 1)
       - **Accuracy:** 75%
          
### Model Evaluation:
  - **AUC Score:** 0.7836, indicating a good balance between sensitivity and specificity.
  - **ROC Curve:** Demonstrates robust ability to differentiate between the two classes.

--- 

This concludes the analysis. The model shows good performance in terms of recall and overall accuracy, aligning with the business objective of predicting insurance cross-selling. Further enhancements can be made to balance precision and recall for improved utility in practical scenarios. The model is now ready for deployment based on the identified optimal threshold.
