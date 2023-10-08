# Waze
#### Predicting Waze User Churn 
Waze Project - Google Advanced Data Analytics
## Overview
The goal of this project was to construct a logistic regression and XGBoost model to help Waze predict whether or not a user is retained or churned. The final XGBoost model had an accuracy score of 81.3% and a precision score of 43.1% in predicting the features that are most important in determining if a Waze user will be retained or churned. According to the model, the top three factors that had the most influence in determining if a user is retained or churned are kilometers per hour, number of days after onboarding, and percent sessions in the last month.
## Business Understanding
Waze is a mobile app created in 2009 that gives users driving directions while bringing a new approach to virtual maps (waze.com). User churn is when an indivudal stops using the service, in this case Waze, and Waze is seeking to reduce user churn.
## Data Understanding
This project uses synthetic data created for the Google Advanced Data Analytics course in partnership with Waze. This dataset contains 14,999 unique observations and 13 features. Features in this dataset include information about how much the user drove, how many times they used the app, the kind of device used, and if they were retained or churned. In this model, feature engineering was performed on multiple variables in the dataset to create new variables for modeling, and columns were dropped or reformatted to fit the model.
## Modeling and Evaluation
The final XGBoost model was used to determine feature importance in determining if a Waze user will be retained or churned. The final XGBoost model had 81.3% accuracy, and 41.3% precision. The following plot shows the features that were most important in separating a retained user from a churned user.

<img width="773" alt="Screenshot 2023-10-07 at 8 51 21 PM" src="https://github.com/allisonlmueller/Waze/assets/147258601/9f4c80f8-fbc6-4951-a35d-c76b5511cacc">

The XGBoost model relied heavily on engineered features, with three of the top five most important factors being engineered. 
## Conclusion
Overall, this model is not a good predictor of if a user will be churned or retained. It performed quite low on precision, recall, and F1, and when the model was fit to the data, it resulted in lower scores. I would not recommend this model for churn prediction; however, it could be improved by performing more feature engineering and having more information on user habits.
