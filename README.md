# Predicting Customer Churn at Syriatel Mobile Telecom using Machine Learning

![Telecom Mast](plots/telecom.jpg)

---

## Project Overview
The primary goal of any company is to maximize profit while minimizing losses, and a key factor in achieving this is ensuring customer satisfaction. Satisfied customers are more likely to remain loyal, which is crucial for business success. In the highly competitive telecom industry, maintaining customer satisfaction is paramount. This project aims to create a predictive model for customer churn, identifying behavior patterns that indicate a higher risk of customers leaving. 

---

## Business Understanding
SyriaTel, a mobile network provider based in Syria is keen to reduce losses that result from customers who don't stick around very long. The increase in customer churn is threatening the company's growth and profitability hence the need to assess customer behavior patterns and identify whatever factors may be contributing to the increase in customer churn. This will enable the company to create effective retention strategies that will not only increase customer satisfaction but also attract new customers to the company.

### Objectives
1 Create several machine learning models to predict customer churn by analyzing the key features within the data provided.

2 Identify the best pattern using classification metrics and identifyting what the key features contributing to customer churn in the company are.

3 Recommend cost-effective strategies that Syriatel can implement to help retain its customers thus reducing loss The primary stakeholder is Syriatel.

### Data Understanding
The data used in this project was sourced from Kaggle.

### Methodology
The following steps were taken to complete the project:
1. Data cleaning and Exploratory Data Analysis. 

2. Data Preprocessing involving the encoding of categorical values , scaling and handling class imbalance. Feature selection was also conducted to ensure those with greates impact on customer churn were included in the model

3. Model training and testing. Classification metrics were utilises to analyze model performance

4. Model Optimization. Models were optimized through hyperparameter tuning through the Gridsearch technique

5. Analyzing feature importance to identify features that had high influence on customer churn

---

## Model Evaluation
The metrics used to evaluate the performance of the models are Accuracy, Precision, Recall, F1-score and AUC ROC so as to select the best performing model. Below is a summary of how the various models performed:

### Baseline Model: Logistic Regression

 - **Accuracy:** Model's accuracy is  77.2% indicating the percentage of instances predicted correclty.
 
 - **Recall:** Model correctly identified 77% of the actual instances of class 0 and 76% of the actual instances of class 1.

 - **Precision:** The model accurately predicted 95% of instances for class 0, minimizing false positives, but it demonstrated a lower accuracy in predicting class 1, with a precision of 38%.
  
- **F1-Score:** The F1-Score for class 0 is 85%, indicating a good balance between precision and recall. However, for class 1, it is lower at 50%, suggesting a weaker balance between precision and recall for this class.

![image](plots/ROC%CurveforLogisticRegression.jpg)

### Decision Tree

 - **Accuracy:** Model's accuracy is  93.1% indicating the percentage of instances predicted correclty.
 
 - **Recall:** Model correctly identified 96% of the actual instances of class 0 and 79% of the actual instances of class 1. 

 - **Precision:** For class 0, the model accurately predicts 96% of instances, minimizing false positives. However, it demonstrates lower accuracy in predicting class 1, with a precision of 76%.
  
- **F1-Score:** The F1-Score for class 0 is 87%, indicating a good balance between precision and recall. In contrast, the F1-Score for class 1 is 93%, which also represents a strong balance between precision and recall for this class.

![image](plots/ROC%20Curve%20for%20Decision%20Tree%20Classifier.jpg)

### Random Forest

 - **Accuracy:** Model's accuracy is  94% indicating the percentage of instances predicted correclty.
 
 - **Recall:** Model correctly identified 96% of the actual instances of class 0 and 81% of the actual instances of class 1. 

 - **Precision:** For class 0, the model accurately predicts 97% of instances, minimizing false positives. However, it demonstrates lower accuracy in predicting class 1, with a precision of 80%.
  
- **F1-Score:** The F1-Score for class 0 is 97%, indicating a good balance between precision and recall. In contrast, the F1-Score for class 1 is 81%, which also represents a strong balance between precision and recall for this class.

![image](plots/ROC%20Curve%20for%20Random%20Forest%20Model.jpg)

The Random Forest performed better than the other models. It has the highest accuracy scores as well as the highest precicion, recall and f1 scores as well as the highest accuracy scores which means that it performs well in terms of overall correctness in classifying data points. Its high test set accuracy indicates that a significant portion of the test data points is correctly classified, making it a reliable choice for predicting outcomes.

### Feature Importance
![image](plots/ROC%20Curve%20for%20Random%20Forest%20Model.jpg)

Form the barchart we see that the top three features for predicting customer churn are:

**Total Day Minutes:** The total number of minutes the customer has been in calls during correlates with the charges. This means that if the company's charges are deemed to be too high by a customer then this may contribute to customer churn.

**Customer Service Calls:** The number of calls the customer has made to customer service correlates with customer satisfaction and therefore churn since the more a customer calls customer service the more likely it is that they may not be satified with the company's services.

**International Plan:** A customer having the international plan influences churn due to the difference in international calling rates. If the plans are too costly then customers may be dissatisfied resulting in increased churn.

### Conclusion 
The Random Forest performed better than the other models. It has the highest accuracy scores as well as the highest precicion, recall and f1 scores as well as the highest accuracy scores which means that it performs well in terms of overall correctness in classifying data points. Its high test set accuracy indicates that a significant portion of the test data points is correctly classified, making it a reliable choice for predicting outcomes.

### Recommendations
**Analyze Pricing and Improve Communication:** The company should conduct a pricing analysis to ensure that charges are competitive and aligned with customer expectations. 

**Customer Service Improvement:** To reduce churn, the company should invest in enhancing its customer service by providing prompt and effective solutions to customer issues. 
The company can also implement customer feedback surveys to help understand their satisfaction levels and expectations. 

**Optimize International Plan Options and Customer Retention Incentives:** Syriatel should consider diversifying its international plan offerings byintroducing more affordable international plans or flexible packages that cater to different customer needs. Customer retention strategies such as loyalty programs to reward long-standing customers will incentivize them to stay with the company.

** **Continuous monitoring and evaluation:** To ensure that each of these strategies are achieving optimum results 

By implementing these proactive strategies, SyriaTel will be able to cultivate a loyal customer base and effectively reduce the rates of churn thus ensuring the success of the company in the telecom industry.
