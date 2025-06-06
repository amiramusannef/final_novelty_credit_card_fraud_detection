# Credit Card Fraud Detection Using Explainable ANN
We selected this topic because while credit card fraud detection is a well-researched problem, much of the existing work emphasizes maximizing accuracy using advanced machine learning and deep learning models, often at the expense of interpretability. 

Goal: Optimizing fraud detection model performance while making the predictions of the model more understandable and transparent by visualizing which features influence their decisions.

## General Acknowledgement
The notebook was developed based on a [Kaggle notebook by Shalinee Kumari](https://github.com/Shalinee13/Credit-Card-Fraud-Detection-using-ML-models) which provided data understanding, EDA, model building and model evaluation.

**Modifications and Contributions (inspired from 3 literature works):**
- Added hybrid sampling (SMOTETomek)
- Built a custom ANN architecture using Keras with:
  - Batch Normalization
  - Dropout
  - L2 Regularization
  - Callbacks (EarlyStopping, ModelCheckpoint, Learning Rate Scheduler)
- Integrated SHAP for ANN interpretability
- Model comparison with Random Forest and feature importance analysis 

## Dataset 
The dataset used in this project is anonymized and was provided by an undisclosed institution for research purposes due to privacy and confidential issue. We sourced the dataset from a GitHub repository (https://github.com/Shalinee13/Credit-Card-Fraud-Detection-using-ML-models?tab=readme-ov-file) which references the original data hosted on Kaggle. Due to its large size, the files are available via OneDrive links provided in the repository 
* Dataset: Download the dataset from "cardtrans_csv_onedrive.txt" 

The dataset simulates transactional data related to credit card usage and fraud detection. Each row represents a single transaction and includes the following features:

> 1) distance_from_home: Distance between the transaction location and the cardholder's home.

> 2) distance_from_last_transaction: Distance from the location of the previous transaction.

> 3) ratio_to_median_purchase_price: Ratio of the current transaction amount to the cardholder’s median purchase price.

> 4) repeat_retailer: Binary indicator (1 or 0) showing if the transaction is at a retailer the customer has visited before.

> 5) used_chip: Indicates whether a chip was used in the card (1) or not (0).

> 6) used_pin_number: Indicates if a PIN was used during the transaction (1) or not (0).

> 7) online_order: Indicates if the transaction was done online (1) or in-person (0).

> 8) fraud: Binary label where 1 indicates a fraudulent transaction and 0 indicates a legitimate one.

## Tools & Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import shap
import warnings

from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.ensemble import RandomForestClassifier
from sklearn import metrics
from sklearn.metrics import (
    accuracy_score, f1_score, confusion_matrix,
    classification_report, average_precision_score, ConfusionMatrixDisplay
)

from imblearn.over_sampling import SMOTE
from imblearn.combine import SMOTETomek

from tensorflow import keras
from tensorflow.keras import regularizers

```

## Project Pipeline

1. Load and explore the dataset.
2. Preprocess the data (handle imbalance with hybrid sampling, scale features).
3. Build and train an Artificial Neural Network (ANN) using Keras.
4. Evaluate model performance using metrics like Accuracy, AUPRC, and F1-score.
5. Apply SHAP for feature explainability on ANN.
6. Train and evaluate a Random Forest model for comparison with feature importance analysis.
7. Compare models and visualize performance.

### This is Group 21 final project for DS340W Spring 2025. 
### Written by Nur Najwa Ayda Sahren & Che Amira Aisyah Musannef





