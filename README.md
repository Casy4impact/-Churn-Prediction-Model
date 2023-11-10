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

## Below are the predictor variables arranged in order of their predictive power
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
