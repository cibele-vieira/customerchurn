# Bank Customer Churn Prediction

## Data Source
The dataset used in this project was obtained from Kaggle and is used for educational and portfolio purposes only.

This project focuses on predicting customer churn using a structured machine learning pipeline, combining exploratory data analysis and supervised learning models. The objective is to identify customers at higher risk of leaving the bank and to understand the main factors driving churn.

## Dataset
The dataset was obtained from Kaggle and contains information about bank customers, including demographic, financial, and behavioral attributes.  
The target variable is **Exited**, where:
- 1 indicates the customer churned
- 0 indicates the customer remained with the bank

## Exploratory Data Analysis (EDA)
A comprehensive exploratory analysis was conducted before model training. The analysis included:
- Distribution and statistical overview of numerical variables
- Churn analysis by age, geography, gender, and activity status
- Bidimensional analysis to evaluate combined effects of key variables (e.g., Age × Geography, Age × Activity)

This analysis revealed strong and consistent churn patterns, particularly higher churn rates among customers aged 51–60 and customers located in Germany.

Variables that could cause data leakage were identified and removed to ensure realistic model performance.

## Modeling Approach
Two supervised learning models were trained and evaluated:

- **Logistic Regression**: Used as a baseline model due to its simplicity and interpretability.
- **Random Forest Classifier**: Used to capture non-linear relationships and interactions between features.

## Model Evaluation
Models were evaluated using multiple metrics, including:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

While Logistic Regression provided a solid baseline, it showed low recall for churned customers. The Random Forest model significantly improved recall, precision, and F1-score, demonstrating a better ability to identify customers at risk of churn.

## Results
The Random Forest model outperformed Logistic Regression across all key metrics, making it the preferred model for this churn prediction task. Its ability to capture complex customer behavior makes it more suitable for real-world retention strategies.

## Conclusion
This project demonstrates the importance of combining exploratory data analysis with appropriate model selection. Understanding customer behavior prior to modeling proved essential for building a reliable and effective churn prediction model.

```mermaid
flowchart LR
    A[Base de Clientes] --> B[Job de Scoring]
    B --> C[Tabela de Churn Scores]
    C --> D[Job de Integração]
    D --> E[CRM / Marketing]
```

