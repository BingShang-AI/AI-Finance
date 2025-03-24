# Financial Risk Management - Fraud Detection

## Project Overview

This project focuses on developing a robust and adaptive fraud detection system for credit card transactions using a combination of Machine Learning (ML), Deep Learning (DL), and Natural Language Processing (NLP) techniques.

**Data Source:** Kaggle - [Credit Card Fraud Data](https://www.kaggle.com/datasets/neharoychoudhury/credit-card-fraud-data/data)

**AI Branches:**

*   Machine Learning (ML)
*   Deep Learning (DL)
*   Natural Language Processing (NLP)

**Models:**

*   Random Forest Classifier (RFC)
*   K-Means Clustering
*   Long Short-Term Memory Network (LSTM)
*   spaCy's built-in "en_core_web_sm" model

**Data Analytics Methods:**

*   **Binary Classification (RFC):** Predicting a binary outcome (fraudulent or not).
*   **Clustering (K-Means):** Grouping transactions based on similarities in selected features ('amt', 'transaction_hour').
*   **Time Series Forecasting (LSTM):** Predicting future values in a time series (daily fraud counts).
*   **Natural Language Processing (NLP) with spaCy:** Text processing for merchant name standardization and analysis.
*   **Exploratory Data Analysis (EDA):** Visualizations and statistical analysis to understand data patterns.

## 1. Business Problem Statement

Credit card fraud poses significant financial risks to institutions and individuals. Fraudulent transactions cause losses, increase operational costs, and damage trust. Traditional rule-based systems struggle with evolving fraud patterns and often generate a high number of false positives.  This project aims to develop a robust, adaptive, and accurate fraud detection system using ML, DL, and NLP to:

*   Identify fraudulent transactions in real-time.
*   Minimize false positives.
*   Protect stakeholders from financial losses.

The NLP component specifically addresses the challenge of inconsistent merchant names, improving the accuracy of merchant-based risk analysis.

## 2. Project Objectives

Addressing the limitations of traditional rule-based systems, this project develops a robust, adaptive, and accurate fraud detection system leveraging machine learning (ML), deep learning (DL), and natural language processing (NLP).  By analyzing a public credit card transaction dataset, the project aims to achieve:

*   **High-precision fraud detection:** Accurately identify fraudulent transactions.
*   **Identify distinct transaction groups:**  Use clustering to find groups with varying levels of fraud risk.
*   **Forecast future fraud trends:** Enable proactive risk management decision-making.
*   **Enhance merchant-based risk assessment:** Improve the identification of high-risk merchants.
*   **Identify key factors:** Determine the most important features related to fraudulent activity.
*   **Create an interactive tool and Chatbot:** Enable users to input transaction details to receive real-time fraud probability predictions and quickly identify risky merchants via a Chatbot.

## 3. Project Importance

*   **Financial Loss Mitigation:** Reduce financial losses due to fraud.
*   **Enhanced Customer Trust:** Build trust through proactive fraud prevention.
*   **Operational Efficiency:** Automate fraud detection, improving efficiency and reducing manual review efforts.
*   **Regulatory Compliance:** Meet regulatory requirements for fraud prevention.
*   **Adaptive Security:**  ML models can adapt to evolving fraud patterns.
*   **Proactive Risk Management:** Forecasting enables proactive risk mitigation strategies.
*   **Merchant Risk Profiling:** NLP identifies high-risk merchants, allowing for targeted interventions and improved risk management.

## 4. Project Procedures

1.  **Data Loading and Preprocessing:**  Load the dataset and prepare it for analysis (handling missing values, data type conversions, etc.).
2.  **Exploratory Data Analysis (EDA):**  Analyze the data to understand patterns, distributions, and relationships between variables.
3.  **Model Development:** Build, train, and tune the ML, DL, and NLP models.
4.  **Model Evaluation:** Assess the performance of the models using appropriate metrics (e.g., precision, recall, F1-score, AUC-ROC).
5.  **Documentation, Visualization and Reporting:** Document the project process, create visualizations to communicate findings, and generate a comprehensive report.

## 5. Data Field Description

The dataset contains information on credit card transactions, with a label indicating whether each transaction is fraudulent (`is_fraud`).

| Field Name             | Description                                                      | Data Type | Notes                                     |
| ----------------------- | ---------------------------------------------------------------- | --------- | ----------------------------------------- |
| `trans_date_trans_time` | Transaction date and time                                        | datetime  |                                           |
| `merchant`             | Merchant name                                                    | string    | Processed using NLP for standardization.   |
| `category`             | Merchant category                                                 | string    |                                           |
| `amt`                  | Transaction amount                                               | float     |                                           |
| `city`                 | Cardholder's city                                               | string    |                                           |
| `state`                | Cardholder's state                                              | string    |                                           |
| `lat`                  | Cardholder's latitude                                            | float     |                                           |
| `long`                 | Cardholder's longitude                                           | float     |                                           |
| `city_pop`             | Cardholder's city population                                      | integer   |                                           |
| `job`                  | Cardholder's occupation                                          | string    |                                           |
| `dob`                  | Cardholder's date of birth                                       | datetime  |                                           |
| `trans_num`            | Unique transaction identifier                                     | string    |                                           |
| `merch_lat`            | Merchant's latitude                                             | float     |                                           |
| `merch_long`           | Merchant's longitude                                            | float     |                                           |
| `is_fraud`             | Fraud indicator (1 for fraudulent, 0 for not fraudulent)          | integer   | Target variable                           |
