Titanic Survival Prediction
This repository contains a simple Python script for predicting survival on the Titanic using a Random Forest Classifier. The dataset is obtained from Kaggle's Titanic competition.

Prerequisites
Make sure you have the required libraries installed. You can install them using:

bash
Copy code
pip install pandas scikit-learn
Dataset
The training and testing datasets (train.csv and test.csv) are used for this prediction task. The data includes features such as Pclass, Sex, SibSp, Parch, etc.

Code Overview
Data Loading:

The script starts by loading the training and testing datasets.
Feature Extraction:

The target variable "Survived" is extracted from the training dataset.
Features are defined, including Pclass, Sex, SibSp, and Parch.
Parameter Grid for GridSearchCV:

A parameter grid is defined for hyperparameter tuning using GridSearchCV.
Data Preprocessing:

Dummy variables are created for categorical features using one-hot encoding.
Random Forest Model Initialization:

A Random Forest model is initialized.
GridSearchCV for Hyperparameter Tuning:

GridSearchCV is employed to find the best hyperparameters for the Random Forest model.
Training the Model:

The model is trained using the training data.
Making Predictions:

Predictions are made on the test set using the best model obtained from GridSearchCV.
Submission:

The predictions are saved to a CSV file (submission.csv) for submission to Kaggle.
Training Accuracy (Optional):

Training accuracy is calculated for illustration purposes.
How to Use
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/titanic-survival-prediction.git
Navigate to the project directory:

bash
Copy code
cd titanic-survival-prediction
Run the script:

bash
Copy code
python titanic_prediction.py
Kaggle Submission
The script generates a submission file (submission.csv) that can be submitted to Kaggle for evaluation.

Note
The training accuracy is calculated for illustration purposes and is typically not done in practice.

Feel free to modify the features, hyperparameters, or other aspects of the script for experimentation.
