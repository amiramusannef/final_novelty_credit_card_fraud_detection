# Credit Card Fraud Detection Using Explainable ANN
We selected this topic because while credit card fraud detection is a well-researched problem, much of the existing work emphasizes maximizing accuracy using advanced machine learning and deep learning models, often at the expense of interpretability. 

Goal: Optimizing fraud detection model performance while making the predictions of the model more understandable and transparent by visualizing which features influence their decisions.

# General Acknowledgement
This model was developed based on a Kaggle notebook titled “Credit Card Fraud Detection using ML models” by Shalinee Kumari (https://github.com/Shalinee13/Credit-Card-Fraud-Detection-using-ML-models?tab=readme-ov-file), which provided data understanding, EDA, model building and model evaluation.

Modifications: Implementation of Hybrid Sampling Technique and ANN model building including custom dropout, batch normalization, and callback tuning. 

# Dataset 
The dataset used in this project is anonymized and was provided by an undisclosed institution for research purposes due to privacy and confidential issue. It simulates transactional data related to credit card usage and fraud detection.

Each row represents a single transaction and includes the following features:

> 1) distance_from_home: Distance (in km) between the transaction location and the cardholder's home.

> 2) distance_from_last_transaction: Distance (in km) from the location of the previous transaction.

ratio_to_median_purchase_price: Ratio of the current transaction amount to the cardholder’s median purchase price.

repeat_retailer: Binary indicator (1 or 0) showing if the transaction is at a retailer the customer has visited before.

used_chip: Indicates whether a chip was used in the card (1) or not (0).

used_pin_number: Indicates if a PIN was used during the transaction (1) or not (0).

online_order: Indicates if the transaction was done online (1) or in-person (0).

fraud: Binary label where 1 indicates a fraudulent transaction and 0 indicates a legitimate one.

This dataset enables the modeling and evaluation of fraud detection systems based on transactional patterns and contextual features.

