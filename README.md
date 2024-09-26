

### Overview

This project involves developing a machine learning model to predict fraudulent transactions for a financial company. The dataset used in this project is large, containing 6,362,620 rows and 10 columns, and is provided in CSV format. The primary goal is to build a predictive model to identify fraudulent transactions and provide actionable insights to prevent fraud.

**Important Note:** The dataset used in this project is not owned by me. It is provided for educational and research purposes. All rights and permissions related to the dataset are held by the original owner.

### Data Access
To replicate this analysis, you will need to access the dataset used for this project. Please download the dataset from the following link:

- **[Download Dataset](https://drive.google.com/file/d/1hKuOvYlADY0CT0kG2kL2vV1btXSvfddu/view?usp=sharing)**

Important: This dataset is provided for educational and research purposes. The dataset’s ownership and permissions are held by the original provider. Be sure to review and adhere to any usage terms associated with the dataset.

For details on the dataset’s structure and features, refer to the [Data Description](https://drive.google.com/file/d/1NKF-VLlAK2RkeTaqw7A4UBy_72zYH9oC/view?usp=sharing) File.

### Data Description

The dataset includes the following columns:

- **step:** Represents time in hours; each step is equivalent to 1 hour. The total simulation spans 744 steps, covering 30 days.
  
- **type:** Type of transaction, including:
  - `CASH-IN`
  - `CASH-OUT`
  - `DEBIT`
  - `PAYMENT`
  - `TRANSFER`

- **amount:** Amount of the transaction in local currency.

- **nameOrig:** Customer initiating the transaction.

- **oldbalanceOrg:** Initial balance of the customer before the transaction.

- **newbalanceOrig:** New balance of the customer after the transaction.

- **nameDest:** Customer receiving the transaction. Note: Information is not available for customers whose IDs start with 'M' (Merchants).

- **oldbalanceDest:** Initial balance of the recipient before the transaction. Note: Information is not available for customers whose IDs start with 'M' (Merchants).

- **newbalanceDest:** New balance of the recipient after the transaction. Note: Information is not available for customers whose IDs start with 'M' (Merchants).

- **isFraud:** Indicator of fraudulent transactions. Fraudulent behavior in this dataset involves agents taking control of customer accounts and attempting to empty the funds by transferring them to another account and then cashing out.

- **isFlaggedFraud:** Indicates whether a transfer is flagged as illegal. Transfers exceeding 200,000 in a single transaction are flagged.

### Objectives

1. **Model Development:** Develop and train a machine learning model to predict fraudulent transactions. Techniques can include Logistic Regression, Decision Trees, Random Forests, Gradient Boosting, Neural Networks, etc.

2. **Model Evaluation:** Evaluate the model's performance using metrics such as accuracy, precision, recall, F1 score, and AUC-ROC. Ensure evaluation on separate calibration and validation datasets for robustness.

3. **Insights and Action Plan:** Use the model’s predictions to generate insights and recommendations to help the company mitigate fraudulent activities.

### Procedure

1. **Data Preparation:** Clean and preprocess the data, handling missing values, encoding categorical variables, and scaling features as necessary.

2. **Model Training:** Apply various machine learning algorithms, tune hyperparameters, and validate models using cross-validation.

3. **Model Testing:** Assess the model on a validation dataset to verify its ability to predict fraudulent transactions effectively.

4. **Interpretation:** Analyze the model’s results and feature importance to understand key factors contributing to fraud. Develop actionable strategies based on these insights.

### Files and Resources

- `fraud_detection.csv`: The dataset used for model development. **Note:** This dataset is not owned by me. Please refer to the original source for permissions and use restrictions.
- `data_preprocessing.py`: Script for data cleaning and preprocessing.
- `model_training.py`: Script for training and evaluating machine learning models.
- `insights_and_recommendations.pdf`: Document detailing the insights from the model and recommended actions.



