# Analysis report 

The Amazon Customer Behavior Survey analysis delves into understanding the behaviours, preferences, and sentiments of customers engaging with Amazon's platform. Through a comprehensive exploration of various factors such as purchase frequency, product search methods, personalized recommendations, and satisfaction levels, this analysis aims to uncover insights that can inform business strategies, improve customer experiences, and drive growth. By statistical techniques, visualization tools, and exploratory data analysis, the analysis sheds light on patterns, correlations, and trends within the dataset, providing valuable insights for decision-making and optimization in the e-commerce domain. The dataset consists of 602 observations and contains information on purchase frequency and browsing frequency.
 For purchase frequency, the data is divided into five categories, with "Few times a month" being the most frequently occurring category, accounting for 203 observations. Similarly, browsing frequency is classified into four categories, with "Few times a week" being the most prevalent, representing 249 observations. 
These descriptive statistics provide an overview of the distribution of purchase and browsing habits among the surveyed individuals.


![Normality Test histogram](https://github.com/vinodhinidevaraj/amazon_customer_behavior_survey_analysis/assets/145280558/5e6da5da-292a-4154-abd9-afba74b9aed2)


![Q-Q plot](https://github.com/vinodhinidevaraj/amazon_customer_behavior_survey_analysis/assets/145280558/b3c4768a-1f21-4010-9f16-11c2b94ad7c2)


             
Additionally, the Anderson-Darling test was conducted to assess the normality of the dataset. The test results indicate that at various significance levels (15%, 10%, 5%, 2.5%, and 1%), the dataset is not normally distributed. 
This means that the data's distribution significantly deviates from a normal distribution.  As a result, parametric statistical tests that assume normality may not be appropriate for this dataset, and alternative non-parametric methods may be more suitable for analysis.

**Correlation analysis**

![Correlation Analysis](https://github.com/vinodhinidevaraj/amazon_customer_behavior_survey_analysis/assets/145280558/e6d384b1-4b35-4c17-b35c-95225e720440)


Among the variables listed in the correlation matrix, "Rating_Accuracy" has the strongest correlation with "Shopping_Satisfaction" (correlation coefficient = 0.514), indicating a moderate positive relationship. On the other hand, "age" has the weakest correlation with "Shopping_Satisfaction" (correlation coefficient = 0.0039), suggesting a negligible or very weak association between age and shopping satisfaction in this dataset.
The matrix indicates that customer satisfaction in the Amazon dataset is positively associated with the importance attributed to reviews, the frequency of personalized recommendations, and the accuracy of ratings. This suggests that customers who value reviews, receive personalized recommendations frequently, and perceive ratings as accurate tend to report higher levels of satisfaction with their shopping experiences on Amazon.

**Statistical model**


We performed a simple linear regression analysis to investigate the relationship between "Rating_Accuracy" and "Shopping_Satisfaction". The regression model yielded an R-squared value of 0.264, indicating that approximately 26.4% of the variance in shopping satisfaction can be explained by rating accuracy. The coefficient for "Rating_Accuracy" is 0.5782, suggesting that for every one-unit increase in rating accuracy, there is a corresponding increase of approximately 0.5782 units in shopping satisfaction. This coefficient is statistically significant (p < 0.001), indicating a strong positive relationship between rating accuracy and shopping satisfaction. Additionally, the intercept term (const) is 0.9181, indicating the expected shopping satisfaction score when the rating accuracy is zero. Overall, the regression model provides evidence of a significant and positive association between rating accuracy and shopping satisfaction.

**Exploratory Analysis**

![Distibution of the variables](https://github.com/vinodhinidevaraj/amazon_customer_behavior_survey_analysis/assets/145280558/f49a61d2-bb89-4d58-b3d2-a16ce5315f5b)

In this section, we conducted exploratory data analysis (EDA) using histogram plots to delve into key aspects of customer behaviour from the Amazon Customer Behavior Survey dataset. We examined "Purchase Frequency" to reveal that most customers make purchases a few times a month, while "Purchase Categories" analysis unveiled the most popular product categories. We visualized the significance of "Customer Reviews" and the frequency of "Personalized Recommendations" to understand their impact on customer behaviour. Furthermore, we assessed "Shopping Satisfaction" and "Service Appreciation" distributions to gauge customer contentment levels. These insights can guide strategic decisions and enhance customer satisfaction initiatives.


**Customer Segmentation using K-means Clustering**
                   

![K-means Clustering](https://github.com/vinodhinidevaraj/amazon_customer_behavior_survey_analysis/assets/145280558/342612b9-9985-4995-ac4c-ce871eeafea4)


                      
we applied K-means clustering to segment customers based on their behaviour using three key features: "Purchase Frequency," "Customer Reviews Importance," and "Shopping Satisfaction." The clustering process identified distinct groups of customers exhibiting similar behaviour patterns. The cluster centres represent the average values of each feature within each cluster. The cluster counts indicate the number of customers assigned to each cluster. By visualizing the clusters, we can observe the distribution of customers across different behaviour segments. This segmentation enables businesses to better understand their customer base and tailor marketing strategies and services to meet the specific needs and preferences of each cluster.



**Analysis of Popular Purchase Categories by Age Group**


![Purchase Frequency by gender and age](https://github.com/vinodhinidevaraj/amazon_customer_behavior_survey_analysis/assets/145280558/29df9409-baea-4578-b56c-b2d408c32506)

 
In this analysis, we explored the most popular purchase categories within different age groups using the Amazon Customer Behavior Survey dataset. By grouping the data based on age group and purchase category, we counted the occurrences of each purchase category. The results revealed insightful patterns: among individuals under 18, "Clothing and Fashion; others" was the most popular category, while for the age group 18-35, "Clothing and Fashion" dominated with a considerable count of 83. Interestingly, the age group 36-55 showed a preference for "Beauty and Personal Care," with 23 occurrences, while individuals aged 56 and above also leaned towards "Beauty and Personal Care," albeit with a lower count of 5. Notably, the age group 18-35 emerged as the demographic with the maximum number of purchases, reinforcing the significance of understanding consumer behaviour within this cohort for targeted marketing strategies and product offerings.

**Conclusion**
The analysis of maximum shopping by gender in each age category reveals intriguing patterns that offer valuable insights into consumer behaviour within the dataset. Particularly, females aged 18-35 exhibit a notable presence across various purchase frequencies, indicating a strong engagement with Amazon's offerings. This demographic segment appears to be actively involved in shopping activities, with significant proportions of shopping less than once a month, once a month, and a few times a month. On the other hand, females under 18 predominantly engage in shopping activities a few times a week, suggesting a higher frequency of purchase behaviour among younger female consumers. The findings underscore the importance of understanding demographic differences in consumer behaviour, especially in the context of e-commerce platforms like Amazon. Such insights can inform targeted marketing strategies, product recommendations, and personalized experiences tailored to specific demographic segments. By recognizing and leveraging these patterns, businesses can optimize their approach to customer engagement and drive greater customer satisfaction and loyalty.

