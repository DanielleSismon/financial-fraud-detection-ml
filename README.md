# Financial Fraud Detection using Machine Learning

### 📌 Project Overview 

This project builds a Machine Learning model to detect fraudulent financial transactions within a highly imbalanced dataset context (only 0.1% of transactions are actual fraud).
The primary goal was not just classification accuracy, but maximizing Recall (the ability to detect actual fraud), prioritizing financial security and loss prevention over minimizing false positives.

### 💼 Business Problem

In banking transactions, the cost of missing a fraudulent transaction (False Negative) is significantly higher than blocking a legitimate one (False Positive). Therefore, traditional models focused solely on Accuracy are inefficient and risky for this scenario.
Challenge: How to make a model "learn" the fraud pattern with extremely limited examples?

### 🛠️ Tech Stack

-	Language: Python
-	Data Manipulation: Pandas, NumPy
-	Visualization: Matplotlib, Seaborn
-	Machine Learning: Scikit-learn
-	Advanced Techniques: One-Hot Encoding, StandardScaler, RandomUnderSampler (Balancing).

### 🚀 Methodology

1.	Exploratory Data Analysis (EDA): Identified extreme class imbalance (99.9% legitimate vs. 0.1% fraud) and correlation analysis.
2.	Preprocessing:
	Removal of ID columns (noise).
	Transformation of categorical variables (type) using One-Hot Encoding.
	Feature Scaling (StandardScaler) to ensure algorithm performance.
3.	Data Balancing: Applied Random Under Sampling to create a balanced training dataset (50/50), enabling the model to effectively learn fraud patterns.
4.	Modeling: Training and comparison of two algorithms:
	Logistic Regression
	Decision Tree

### 📊 Results & Business Impact

The Decision Tree model outperformed Logistic Regression on business-critical metrics.
Metric	Result (Decision Tree)	Business Meaning
Recall (Fraud)	82%	The model detects 4 out of every 5 actual fraud attempts.
Precision	9%	We accept a higher volume of alerts to guarantee security.
Conclusion: The model is highly effective in shielding the system against financial losses, meeting the institution's security objectives.

### 📂 Repository Structure
-	fraud_detection_analysis.ipynb: The Jupyter Notebook containing all code, analysis, and visualizations.
-	Fraud.csv: ([Link to original Kaggle source due to file size](https://www.kaggle.com/datasets/parthaade/fraud-analysis)).

### 👩‍💻 Author
Danielle Sismon
-	LinkedIn: https://www.linkedin.com/in/danielle-sismon
-	Software Development Student (Fatec) focused on Data Engineering and AI. 
