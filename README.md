# Hoeffding-Trees-for-Data-Stream-Classification

## A Survey on Adaptive Splitting, Concept Drift, and Ensemble Methods

## 📌 Project Overview

This project explores Hoeffding Trees and their application to data stream classification. Unlike traditional machine learning models that are trained on a complete dataset, data stream models learn incrementally as new data arrives.

The project compares traditional batch learning with online learning algorithms and investigates how adaptive models respond to changes in data patterns, known as concept drift.

The experiments use the Kaggle Credit Card Fraud Detection dataset to simulate an incoming transaction stream. A separate synthetic dataset is also used to create controlled concept drift and study model adaptation.

## 🎯 Objectives

- Understand the fundamentals of data stream classification.
- Explore how Hoeffding Trees perform incremental learning.
- Study adaptive splitting and concept drift.
- Compare traditional and online machine learning algorithms.
- Evaluate ensemble methods for streaming data.
- Analyse model performance on an imbalanced classification problem.

## 🧠 Algorithms Implemented

- Decision Tree
- Hoeffding tree
- Hoeffding Adaptive tree
- Adaptive random forest
  
## 📊 Dataset

Credit Card Fraud Detection Dataset

Source: [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
The dataset contains anonymised credit card transactions made by European cardholders.

## ⚙️ Methodology

The project follows a stream-based evaluation approach:

1.**Data loading**: Load the Kaggle dataset and inspect its structure.
2.**Preprocessing**: Sort transactions by time and separate features from target labels.
3.**Initial training**: Use an initial portion of the data to initialise the models.
4.**Stream simulation**: Feed the remaining transactions one at a time.
5.**Prequential evaluation**: Predict the class of each transaction before updating the model with its actual label.
6.**Performance evaluation**: Compare the algorithms using classification metrics.
7.**Concept drift experiment**: Generate a synthetic stream with a controlled change in the relationship between features and labels.
8.**Comparison**: Analyse how traditional and adaptive models respond to incoming data and concept drift.

## 📈 Evaluation Metrics

Because fraudulent transactions are extremely rare, accuracy alone is not sufficient to evaluate model performance.

The following metrics are used:

- Accuracy: Overall proportion of correct predictions.
- Precision: Proportion of predicted fraud cases that are actually fraudulent.
- Recall: Proportion of actual fraud cases correctly identified.
- F1-score: Harmonic mean of precision and recall.
- Average Precision: Summarises precision-recall performance across different classification thresholds.

## 🔄 Concept Drift Experiment

Concept drift occurs when the relationship between input features and target labels changes over time.

To study this behaviour, a synthetic dataset is generated with two different classification patterns:

- Before drift: The target depends on the first feature.
- After drift: The target depends on the second feature.

This controlled experiment makes it possible to compare how traditional and adaptive algorithms respond to a known change in the data.

## Author

Anamika J
- GitHub: github.com/Anamika79
- LinkedIn: linkedin.com/in/anamika-j
