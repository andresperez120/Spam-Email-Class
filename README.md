# Spam-Email-Classification

A classification project using Logistic Regression, CART, and Random Forest to identify spam emails from the Enron dataset.

## Project Overview
This project explores the classification of emails into spam and non-spam categories using machine learning models. The dataset is derived from the Enron email corpus. The analysis includes data preprocessing, feature engineering, model training, and evaluation of three classification models:

- **Logistic Regression**: Baseline model for classification.
- **CART (Classification and Regression Trees)**: For interpretable decision paths.
- **Random Forest**: An ensemble method for improved accuracy and robustness.

## Key Results
- **Best Model**: Random Forest
- **Test Accuracy**: 98.8%
- **Test AUC**: 0.9995
- Models were evaluated on both training and testing sets using metrics such as accuracy and AUC.

## Repository Structure
├── README.md # Project overview and instructions 
├── Spam_Email_Classification.Rmd # R Markdown file with the full analysis 
├── Spam_Email_Classification.html # Knitted HTML output of the analysis 
├── Spam_Email_Classification.pdf # Knitted PDF output of the analysis 
├── emails.csv # Dataset for spam classifications

## Methods

### Data Preprocessing
1. Removed rows with missing or non-numeric values.
2. Calculated the character count for each email.
3. Created a document-term matrix (DTM) and a sparse DTM (spdtm) for word-level analysis.
4. Applied stemming and removed stopwords to focus on meaningful word stems.

### Model Training
Three models were trained and evaluated:
1. **Logistic Regression**: Provided a baseline for comparison.
2. **CART**: Decision tree algorithm for interpretable results.
3. **Random Forest**: An ensemble method that significantly outperformed the other models.

### Evaluation Metrics
- **Accuracy**: Fraction of correctly classified emails.
- **AUC**: Area Under the ROC Curve, measuring classifier performance.

### Results Summary
| Model                 | Train Accuracy | Train AUC | Test Accuracy | Test AUC |
|-----------------------|----------------|-----------|---------------|----------|
| Logistic Regression   | 99.9%         | 0.9999    | 81.25%        | 0.848    |
| CART                  | 94.1%         | 0.9670    | 94.06%        | 0.9670   |
| Random Forest         | 98.8%         | 0.9995    | 98.78%        | 0.9995   |

## Conclusion
Random Forest outperformed Logistic Regression and CART in both accuracy and AUC, making it the most suitable model for spam email classification. CART provided interpretable results, while Logistic Regression offered a simpler baseline model.

---

## How to Run the Project
1. Clone this repository:
   ```bash
   git clone https://github.com/andresperez120/Spam-Email-Classification.git
