## Diabetes Prediction using Support Vector Machine (SVM)

This project demonstrates how to use a Support Vector Machine (SVM) classifier to predict the likelihood of a person having diabetes based on various medical features. The goal is to classify individuals as either diabetic (1) or non-diabetic (0) based on their medical data.

### Project Overview

In this project, we use a diabetes dataset that includes various medical measurements such as glucose levels, BMI, age, and blood pressure to predict whether an individual has diabetes. We preprocess the data, standardize it, and apply an SVM classifier to predict the outcome. The performance of the classifier is then evaluated using accuracy metrics on both the training and testing data.

### Steps Involved:

1. **Data Exploration**:
   - The dataset is loaded and explored. Basic information such as shape, summary statistics, and the distribution of the target variable (`Outcome`) is checked.
   - We analyze the dataset to identify any potential imbalances between classes (diabetic vs non-diabetic).

2. **Feature Selection**:
   - The target variable (`Outcome`) is separated from the features. The features (`X`) include all the columns except for `Outcome`, and the target variable (`Y`) is the `Outcome` column.

3. **Data Standardization**:
   - The features are standardized using `StandardScaler` to normalize the data, ensuring that all features have the same scale. This is important for algorithms like SVM, which are sensitive to the scale of the data.

4. **Splitting the Data**:
   - The dataset is split into training and testing sets using `train_test_split`. Stratified sampling is applied to ensure that the distribution of diabetic and non-diabetic individuals is preserved in both the training and testing sets.

5. **Modeling with SVM**:
   - A Support Vector Machine classifier with a linear kernel is instantiated and trained on the training data. 
   - The model is then used to predict the target variable (`Outcome`) on both the training and testing datasets.

6. **Model Evaluation**:
   - The accuracy of the model is evaluated by comparing the predicted values with the actual values in both the training and testing sets.

