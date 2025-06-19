# Spaceship Titanic - Kaggle Competition

This repository contains my solution for the [Spaceship Titanic Kaggle competition](https://www.kaggle.com/competitions/spaceship-titanic/overview). The objective is to predict which passengers were transported to an alternate dimension using machine learning models.

## File Structure

```
Spaceship Titanic/
├── data/
|   ├── sample_submission.csv
│   ├── train.csv
│   ├── test.csv
├── spaceship_titanic.ipynb
├── requirements.txt
├── .gitignore
├── LICENSE
└── README.md
```

## Python Environment

- **Python version:** 3.9+
- All dependencies are listed in `requirements.txt`.

To install the required packages, run:
```
pip install -r requirements.txt
```

## Models Used

The following scikit-learn models are implemented and compared to determine the best performer:

- **Logistic Regression**
- **Decision Tree Classifier**
- **Multi-layer Perceptron (MLP) Classifier**
- **Support Vector Machine (SVM) Classifier**
- **AdaBoost Classifier**

## Model Evaluation

Each model is evaluated using the following metrics: **Precision**, **Recall**, **F1-Score**, and **Accuracy**.

| Model                | Precision | Recall | F1-Score | Accuracy |
|----------------------|-----------|--------|----------|----------|
| Logistic Regression  |    0.86     |   0.86   |    0.86    |    0.86    |
| Decision Tree        |    1.00     |   1.00   |    1.00    |    0.99    |
| MLP Classifier       |    0.99     |   0.99   |    0.99    |    0.99    |
| Ridge SVM Classifier       |    0.96     |   0.96   |    0.96    |    0.96    |
| AdaBoost Classifier  |    0.78     |   0.78   |    0.78    |    0.78    |

## Final Thoughts

This project follows a standard machine learning workflow: data exploration, preprocessing, model selection, and evaluation. While logistic regression provides a strong baseline, tree-based and neural network models may capture more complex patterns. Future improvements could include hyperparameter tuning, advanced feature engineering, and model ensembling. The modular structure of the codebase makes it easy to extend and experiment