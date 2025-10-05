# Telco Customer Churn Prediction

## 1. Overview and Goal

This project focuses on predicting customer churn for a telecommunications company. The main goal is to build a machine learning model that can accurately identify customers who are likely to leave the company. This enables the company to implement targeted retention strategies, reduce churn rates, and ultimately increase profitability by retaining valuable customers.

## 2. Technologies Used

-   Python
-   pandas (for data manipulation and analysis)
-   NumPy (for numerical operations)
-   Matplotlib and Seaborn (for data visualization)
-   Scikit-learn (for machine learning model building, evaluation, and preprocessing)
-   XGBoost (for the XGBoost classifier)

## 3. Methodology

The project follows a standard machine learning workflow:

-   **Data Loading and Exploration:** The telco customer data was loaded and explored to understand its structure, identify data types, and check for missing values.
-   **Data Preprocessing:** Missing values in 'TotalCharges' were handled by filling them with 0. Categorical variables were encoded using one-hot encoding and binary mapping. The 'customerID' column was dropped as it is not relevant for modeling.
-   **Feature Selection:** Based on correlation analysis with the target variable 'Churn', relevant features were selected for model training.
-   **Model Building and Evaluation:** Several classification models were trained and evaluated, including Logistic Regression, Random Forest, XGBoost, and Neural Network. Model performance was assessed using accuracy and classification reports.
-   **Model Optimization:** Hyperparameter tuning was performed on the best-performing model (Logistic Regression) using GridSearchCV to find the optimal parameters.
-   **Prediction:** The optimized model was used to predict churn probability for new data, and an optimal threshold was determined using the ROC curve to classify customers as likely to churn or not churn.

## 4. Results / Conclusion

The evaluation of the models showed that Logistic Regression performed slightly better than the other models based on accuracy. Hyperparameter tuning further optimized the Logistic Regression model. An optimal threshold was determined to balance precision and recall for predicting churn. The visualizations also provided insights into key factors influencing churn, such as Internet Service (Fiber optic), Payment Method (Electronic check), and Contract type (Month-to-month).

## 5. Feature Importance

Based on the correlation analysis and the selected features for the models, the following features showed significant importance in predicting churn:

-   Internet Service (particularly Fiber optic)
-   Payment Method (particularly Electronic check)
-   Contract Type (particularly Two-year contract)
-   Tenure

## 6. Business Value

This project provides significant business value by:

-   **Identifying High-Risk Customers:** Enabling the company to pinpoint customers likely to churn before they actually leave.
-   **Targeted Retention Efforts:** Allowing for the implementation of personalized retention strategies and offers to specific customer segments.
-   **Reducing Churn Rate:** Contributing directly to a lower customer churn rate, which is crucial for sustainable growth.
-   **Improving Customer Lifetime Value:** Retaining customers leads to increased revenue and a higher overall customer lifetime value.
-   **Optimizing Resource Allocation:** Focusing retention efforts on the most vulnerable customers optimizes marketing and customer service resources.

## 7. Next Steps & Contact

**Next Steps:**

-   Explore other feature engineering techniques.
-   Experiment with more advanced machine learning models.
-   Implement the model in a production environment for real-time predictions.
-   Develop a dashboard to visualize churn predictions and key metrics.
