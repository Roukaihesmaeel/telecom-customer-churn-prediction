# telecom-customer-churn-prediction

# Customer Churn Prediction

## Project Overview

This project focuses on predicting customer churn in the telecommunications industry using Machine Learning.

The main objective is to identify customers who are likely to leave the company and provide useful insights that can support customer retention strategies.

## Business Problem

Customer churn can negatively affect a company's revenue and long-term growth.

By identifying customers with a high probability of churn, businesses can take proactive actions such as improving customer support, offering suitable plans, or providing retention offers.

## Dataset

The project uses the IBM Telco Customer Churn dataset.

The dataset contains 7,043 customers and 21 features, including:

* Customer demographic information
* Services and subscriptions
* Contract information
* Payment methods
* Monthly charges
* Total charges
* Customer churn status

## Exploratory Data Analysis

Exploratory Data Analysis was performed to understand customer behavior and identify patterns related to churn.

### Churn Distribution

* Customers who did not churn: 73.46%
* Customers who churned: 26.54%

### Churn by Contract Type

Customers with month-to-month contracts showed a significantly higher churn rate compared with customers with one-year and two-year contracts.

### Churn by Tenure

Customers with shorter tenure were more likely to churn.

The observed churn rates were approximately:

* 47.4% for customers with 0–12 months of tenure
* 28.7% for customers with 13–24 months
* 20.4% for customers with 25–48 months
* 9.5% for customers with 49–72 months

### Churn by Monthly Charges

Customers with higher monthly charges generally showed higher churn rates.

The highest observed churn rate was approximately 33.9% among customers paying between 61 and 90 per month.

## Data Preprocessing

The following preprocessing steps were performed:

* Converted `TotalCharges` into numeric values
* Handled missing values
* Identified categorical and numerical features
* Applied One-Hot Encoding to categorical variables
* Prepared the data for Machine Learning

## Machine Learning

Several Machine Learning models were evaluated.

### Logistic Regression

Accuracy:

**80.31%**

### Random Forest

Accuracy:

**78.39%**

### Balanced Logistic Regression

A balanced Logistic Regression model was used to improve the detection of customers who churn.

Performance:

* Accuracy: 73%
* Churn Precision: 49%
* Churn Recall: 80%
* Churn F1-Score: 61%

Churn Recall was given particular attention because correctly identifying customers who are likely to leave can help businesses take preventive retention actions.

## Feature Analysis

The most influential features included:

* Contract type
* Internet service
* Payment method
* Online security
* Technical support
* Senior citizen status

Month-to-month contracts were associated with higher churn risk, while two-year contracts were associated with lower churn risk.

## Prediction Application

The trained model can be used to analyze new customers and provide:

* Churn prediction
* Churn probability
* Risk level
* Business recommendation

Example prediction:

* Churn Prediction: Yes
* Churn Probability: 88.62%
* Risk Level: High

## Business Recommendation

For customers classified as high risk, the application recommends proactive retention actions such as contacting the customer and offering a suitable retention plan or discount.

## Interactive Application

A Gradio-based interface was developed to allow users to enter customer information and receive a churn prediction without directly interacting with the Machine Learning code.

## Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Gradio
* Google Colab

## Project Structure

```text
customer-churn-prediction/
│
├── Customer_Churn_Prediction.ipynb
├── model_results.csv
└── README.md
```

## Future Improvements

Future development could include:

* Hyperparameter tuning
* Advanced Machine Learning models
* SHAP-based model explainability
* Interactive dashboards
* Web application deployment
* Integration with real-time customer data

## Author

Ruqayya

Machine Learning / AI Project
