# Bank Customer Churn Prediction

## Project Description
This project aims to analyze and predict customer churn in the banking sector using machine learning techniques.  
Customer churn occurs when a client ends their relationship with the bank, leading to revenue loss and increased customer acquisition costs.

The project follows an end-to-end data science workflow, starting with exploratory data analysis (EDA) and progressing toward predictive modeling, with a strong focus on business understanding.

---

## Objective
- Identify patterns and factors associated with customer churn  
- Build models to predict which customers are more likely to leave the bank  
- Support proactive customer retention strategies  

---

## Dataset
- Source: Kaggle  
- Name: Bank Customer Churn Records  
- Size: 10,000 records  
- Features: 18 variables  
- Target variable: `Exited`  
  - 0 = Customer stayed  
  - 1 = Customer churned  

The dataset contains no missing values and includes numerical, binary, and categorical features.

---

## Exploratory Data Analysis (EDA)
The initial exploratory analysis included:
- Dataset size and structure inspection  
- Data type verification  
- Missing value analysis  
- Descriptive statistics for numerical variables  
- Identification of non-predictive columns  

### Key findings
- Around 20% of customers have churned  
- The dataset presents moderate class imbalance, common in real-world churn problems  
- Columns such as `RowNumber`, `CustomerId`, and `Surname` are identifiers and should not be used for modeling  
- Features related to customer activity, complaints, and satisfaction show strong predictive potential  

---
## Author
Cibele Vieira  
Project developed for academic purposes and data science portfolio building.

