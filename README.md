 Customer Churn Prediction using IBM SPSS Modeler

 Project Overview

This project focuses on predicting customer churn using IBM SPSS Modeler.

The project uses customer data and a CHAID decision tree model to identify customers who are likely to churn.

The final output identifies high-risk customers whose predicted churn probability is greater than 0.9.

 Objective

The main objective of this project is to:

- Analyze customer data
- Prepare the data for modelling
- Build a CHAID predictive model
- Predict customer churn
- Identify customers at high risk of churn
- Export the high-risk customer information

 Tools & Technologies

- IBM SPSS Modeler
- CHAID Decision Tree
- Microsoft Excel
- Predictive Analytics

 Dataset

The project uses a Telco customer dataset containing customer-related information.

Important fields used in the project include:

- customer_id
- gender
- age
- tariff
- churn
- Other customer-related fields

 Project Workflow

The project follows these main steps:

1. Import the customer dataset into IBM SPSS Modeler.
2. Check and understand the available fields.
3. Define the required field types.
4. Set `churn` as the target field.
5. Build a CHAID model.
6. Generate predictions using the CHAID Model Nugget.
7. Select customers predicted as `Churned`.
8. Select customers whose churn probability is greater than 0.9.
9. Use a Filter node to keep the required fields.
10. Export the high-risk customers using a Flat File node.

 Model Used

CHAID Decision Tree

CHAID (Chi-square Automatic Interaction Detection) is a decision-tree-based modelling technique.

In this project, CHAID is used to predict whether a customer is likely to churn.

Customer Risk Selection

The project selects customers using the following condition:

```text
$R-churn = "Churned" AND $RC-churn > 0.9
