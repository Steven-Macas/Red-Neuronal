<div align="center">

# Customer Churn Prediction

**Predicting which customers will leave, with logistic regression and a neural network**

<a href="https://colab.research.google.com/github/Steven-Macas/Red-Neuronal/blob/main/ejercicio_churn_red_neuronal.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab" /></a> <img src="https://img.shields.io/badge/Python-3-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python: 3" /> <img src="https://img.shields.io/badge/Pandas-data-150458?style=flat-square&logo=pandas&logoColor=white" alt="Pandas: data" /> <img src="https://img.shields.io/badge/scikit--learn-ML-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn: ML" /> <img src="https://img.shields.io/badge/TensorFlow-Keras-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" alt="TensorFlow: Keras" />

</div>

## Overview

Binary classification of customer churn. The notebook prepares the data, analyses which features matter
most, trains a **logistic regression** baseline and then **Keras neural networks** with one and two outputs.

## Approach

1. **Data preparation** – cleaning of `Churn.csv` and a split into training, validation and test sets (about 54 / 26 / 20 %).
2. **Feature importance** – analysis of how each property relates to churn.
3. **Feature engineering** – one-hot encoding with `DictVectorizer` (45 input features).
4. **Baseline** – `LogisticRegression` (liblinear) evaluated with predicted probabilities on the validation set.
5. **Neural network** – Dense(45, ReLU) → Dense(45, ReLU) → Dense(1, sigmoid), Adam, binary cross-entropy, 500 epochs.
6. **Variant** – the same network with two outputs.

## Results

| Model | Data | Accuracy |
| --- | --- | --- |
| Neural network (1 output) | training set | 81.7 % |

## How to run

Open the notebook in Colab with the badge above and upload `Churn.csv`.

*The notebook is written in Spanish.*

---

<sub>Made by <b>Steven Macas</b> — Data Engineer &amp; Data Analyst · <a href="https://gointy.com">gointy.com</a> · <a href="https://www.linkedin.com/in/steven-macas">LinkedIn</a> · <a href="https://github.com/Steven-Macas">GitHub</a></sub>
