# Spam-Email-Classification
A classification project using logistic regression, CART, and Random Forest to identify spam emails from the Enron dataset.


## Project Overview
This project explores the classification of emails into spam and non-spam categories using machine learning models. The dataset is derived from the Enron email corpus, and the analysis includes feature engineering, data preprocessing, and the evaluation of three models:
- **Logistic Regression**
- **CART (Classification and Regression Trees)**
- **Random Forest**

## Key Results
- **Best Model:** Random Forest
  - **Test Accuracy:** 98.8%
  - **Test AUC:** 0.9989652
- Models were compared on both training and testing sets using metrics such as accuracy and AUC.

## Repository Structure
- `data/`: Contains example datasets (or instructions to access the data source).
- `scripts/`: Modular R scripts for data preprocessing, feature engineering, and modeling.
- `notebooks/`: Contains the original exploratory analysis in R.
- `outputs/`: Saved results such as plots and evaluation metrics.
- `README.md`: Project overview and instructions.

## Methods
### Data Preprocessing
1. Removed rows with missing or non-numeric values.
2. Calculated character counts for each email.
3. Created a document-term matrix (DTM) and a sparse DTM (spdtm) for word-level analysis.
4. Applied stemming and removed stopwords to focus on meaningful word stems.

### Models
1. **Logistic Regression:** Baseline model for classification.
2. **CART:** Decision tree algorithm for interpretable results.
3. **Random Forest:** An ensemble method for higher accuracy and robustness.

### Evaluation
Models were evaluated using:
- **Accuracy**: Fraction of correctly classified emails.
- **AUC**: Area Under the ROC Curve to measure classifier performance.

## Results Summary
| Model             | Train Accuracy | Train AUC | Test Accuracy | Test AUC   |
|--------------------|----------------|-----------|---------------|------------|
| Logistic Regression | 99.9%         | 0.9999995 | 77.8%         | 0.8115662  |
| CART               | 94.6%         | 0.9719    | 93.4%         | 0.9670     |
| Random Forest      | 98.4%         | 0.9990461 | 98.8%         | 0.9989652  |
