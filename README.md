**INTRODUCTION**

In the fiercely competitive landscape of the banking industry, retaining existing customers is just as crucial as acquiring new ones. Customer churn, or the rate at which customers discontinue their services, is a key metric that directly impacts a bank's profitability. We delve into customer churn prediction, leveraging a comprehensive dataset encompassing a wide array of customer attributes.

Our primary goal is to build a predictive model that accurately identifies customers who are at risk of churning. We leverage machine learning techniques to provide the bank with actionable insights to engage with potentially at-risk customers proactively.

**RESEARCH METHODOLOGY**

In this paper, we adopt the CRISP-DM (Cross-Industry Standard Process for Data Mining) Framework, widely regarded as the most favored methodology in the data mining domain. By adhering to CRISP-DM, we aim to uncover interesting patterns and insights from the data systematically.

**Data Preparation and Visualization**

*(a) Correlation matrix analysis.*

Figure 2 depicts the correlation matrix, revealing that no pair of variables exhibits a strong correlation. This observation is crucial as it satisfies the fundamental assumption of modelling, namely the absence of multicollinearity. However, a notable correlation was observed between the number of products and balance. 
![image](https://github.com/user-attachments/assets/51e65f6c-7ed1-456a-bda8-d8e722892d35)

*b) Analysis Based on Balance, Age, Credit Score, and Tenure*

Our investigation reveals that customers who maintain a balance exceeding $85,000 are more likely to churn. Notably, customers aged between 30 and 50 appear to be primary contributors to this trend. Conversely, customers possessing two or more products the bank offers exhibit notably reduced likelihood of leaving. Interestingly, numerical factors such as credit scores and tenure do not significantly impact the customer attrition rate.
![image](https://github.com/user-attachments/assets/62e0903c-2cca-496a-9c7d-d409322bae8d)

Fig 3 showcases a scatterplot illustrating the relationship between credit scores and customer churn. Notably, all churned customers (orange dots) possess credit scores below 400. This suggests that customers with poor credit histories are more prone to leaving the bank. The clustering of churned customers below the credit score threshold of 400 underscores the potential influence of weak economic statuses on customer attrition.
![image](https://github.com/user-attachments/assets/8f136164-b912-4450-9c93-73ae72d0256b)

*(c) Gender, active members, credit cards and country-based analysis.*

We found that 45.4% of female customers churned, while 898 male customers churned out of a total of 5,457 (approximately 16%). Male account for 54.6% of all churning customers. The attrition rate among inactive customers is nearly double that of active customers (27% for inactive compared to 14% for active). Among the countries, France exhibits the highest customer churn rate at 50.1%, followed by Germany at 25.1%, and Spain at 24.8%
![image](https://github.com/user-attachments/assets/5a9c0646-bb3c-46b6-89ed-53abd931c4f2)

**RESULTS AND DISCUSSION**

The evaluation presented in Table 2 highlights the performance of different models in predicting churn, with a focus on sensitivity and accuracy as the most relevant metrics. 
Model Performance:
Random Forest achieved the highest accuracy at 99%, closely followed by KNN at 71.1%. Similarly, Random Forest outperformed KNN in terms of F1 score, specificity, and AUC, indicating its overall superior performance across multiple metrics.
Sensitivity and Accuracy:
Random Forest exhibited the highest sensitivity at 100%, indicating its ability to correctly identify churned customers. KNN followed with a sensitivity of 73.7%.
Since sensitivity and accuracy are considered the most relevant metrics for predicting churn, Random Forest emerges as the preferred choice due to its strong performance in both metrics.
In conclusion, based on the evaluation and considering the importance of sensitivity and accuracy in predicting churn, Random Forest emerges as the preferred choice due to its excellent performance across these key metrics. Random Forest not only demonstrated high sensitivity and accuracy but also excels in handling large datasets with many variables. This scalability makes it well-suited for real-world applications where data volume and complexity are significant.
![image](https://github.com/user-attachments/assets/b8bf5d03-de7b-4e76-bcbb-4980e1f43b27)
