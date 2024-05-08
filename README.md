# Customer Churn Analysis

[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
[![made-with-pandas](https://img.shields.io/badge/Made%20with-Pandas-150458.svg)](https://pandas.pydata.org/)
[![made-with-scikit-learn](https://img.shields.io/badge/Made%20with-scikit--learn-f7931e.svg)](https://scikit-learn.org/stable/)
[![imbalanced-learn](https://img.shields.io/badge/Imbalanced--learn-library-f7931e.svg)](https://imbalanced-learn.org/)
[![made-with-numpy](https://img.shields.io/badge/Made%20with-NumPy-777BB4.svg)](https://numpy.org/)
[![made-with-plotly](https://img.shields.io/badge/Made%20with-Plotly-3F4F75.svg)](https://plotly.com/)



## 👀 Description

This project is aimed at a major financial institution concerned with a high customer churn rate among credit cardholders. The goal is to analyze the client database to predict which clients are more likely to close their accounts after being targeted by competing offers. Our main priority is to find the optimal classification model to trigger an attrition flag for customers at risk.

The tested classification models are: AdaBoost, Decision Tree, Gradient Boost, K Nearest Neighbours, Logistic Regression, and Random Forest.

![alt text](https://s.yimg.com/ny/api/res/1.2/t7kTIpm2KCY9Kc_jxEzetA--/YXBwaWQ9aGlnaGxhbmRlcjt3PTk2MDtoPTY0MDtjZj13ZWJw/https://media.zenfs.com/en/gobankingrates_644/b33b3dca38e91ee95153dd93fc8558e5)

## 📦 Repo Structure
```
.
├── Classification/
│ ├── -Model summaries.md
│ ├── AdaBoost.ipynb
│ ├──Decision_Tree.ipynb
│ ├──Gradient_boost.ipynb
│ ├──KNN.ipynb
│ ├──Log_regression.ipynb
│ ├──Rand_forest.ipynb
├── Data/
│ ├── BankChurners.csv
├── Exploration/
│ ├── exploration.ipynb
├── .gitignore
├── requirements.txt
└── README.md
```


## 📈  Model Metrics Summaries
All metrics were taken after hyperparameter tuning. Given the imbalanced nature of the target variable, SMOTE was applied to improve model performance. The models were evaluated based on accuracy, ROC AUC, and a comprehensive classification report, including cross-validation to ensure robustness.

### Best Models
- **Random Forest**: Demonstrates strong performance with consistent accuracy and F1-scores. Overall test accuracy improved slightly after introducing SMOTE.
- **Gradient Boost**: Exceptional performance with high accuracy and ROC AUC.

### Discussion
SMOTE generally improves recall at the cost of precision. Models like Gradient Boost and Random Forest were less affected by SMOTE, showing robustness to class imbalance. The other models decreased on all metrics other than minority group (expired customers) recall. However, since the top priority is to detect this group spicifally, we opt for a model that indeed implements SMOTE.

For more detailed model performance analyzation and the performance metrics for each model, please refer to the `-Model summaries` file.

## ⏱️ Timeline
This project was completed over the course of three days.

## 📌 Personal Situation
This project was developed as part of my training into machine learning at [BeCode](https://becode.org/). It serves as a practical application of data preprocessing, feature engineering, and model training and evaluation

Connect with me on [LinkedIn](https://www.linkedin.com/in/viktor-cosaert/).
