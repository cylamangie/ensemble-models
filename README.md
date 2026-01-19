# Ensemble Models Project

📓 [View the Jupyter Notebook](ensemble_models.ipynb)

## 📌 Overview
This project explores and compares multiple ensemble learning methods on tabular data, including bagging, boosting, voting, and stacking.  
It evaluates training and testing accuracy to understand generalization performance across models.

> 📝 **Note**: This is the **first lab assignment** for **COM6104 – Topics in Data Science and Artificial Intelligence**.  
It documents hands-on experimentation with ensemble methods and serves as a portfolio piece for job applications.

## 🎯 Motivation
Ensemble models are widely used in industry for tabular data due to their ability to reduce overfitting and improve predictive accuracy.  
This project demonstrates practical machine learning skills, model benchmarking, and reproducible experimentation.

## ⚙️ Models Compared
- **Decision Tree**: Simple baseline model
- **XGBoost**: Gradient boosting with regularization
- **LightGBM**: Fast gradient boosting with histogram-based splits
- **Extra Trees**: Randomized tree ensemble (bagging)
- **AdaBoost**: Sequential boosting with weak learners
- **Voting Classifier**: Combines multiple models via soft voting
- **Stacking Classifier (2 models)**: Combines RF and GB with Logistic Regression
- **Stacking Classifier (3 models)**: Combines RF, GB, ET with Logistic Regression

## 📊 Results

| Model                        | Training Accuracy | Testing Accuracy | Runtime     |
|-----------------------------|-------------------|------------------|-------------|
| Decision Tree               | 98.94%            | 33.93%           | < 1 min     |
| XGBoost                     | 51.82%            | 49.21%           | ~ 3 mins    |
| LightGBM                    | 51.48%            | 49.49%           | ~ 2 mins    |
| Extra Trees                 | 98.94%            | 49.61%           | < 1 min     |
| AdaBoost                    | 49.99%            | 49.91%           | < 1 min     |
| Voting Classifier           | 77.20%            | 50.17%           | ~ 15 mins   |
| Stacking (RF + GB)          | 93.59%            | 50.16%           | 51 mins     |
| Stacking (RF + GB + ET)     | 98.36%            | 50.30%           | 48 mins     |

## 🚀 How to Run
```bash
pip install -r requirements.txt
python main.py
