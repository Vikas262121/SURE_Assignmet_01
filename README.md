# Customer Churn Prediction Using Machine Learning

## 📌 Project Overview

Customer churn is a major challenge for businesses that rely on long-term customer relationships. Identifying customers who are likely to discontinue a service helps organizations understand customer behavior and develop effective retention strategies.

This project implements a **Machine Learning-based Customer Churn Prediction system** using the Telco Customer Churn dataset. It explores customer demographics, subscribed services, contract details, and billing information to predict whether a customer is likely to leave the company.

The project also applies **GridSearchCV for hyperparameter tuning** to investigate whether optimizing model parameters can improve predictive performance. Model performance is evaluated using multiple classification metrics to provide a more comprehensive understanding of the results.

## 🎯 Project Objectives

- Analyze customer data and identify patterns associated with churn.
- Clean and preprocess the dataset for Machine Learning.
- Transform customer attributes into suitable numerical features.
- Develop a classification model to predict customer churn.
- Optimize model hyperparameters using GridSearchCV.
- Compare baseline and tuned model performance.
- Evaluate predictions using accuracy, precision, recall, F1-score, and a confusion matrix.
- Identify opportunities for improving churn detection and customer retention insights.

## 📊 Dataset

**Dataset:** Telco Customer Churn

**Source:** [Kaggle – Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

The dataset contains customer-level information, including:

- **Customer Demographics:** Gender, senior citizen status, and dependents.
- **Subscribed Services:** Internet service, phone service, online security, and other service features.
- **Account Information:** Contract type, payment method, and paperless billing.
- **Billing Details:** Monthly charges and total charges.
- **Target Variable:** `Churn`, indicating whether a customer has left the service.

The target variable is used to train a supervised classification model that distinguishes between customers who churn and those who remain.

## 🛠️ Technologies and Libraries

- **Python** – Core programming language
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical computations
- **Scikit-learn** – Model training, preprocessing, evaluation, and hyperparameter tuning
- **Matplotlib / Seaborn** – Data visualization, if used
- **Google Colab** – Cloud-based development environment
- **GridSearchCV** – Systematic hyperparameter search with cross-validation

## ⚙️ Project Workflow

### 1. Data Loading and Inspection
Load the Telco Customer Churn dataset and examine its structure, dimensions, column names, data types, and sample records.

### 2. Data Cleaning and Preprocessing
Inspect missing values, duplicate records, inconsistent data types, and potential data quality issues. Prepare the dataset for reliable model training.

### 3. Exploratory Data Analysis
Explore the distribution of churn and examine customer characteristics that may be associated with service cancellation, where applicable.

### 4. Feature Engineering and Preparation
Separate the input features from the target variable and convert categorical attributes into a machine-readable format. Apply appropriate preprocessing to prepare the features for classification.

### 5. Baseline Model Training
Train an initial classification model to establish a baseline for predictive performance.

### 6. Hyperparameter Tuning with GridSearchCV
Use GridSearchCV to evaluate selected hyperparameter combinations through cross-validation and identify the best-performing configuration within the specified search space.

### 7. Model Evaluation
Evaluate the original and tuned models using relevant classification metrics:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

These metrics help assess both overall correctness and the model's ability to identify customers who are likely to churn.

### 8. Performance Comparison
Compare the baseline and tuned models to determine whether hyperparameter optimization improves the selected evaluation metric and to identify areas for further improvement.

## 📈 Results and Performance Analysis

The experiment produced the following accuracy results:

| Model | Accuracy |
|---|---:|
| Original Classification Model | 73.81% |
| Hyperparameter-Tuned Model | 73.81% |

### Key Observations

- Both models achieved the same reported accuracy of **73.81%**.
- Hyperparameter tuning did not improve overall accuracy in this experiment.
- An unchanged accuracy score does not necessarily mean that tuning had no effect on other performance metrics.
- Further evaluation of recall, F1-score, ROC-AUC, and the confusion matrix can help determine whether the tuned model identifies churn customers more effectively.

**Important:** Accuracy alone is not sufficient to judge a churn prediction model. Since identifying customers who leave is a key objective, recall and precision for the churn class should also be considered.

## 🚀 How to Run the Project

1. Clone or download this repository.
2. Open the notebook in [Google Colab](https://colab.research.google.com/).
3. Download the Telco Customer Churn dataset from the Kaggle source linked above.
4. Upload the CSV file to your Colab environment.
5. Update the dataset file path in the notebook if required.
6. Execute the notebook cells sequentially.
7. Review the model evaluation metrics and compare the baseline and tuned results.

## 🔮 Future Enhancements

- Improve recall for the churn class while maintaining a reasonable precision level.
- Investigate class imbalance using appropriate resampling or class-weighting techniques.
- Experiment with alternative classifiers such as Random Forest, Support Vector Machine, and Gradient Boosting.
- Perform additional feature engineering to capture useful customer behavior patterns.
- Compare models using ROC-AUC and precision-recall metrics.
- Use stratified cross-validation and a separate test set for robust evaluation.
- Analyze feature importance to identify factors associated with customer churn.
- Develop an interactive application that accepts customer details and displays churn predictions.

## 💡 Key Learning Outcomes

Through this project, I explored the practical Machine Learning workflow, including data preprocessing, feature preparation, classification, hyperparameter optimization, and model evaluation.

The project also reinforced the importance of selecting appropriate evaluation metrics, interpreting experimental results, and understanding that hyperparameter tuning does not guarantee an improvement in every performance measure.

## 👨‍💻 Author

**vikas nath**

B.Tech –cse siml

Interested in Machine Learning, Artificial Intelligence, and data-driven problem-solving.

---

*This project was developed for educational purposes to explore supervised Machine Learning and hyperparameter optimization for customer churn prediction.*
