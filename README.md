# ChurnPredictionProject
This is a ML project to predict churn of a telecom provider based on user data.

We have a file with user data like customerID, gender, tenure, contract type, etc. Our goal is to predict the customer churn based on this data. 
This is classification task as we only have to predict whether a customer left or not.

If you notice, the dataset is unbalanced. We have more rows with churn No as compared to Yes. 

We have tried various classification models - Logistic Regression, Decision Trees, Random Forest, Adaptive Boosting Classifier and Gradient Boosting Classifier.
We have to figure out what's the important parameter for us to judge or rate all models based on. 
Since our aim would be to reduce customer churn, it is important that we don't classify a customer who will churn as 0(will not churn) i.e. we need to avoid false negatives.
This can be done using Recall metric - how much the model correctly identifies as belonging to the “positive class”.
We have used accuracy and recall as our main metrics to identify that Logistic Regression with 'class weights' is the best model for this problem.

Note: I have also added a notebook from Pierian Data by Jose Portilla. He has done some excellent data analysis.
Thank you for your course on Udemy(Python for Machine Learning and Data Science Masterclass).
