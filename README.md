# Company Bankruptcy Prediction

This project evaluates machine learning models for predicting corporate bankruptcy using financial indicators. The dataset contains **6,819 companies and 95 financial features**, with bankrupt companies representing only **3.2%** of the observations.

Because of this class imbalance, the analysis emphasizes **recall, ROC AUC, and PR AUC** rather than relying on accuracy alone.

## Key Results

| Model               | Precision |   Recall |   ROC AUC |    PR AUC |
| ------------------- | --------: | -------: | --------: | --------: |
| Logistic Regression |      0.16 |     0.73 |     0.881 |     0.275 |
| K-Nearest Neighbors |      0.57 |     0.24 |     0.758 |     0.232 |
| Decision Tree       |      0.19 | **0.82** |     0.925 |     0.226 |
| Random Forest       |  **0.25** |     0.67 | **0.938** | **0.329** |

Random Forest achieved the strongest overall ranking performance, with a ROC AUC of approximately **0.94** and the highest PR AUC. Decision Tree produced the highest recall, identifying 82% of bankrupt firms, but generated more false positives.

## Methods

* Exploratory data analysis and class-distribution assessment
* Stratified training and test split
* Feature standardization
* Class-weighted modeling
* Cross-validation and hyperparameter tuning
* Model comparison using precision, recall, ROC AUC, and PR AUC
* Permutation-based feature importance analysis

## Tools

* Python
* pandas and NumPy
* scikit-learn
* Matplotlib and Seaborn
* Jupyter Notebook

## Dataset

The analysis uses the [Taiwanese Bankruptcy Prediction dataset](https://archive.ics.uci.edu/dataset/572/taiwanese+bankruptcy+prediction) from the UCI Machine Learning Repository.

The dataset is not stored in this repository. It can be downloaded directly from UCI using the link above.

## Repository Structure

```text
company-bankruptcy-prediction/
├── bankruptcy_prediction.ipynb
├── requirements.txt
├── README.md
└── .gitignore
```

## Project Context

This analysis was developed as a team course project. This repository presents a cleaned and documented version of the analytical workflow for portfolio purposes.

