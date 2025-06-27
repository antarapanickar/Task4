This project is part of an AI/ML internship task that focuses on building a binary classification model using **Logistic Regression**. The goal is to predict if a breast tumor is **malignant** or **benign** based on medical features from cell nuclei images.

The dataset is a classic one from the UCI Machine Learning Repository and is hosted on Kaggle.

## Dataset

- **Name**: Breast Cancer Wisconsin Diagnostic Data
- **Source**: [Kaggle](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)
- **Target Column**: `diagnosis` (`M` = Malignant, `B` = Benign)
- **Number of Features**: 30 numeric features that describe characteristics like radius, texture, perimeter, area, and smoothness.

## Steps Followed

1. **Data Cleaning**
   - Removed irrelevant columns such as `id` and `Unnamed: 32`
   - Changed diagnosis values into binary form: `M` becomes 1, `B` becomes 0

2. **Train-Test Split**
   - Divided the dataset into 80% for training and 20% for testing using `train_test_split`

3. **Feature Scaling**
   - Used `StandardScaler` to normalize feature values

4. **Model Training**
   - Applied `LogisticRegression` from `sklearn`
   - Fit the model on the scaled training data

5. **Evaluation**
   - Assessed using:
     - Confusion Matrix
     - Precision
     - Recall
     - ROC-AUC Score
     - ROC Curve Plot

## Results

### Metrics:
- **Precision**: `0.98`
- **Recall**: `0.95`
- **ROC-AUC Score**: `1.00`

### ROC Curve:
The ROC curve shows excellent model performance with an AUC of 1.00; this indicates perfect separation between malignant and benign cases.

## Visuals

- Confusion matrix heatmap to analyze true and false predictions
- ROC curve to assess how the model performs across different thresholds

## Tools Used

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Kaggle Notebooks
