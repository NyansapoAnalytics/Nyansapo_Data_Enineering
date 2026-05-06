Telecom Customer Churn Prediction (PySpark ML Pipeline)

Overview:
This project is all about predicting customer churn in the telecom industry using PySpark, Spark SQL, and Machine Learning pipelines. We’re working with a dataset that includes 3,333 customer records and 21 features, such as call usage, charges, service plans, and customer service interactions. Our main goal? To pinpoint which customers are likely to leave and to grasp the key factors that drive their churn behaviour.

Dataset Description

The dataset is housed in HDFS (/gldata/Churn.csv, /gldata/Churntest.csv) and features elements like:
Account length, voicemail usage, call minutes, international plan, customer service calls, and churn status (0 = churner, 1 = non-churner).

Project Workflow
Initial Setup
- Chose the PySpark kernel in Jupyter Notebook
- Confirmed SparkContext is up and running
- Loaded the dataset from HDFS using Spark DataFrame
- Compared Spark DataFrame with Pandas DataFrame
- Familiarised myself with the Spark ML Pipeline structure

Data Processing & EDA
- Corrected data types (converted categorical data from integers)
- Checked for missing values and duplicates
- Cleaned and transformed features
- Conducted correlation analysis and selected features
- Created visualisations: histograms, count plots, and correlation heatmaps

Machine Learning Pipeline
- Used VectorAssembler for feature engineering
- Applied various models:
  - Logistic Regression
  - Decision Tree Classifier
  - Random Forest Classifier
  - Gradient Boosted Trees
- Trained and evaluated using a pipeline
- Metrics tracked: Accuracy, Precision, Recall, F1-score, ROC-AUC

Key Insight

We found that customer service calls, daytime usage, and international plans are strong predictors of churn behaviour. Among the models, ensemble methods like Gradient Boosting stood out as the most effective in identifying churners.

Author: Dr Emmanuel Dwamena Sasu
