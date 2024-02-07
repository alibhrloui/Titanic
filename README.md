# Titanic Survival Prediction

This repository contains a simple Python script for predicting survival on the Titanic using a Random Forest Classifier. The dataset is obtained from Kaggle's Titanic competition.

## Prerequisites

Make sure you have the required libraries installed. You can install them using:

```bash
pip install pandas scikit-learn
```

## Dataset

The training and testing datasets (`train.csv` and `test.csv`) are used for this prediction task. The data includes features such as Pclass, Sex, SibSp, Parch, etc.

## Code Overview

1. **Data Loading:**
   - The script starts by loading the training and testing datasets.

2. **Feature Extraction:**
   - The target variable "Survived" is extracted from the training dataset.
   - Features are defined, including Pclass, Sex, SibSp, and Parch.

3. **Parameter Grid for GridSearchCV:**
   - A parameter grid is defined for hyperparameter tuning using GridSearchCV.

4. **Data Preprocessing:**
   - Dummy variables are created for categorical features using one-hot encoding.

5. **Random Forest Model Initialization:**
   - A Random Forest model is initialized.

6. **GridSearchCV for Hyperparameter Tuning:**
   - GridSearchCV is employed to find the best hyperparameters for the Random Forest model.

7. **Training the Model:**
   - The model is trained using the training data.

8. **Making Predictions:**
   - Predictions are made on the test set using the best model obtained from GridSearchCV.

9. **Submission:**
   - The predictions are saved to a CSV file (`submission.csv`) for submission to Kaggle.

10. **Training Accuracy (Optional):**
    - Training accuracy is calculated for illustration purposes.

## How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/titanic-survival-prediction.git
   ```

2. Navigate to the project directory:

   ```bash
   cd titanic-survival-prediction
   ```

3. Run the script:

   ```bash
   python titanic_prediction.py
   ```

## Kaggle Submission

The script generates a submission file (`submission.csv`) that can be submitted to Kaggle for evaluation.

## Note

- The training accuracy is calculated for illustration purposes and is typically not done in practice.

- Feel free to modify the features, hyperparameters, or other aspects of the script for experimentation.

