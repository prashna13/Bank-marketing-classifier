# Bank Marketing Classifier

A machine learning classification project that predicts whether a customer is likely to subscribe to a term deposit based on customer and campaign-related information.

## Overview

Banks use direct marketing campaigns to promote financial products such as term deposits. However, contacting every customer can be inefficient because only a portion of customers respond positively to a campaign.

This project applies supervised machine learning to the Bank Marketing dataset to classify customers based on whether they subscribed to a term deposit. A Random Forest classifier is used to learn patterns from customer demographics, financial information, and previous campaign interactions.

The project covers data preprocessing, exploratory analysis, feature preparation, model training, and evaluation.

## Objectives

* Explore customer and campaign data
* Identify factors associated with term deposit subscriptions
* Prepare categorical and numerical features for machine learning
* Train a Random Forest classification model
* Evaluate classification performance using appropriate metrics
* Understand which customer characteristics contribute to predictions

## Dataset

The project uses the Bank Marketing dataset, which contains information collected during direct marketing campaigns conducted by a Portuguese banking institution.

The target variable indicates whether a customer subscribed to a term deposit:

* `yes`: Customer subscribed to the term deposit
* `no`: Customer did not subscribe

The dataset contains customer demographic information, financial details, contact information, and campaign history.

## Machine Learning Approach

The project follows the following workflow:

1. Load and inspect the dataset
2. Perform exploratory data analysis
3. Clean and preprocess the data
4. Encode categorical variables
5. Separate features and target variable
6. Split the data into training and testing sets
7. Train a Random Forest classifier
8. Generate predictions on the test set
9. Evaluate the model using classification metrics
10. Analyze the model results

## Model

### Random Forest Classifier

Random Forest is an ensemble learning algorithm that combines multiple decision trees to produce a more robust classification model.

In this project, Random Forest is used because it can:

* Handle nonlinear relationships between features
* Work with a mixture of feature types after preprocessing
* Reduce overfitting compared with a single decision tree
* Provide feature importance information
* Perform well on structured tabular data

## Technologies Used

* Python
* pandas
* NumPy
* scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

## Project Structure

```text
Bank-marketing-classifier/
│
├── Bank Marketing_dataset/
│   └── Bank Marketing dataset files
│
├── bank_marketing_rf.ipynb
│
└── README.md
```

## Getting Started

### Clone the repository

```bash
git clone https://github.com/prashna13/Bank-marketing-classifier.git
cd Bank-marketing-classifier
```

### Install dependencies

Create a virtual environment if needed:

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

Install the required libraries:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

### Run the notebook

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
bank_marketing_rf.ipynb
```

Run the notebook cells in order to reproduce the analysis and model training process.

## Evaluation

The Random Forest model is evaluated using classification metrics such as:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion matrix

These metrics provide a more complete view of the model's performance than accuracy alone, particularly when the target classes are not evenly distributed.

## Key Learning Outcomes

This project provided practical experience with:

* Exploratory data analysis
* Data preprocessing
* Categorical feature encoding
* Supervised classification
* Random Forest models
* Model evaluation
* Feature importance analysis
* Working with real-world financial marketing data

## Limitations

The model is trained on historical campaign data, so its performance may change when applied to customers or campaigns with different characteristics.

The dataset also represents a specific banking campaign and should not be assumed to represent customer behaviour across different banks, countries, or time periods.

## Future Improvements

Potential improvements include:

* Comparing Random Forest with Logistic Regression, XGBoost, and other classifiers
* Applying cross-validation for more robust model evaluation
* Addressing class imbalance using suitable techniques
* Performing hyperparameter tuning
* Optimizing the classification threshold
* Adding feature importance visualizations
* Building an interactive prediction interface



```

This version deliberately avoids claiming specific accuracy scores or preprocessing techniques that I could not verify from the repository page.
```
