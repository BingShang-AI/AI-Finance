# Credit Card Fraud Detection: Data Analysis and Model Development

## **Project Overview**

**Data Source:** [Kaggle - Credit Card Fraud Data](https://www.kaggle.com/datasets/neharoychoudhury/credit-card-fraud-data/data)

**AI Branches:** Machine Learning (ML), Deep Learning (DL), and Natural Language Processing (NLP)

**Models:**

*   Random Forest Classifier (RFC)
*   Long Short-Term Memory Network (LSTM)
*   spaCy's built-in model (`en_core_web_sm`)

**Data Analytics Methods:**

*   **Binary Classification (RFC):** Predicting a binary outcome (fraudulent or not).
*   **Time Series Forecasting (LSTM):** Predicting future values in a time series (daily fraud counts).
*   **Natural Language Processing (NLP) with spaCy:** Text processing for merchant name standardization and analysis.
*   **Exploratory Data Analysis (EDA):** Visualizations and statistical analysis to understand data patterns.

## **1. Business Problem Statement**

Credit card fraud poses significant financial risks to institutions and individuals. Fraudulent transactions cause losses, increase operational costs, and damage trust. Traditional rule-based systems struggle with evolving fraud and high false positives. This project aims to develop a robust, adaptive, and accurate fraud detection system using ML, DL, and NLP to identify fraudulent transactions in real-time, minimize false positives, and protect stakeholders. The NLP component specifically addresses the challenge of inconsistent merchant names, improving the accuracy of merchant-based risk analysis.

## **2. Project Objectives**

Addressing the limitations of traditional rule-based systems, this project develops a robust, adaptive, and accurate fraud detection system leveraging machine learning (ML), deep learning (DL), and natural language processing (NLP). By analyzing a public credit card transaction dataset, the project aims to achieve:

*   **High-precision fraud detection:**  Accurately identify fraudulent transactions.
*   **Forecast future fraud trends:**  Enable proactive risk management decision-making.
*   **Enhance merchant-based risk assessment:**  Improve the identification of high-risk merchants through NLP.
*   **Identify key factors:** Determine the factors most strongly associated with fraudulent activity.
*   **Create an interactive tool:**  Allow users to input transaction details and receive real-time fraud probability predictions.

## **3. Project Importance**

*   **Financial Loss Mitigation:** Reduce financial losses due to fraud.
*   **Enhanced Customer Trust:** Build trust through proactive fraud prevention.
*   **Operational Efficiency:** Automate fraud detection, improving efficiency and reducing manual review.
*   **Regulatory Compliance:** Meet regulatory requirements for fraud prevention.
*   **Adaptive Security:** ML models can adapt to evolving fraud patterns.
*   **Proactive Risk Management:** Forecasting enables proactive risk mitigation.
*   **Merchant Risk Profiling:** NLP identifies high-risk merchants, allowing for targeted interventions and improved risk management.

## **4. Project Procedures**

1.  **Data Loading and Preprocessing:** Loading the dataset and preparing it for analysis (cleaning, handling missing values, feature engineering).
2.  **Exploratory Data Analysis (EDA):**  Analyzing and visualizing the data to identify patterns, trends, and anomalies.
3.  **Model Development:** Building and training the ML (RFC) and DL (LSTM) models.
4.  **Model Evaluation:** Assessing the performance of the models using appropriate metrics.
5.  **Documentation, Visualization and Reporting:**  Documenting the entire process, creating visualizations, and reporting the findings.

## **5. Data Field Description**

The dataset contains information on credit card transactions, with a label indicating whether each transaction is fraudulent (`is_fraud`):

| Field Name              | Description                                      | Data Type |
|--------------------------|--------------------------------------------------|-----------|
| `trans_date_trans_time` | Transaction date and time                         | datetime  |
| `merchant`              | Merchant name                                     | string    |
| `category`              | Merchant category                                 | string    |
| `amt`                   | Transaction amount                                | float     |
| `city`                  | Cardholder's city                                 | string    |
| `state`                 | Cardholder's state                                | string    |
| `lat`                   | Cardholder's latitude                             | float     |
| `long`                  | Cardholder's longitude                            | float     |
| `city_pop`              | Cardholder's city population                       | integer   |
| `job`                   | Cardholder's occupation                           | string    |
| `dob`                   | Cardholder's date of birth                         | datetime  |
| `trans_num`             | Unique transaction identifier                      | string    |
| `merch_lat`             | Merchant's latitude                               | float     |
| `merch_long`            | Merchant's longitude                              | float     |
| `is_fraud`              | Fraud indicator (1 for fraudulent, 0 for not)     | integer   |
