# About The Project

## END TO END MACHINE LEARNING PROJECT 

The objective of this machine learning model is to solve a classification problem. 

This machine learning project focuses on predicting software defects using a dataset of software complexity metrics. The dataset contains 22 features, including measures such as cyclomatic complexity, lines of code, Halstead metrics, and branch counts, which quantify the structural and logical attributes of code. The target variable, defects, indicates whether a code segment contains a defect (True,1) or not (False,0). The goal of this project is to build a predictive model to classify code as defective or non-defective based on these metrics.  The dataset I have picked for this purpose is from open ml. 

These are the following steps I have performed :

1. Loading the dataset into a database , normalizing it into 3NF form and fetching the data into a dataframe.
2. Exploring the data , split it into train and test data after stratifying
3. Used correlation matric and other metrics to analayze and explore the data
4. Cleaned the data by removing low varience features , removing highly correlated features , handled outliers in train and test data ,   normalized Nuemric features  
5. Initialized MLflow to track repo my "atluribhumika08/Code_Defect_Detection_Project"
6. Created a pipeline for preprocessing (StandardScaler, MinMaxScaler, LogTransformation, OneHotEncoding) and Logistic Regression. Logged the F1-score;TP,TN,FN,FP; and results in Mlflow on Dagshub.
7. Created a pipeline for preprocessing and used LogisticRegression, RidgeClassifier, RandomForestClassifier, and XGBClassifier.Logged the F1-score;TP,TN,FN,FP; and results in Mlflow on Dagshub.
8. Performed feature engineering and attribute combination on LogisticRegression, RidgeClassifier, RandomForestClassifier, and XGBClassifier.Logged the F1-score;TP,TN,FN,FP; and results in Mlflow on Dagshub.
9. Performed feature selection using Correlation Threshold, Feature Importance, and Variance Threshold on LogisticRegression, RidgeClassifier, RandomForestClassifier, and XGBClassifier.Logged the F1-score;TP,TN,FN,FP; and results in Mlflow on Dagshub.
10. Used PCA for dimensionality reduction on all the features. Created a scree plot to show which components will be selected for classification. Applied this on LogisticRegression, RandomForestClassifier, and XGBClassifier. Logged results in MLFlow on Dagshub.
11. Performed KNN on PCA reduced features.Logged results in MLFlow on Dagshub.
12. Performed SVM .Logged results in MLFlow on Dagshub.
13. Compared the F1 scores of models across all experiments 
14. Saved the final model using joblib as final_model.joblib.
15. Creatde a FastAPI application to serve the model.
16. Containerize the FastAPI application using Docker and pushed it to Docker Hub.
17. Deployed the containerized API to render.
18. Created a Streamlit app to interact with the deployed model for real-time classification.
