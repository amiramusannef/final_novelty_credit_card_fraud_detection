# Credit Card Fraud Detection Using Explainable ANN
We selected this topic because while credit card fraud detection is a well-researched problem, much of the existing work emphasizes maximizing accuracy using advanced machine learning and deep learning models, often at the expense of interpretability. 

Goal: Optimizing fraud detection model performance while making the predictions of the model more understandable and transparent by visualizing which features influence their decisions.

# General Acknowledgement
This model was developed based on a Kaggle notebook titled “Credit Card Fraud Detection using ML models” by Shalinee Kumari (https://github.com/Shalinee13/Credit-Card-Fraud-Detection-using-ML-models?tab=readme-ov-file), which provided data understanding, EDA, model building and model evaluation.

Modifications: Implementation of Hybrid Sampling Technique and ANN model building including custom dropout, batch normalization, and callback tuning. 

# Dataset 
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



