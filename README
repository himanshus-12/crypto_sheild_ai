# CryptoShieldAI 🔐
### Ethereum Account Fraud Detection using Machine Learning

## About the Project

CryptoShieldAI is a mini machine learning project where I explore Ethereum account transaction data and try to predict whether an account is legitimate or fraudulent.

The main goal of this project was to understand how a machine learning classification problem works, starting from exploring a dataset and preparing features to training different models and comparing their performance.

I experimented with three classification algorithms:

- Logistic Regression
- Random Forest
- XGBoost

This is one of my early machine learning projects, and it helped me get hands-on experience with data analysis, feature engineering and model evaluation.

## What I Worked On

Here's what I implemented in the notebook:

- Loaded and explored the Ethereum account dataset.
- Checked dataset dimensions, data types, missing values and duplicate records.
- Visualized feature distributions using histograms, box plots and scatter plots.
- Created a correlation heatmap to understand relationships between numerical features.
- Separated the target column (`flag`) from the input features.
- Removed the `address` column because it is an account identifier.
- Created 7 additional features using existing transaction-related columns.
- Split the dataset into training, validation and testing sets.
- Applied feature scaling for Logistic Regression.
- Trained and compared three machine learning models.
- Evaluated the models using accuracy, precision, recall, F1-score and ROC-AUC.
- Visualized confusion matrices, ROC curves and Random Forest feature importance.

## Dataset

The dataset contains Ethereum account information and transaction-related features.

- Total records: 12,146
- Original columns: 33
- Target column: `flag`
- Account identifier: `address`

The target variable represents the account class:

- `0` — Legitimate account
- `1` — Fraudulent account

After feature engineering, the notebook works with 38 input features.

**Dataset source:** [Add the original dataset link here.]

The dataset is not included in this repository. You will need to obtain it separately.

## Feature Engineering

I created seven additional features from the existing transaction columns:

1. `netEtherFlow`
2. `transactionsPerDay`
3. `transactionsPerLifetimeDay`
4. `averageSentValue`
5. `averageReceivedValue`
6. `transactionCountRatio`
7. `averageValueDifference`

The idea was to represent transaction behaviour in a few additional ways and see whether these features could help the models.

## Models Used

| Model | Why I used it |
|---|---|
| Logistic Regression | As a baseline classification model |
| Random Forest | To experiment with an ensemble of decision trees |
| XGBoost | To compare performance with gradient boosting |

## Train-Test Setup

I used a stratified split:

- 60% Training data
- 20% Validation data
- 20% Testing data

The test set was kept separate for the final model comparison.

StandardScaler was used for Logistic Regression, while Random Forest and XGBoost were trained using unscaled features.

## Results

The saved notebook run produced the following results:

| Model | Accuracy | Precision | Recall | F1-score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 78.40% | 71.98% | 80.29% | 75.91% | 0.8871 |
| Random Forest | 94.73% | 94.39% | 93.11% | 93.74% | 0.9857 |
| XGBoost | 95.31% | 95.08% | 93.79% | 94.43% | 0.9915 |

In this run, XGBoost achieved the highest overall scores among the three models.

These are results from one held-out test split. They do not guarantee the same performance on new Ethereum accounts.

## Tech Stack

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Google Colab / Jupyter Notebook

## Running the Project

1. Clone this repository.
2. Install the required libraries.
3. Download the dataset from its original source.
4. Upload `crypto_dataset.csv` to your Google Colab session.
5. Open the notebook and run the cells in order.

Install dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn xgboost
```

## Limitations

- The results depend on the dataset and the particular split used.
- The notebook uses a single train/validation/test split.
- The model has not been tested on an independent external dataset.
- Possible duplicate accounts and feature leakage need further investigation.
- High evaluation scores do not necessarily mean the model will perform equally well in real-world fraud detection.

This project is an educational machine learning experiment and should not be treated as a production fraud-detection tool.

## Future Improvements

Some things I would like to explore further:

- Testing the models on an independent dataset.
- Investigating feature importance and possible data leakage.
- Experimenting with hyperparameter tuning.
- Trying additional feature-selection techniques.
- Exploring ways to explain individual model predictions.

---

**Built as a hands-on machine learning mini project while learning data science and classification.**
