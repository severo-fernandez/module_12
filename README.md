## module_12 Challenge

# Credit Risk Classification - imbalanced data

Credit risk poses a classification problem that’s inherently imbalanced. This is because healthy loans easily outnumber risky loans. In this Challenge, you’ll use various techniques to train and evaluate models with imbalanced classes. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

This challenge consists of the following subsections:

* Split the Data into Training and Testing Sets

* Create a Logistic Regression Model with the Original Data

* Predict a Logistic Regression Model with Resampled Training Data 

# Import Modules

- import numpy as np
- import pandas as pd
- from pathlib import Path
- from sklearn.metrics import balanced_accuracy_score
- from sklearn.metrics import confusion_matrix
- from imblearn.metrics import classification_report_imbalanced

- import warnings
- warnings.filterwarnings('ignore')

- from sklearn.model_selection import train_test_split

- from sklearn.linear_model import LogisticRegression

- from imblearn.over_sampling import RandomOverSampler

# Results

- Both models predict loan risk-level well. However, due to the data imbalance, the resampled model has better overall results.