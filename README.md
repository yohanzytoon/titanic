# Titanic Kaggle Project

This repository contains my solution for the Titanic Kaggle competition. The goal of the competition is to predict the survival of passengers aboard the Titanic based on various features in the dataset. 

This project demonstrates the full machine learning pipeline, including data preprocessing, feature engineering, model training with XGBoost, and generating a submission file for the Kaggle leaderboard.

---

## Files

- `titanic.ipynb`: The Jupyter Notebook containing all the code for the project, including data exploration, preprocessing, feature engineering, model training, and evaluation.
- `train.csv`: The training dataset provided by Kaggle.
- `test.csv`: The test dataset provided by Kaggle.
- `gender_submission.csv`: A dataset with baseline gender-based predictions for the Titanic competition.
- `submission.csv`: The final output file with predictions for the test dataset, ready for submission to Kaggle.
- `environment.yaml`: A Conda environment file to reproduce the Python environment used for this project.

---

## Features and Workflow

1. **Data Preprocessing**:
   - Handling missing values in columns such as `Age`, `Fare`, and `Embarked`.
   - Extracting additional features like `Title`, `FamilySize`, `IsAlone`, and `Deck` from the raw data.

2. **Feature Engineering**:
   - Converting categorical variables (`Sex`, `Embarked`, `Title`, `Deck`) into numeric using one-hot encoding.
   - Creating new features (`FamilySize`, `IsAlone`) to capture relationships between passengers.

3. **Model Training**:
   - Using **XGBoost** for classification.
   - Hyperparameter tuning and validation using early stopping to prevent overfitting.

4. **Model Evaluation**:
   - Accuracy score on the validation set.
   - Predictions on the test set with a final submission file for Kaggle.

5. **Reproducibility**:
   - The `environment.yaml` file allows others to set up the same Python environment to run the code seamlessly.

---

## Setup Instructions

### Clone the Repository
To clone this repository to your local machine:
```bash
git clone https://github.com/yourusername/titanic-kaggle-project.git
cd titanic-kaggle-project
