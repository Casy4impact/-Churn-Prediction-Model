# -Churn-Prediction-Model
# Project Problem Overview:
Waze, as a community-based navigation app, faces a critical challenge with user churn. The app’s success relies on consistent user engagement and retention, but the company is experiencing a significant number of users either uninstalling the app or discontinuing its use. This attrition threatens not only user numbers but also potentially impacts revenue and the quality of service provided. To address this, Waze aims to implement a Churn Prediction Model to anticipate user behavior and proactively intervene to retain users at risk of churn.
# Objectives of the Project:
1.	Churn Prediction Model Development: Develop a robust machine learning model that accurately predicts and identifies users at risk of churning. This model will be the cornerstone for proactive intervention strategies.
2.	Enhanced User Retention: Utilize the insights from the churn prediction model to implement targeted strategies to retain at-risk users. This might involve tailored features, engagement campaigns, or incentivization.
3.	Data-Driven Decision Making: Provide Waze leadership with data-informed recommendations and actionable insights to make informed decisions, enabling them to take proactive steps in managing user retention.
4.	Identify Engaging Factors: Analyze user behavior and patterns to identify the key factors that influence user engagement and satisfaction. This insight will guide feature development and strategic decisions to enhance user experience and reduce churn.
# Project Overview/Description:
Project Title: Churn Prediction Model
Waze, a globally used navigation application, recognizes the significance of user churn and its implications for the sustainability and growth of the platform. The Churn Prediction Model project aims to leverage machine learning and predictive analytics to develop a solution that accurately anticipates user churn. By analyzing user data, the project seeks to identify patterns and signals indicative of potential churn. This data will empower Waze to take proactive measures to retain users at risk and enhance the overall user experience.
The project will involve an in-depth analysis of historical user behavior, app usage patterns, and various factors contributing to user churn. Utilizing this analysis, a predictive model will be developed to forecast potential churn, enabling Waze to intervene before users disengage from the platform. This intervention will include tailored strategies designed to re-engage and retain users who show signs of leaving the platform.
Ultimately, the Churn Prediction Model project aims not only to reduce user attrition but also to foster a more data-driven and proactive approach to user retention strategies within Waze. By empowering leadership with insights derived from data analysis, the project will guide strategic decisions and actions to enhance user satisfaction, drive engagement, and sustain the growth of the platform.

### Below are the predictor variables arranged in order of their predictive power
1.	n_days_after_onboarding: The number of days since a user sign up for the app
2.	activity_days: Number of days the user opens the app during the month   
3.	duration_minutes_drives: Total duration driven in minutes during the month
4.	total_sessions: A model estimate of the total number of sessions since a user has onboarded. 
5.	Driven_km_drives: Total kilometers driven during the month
6.	total_navigations_fav1: Total navigations since onboarding to the user’s favorite place 1
7.	driving_days: Number of days the user drives (at least 1 km) during the month
8.	sessions: Number of occurrences of users opening the app during the month 
9.	drives: An occurrence of driving at least 1 km during the month   
10.	total_navigations_fav2: Total navigations since onboarding to the user’s favorite place 2  
11.	device_iPhone: iPhone mobile phone device used to access the app by the user


# Interpret and compare the 3 models
The classification reports provide a comprehensive evaluation of the performance of three different models (Logistic Regression, Decision Tree, and Gradient Boosting) on a binary classification task. Here's an interpretation and comparison of the results:

# Logistic Regression Model:
- Precision: Precision for the 'churned' class is low (0.52), indicating that when the model predicts a customer will churn, it is correct about 52% of the time. On the other hand, the precision for the 'retained' class is high (0.83).
- Recall: Recall for the 'churned' class is very low (0.07), suggesting that the model misses a significant number of actual churned customers. However, recall for the 'retained' class is high (0.99), indicating that the model effectively captures the majority of retained customers.
- F1-Score: The F1-score is a harmonic mean of precision and recall. The F1-score for 'churned' is low (0.12), reflecting the trade-off between precision and recall. The F1-score for 'retained' is high (0.90), indicating a good balance between precision and recall.
- Accuracy: Overall accuracy is 82%, meaning the model correctly predicts the class for 82% of instances.
# Decision Tree Model:
- Precision: Precision for the 'churned' class is relatively low (0.27), and precision for the 'retained' class is high (0.84).
- Recall: Recall for both classes is similar, with 'churned' at 0.28 and 'retained' at 0.84.
- F1-Score: The F1-score for 'churned' is moderate (0.28), and for 'retained' is high (0.84).
- Accuracy: Overall accuracy is 73%, which is lower than the Logistic Regression model.
# Gradient Boosting Model:
- Precision: Precision for the 'churned' class is similar to Logistic Regression (0.52), and precision for the 'retained' class is high (0.83).
- Recall: Recall for 'churned' is low (0.08), similar to Logistic Regression, while recall for 'retained' is high (0.98), similar to the Logistic Regression model.
- F1-Score: The F1-score for 'churned' is low (0.13), and for 'retained' is high (0.90).
- Accuracy: Overall accuracy is 82%, matching the Logistic Regression model.
# Comparison:
- The Decision Tree model generally performs the worst, with lower precision, recall, and accuracy compared to Logistic Regression and Gradient Boosting.
- Logistic Regression and Gradient Boosting models show similar performance, with high precision and recall for the 'retained' class and lower values for the 'churned' class.
- Accuracy is higher for Logistic Regression and Gradient Boosting compared to the Decision Tree.
# Business Recommendations and Conclusions:
If the goal is to prioritize precision for predicting customer churn, further tuning and evaluation may be necessary, as both Logistic Regression and Gradient Boosting models have relatively low precision for the 'churned' class.
The Decision Tree model might need improvement, and its overall lower accuracy suggests it may not be the best choice for this specific task.
### Logistic Regression is the best Performing model. It has been productionised
