# 🏦 Bank Customer Churn Prediction using Logistic Regression

## 📌 Project Overview

Customer retention is essential for the long-term success of any banking institution. Acquiring new customers is generally more expensive than retaining existing ones. Therefore, identifying customers who are likely to leave the bank is important for improving customer satisfaction and sustaining business growth.

This project aims to develop a **Logistic Regression classification model** to predict whether a customer of ABC Bank is likely to churn.

The project includes detailed Exploratory Data Analysis (EDA), data preprocessing, feature selection, model building, and evaluation using various performance metrics.

By identifying customers who are more likely to leave, ABC Bank can take proactive measures to improve customer retention.

---

## 🎯 Project Objectives

* Perform detailed Exploratory Data Analysis (EDA) on the bank customer churn dataset.
* Understand customer characteristics and identify patterns associated with churn.
* Identify relevant features that influence customer churn.
* Clean and preprocess the dataset for machine learning.
* Build a Logistic Regression model to predict customer churn.
* Evaluate the model using various classification performance metrics.
* Provide insights that can help ABC Bank improve customer retention.

---

## 📊 Dataset

**Dataset Name:** Bank Customer Churn Dataset

**Source:** Kaggle

🔗 [Download the dataset from Kaggle](https://www.kaggle.com/datasets/gauravtopre/bank-customer-churn-dataset)

The dataset contains customer-related information that can be used to analyze and predict customer churn.

### Target Variable

The target variable represents whether a customer has churned.

| Value | Description            |
| ----- | ---------------------- |
| 0     | Customer did not churn |
| 1     | Customer churned       |

*Note: Confirm the target column name and its encoding against the downloaded dataset before implementation.*

---

## 🛠️ Technologies Used

* **Python** – Programming language
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical computations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical data visualization
* **Scikit-learn** – Machine learning and model evaluation
* **Jupyter Notebook** – Development and experimentation

---

## 🔍 Exploratory Data Analysis (EDA)

Detailed EDA is performed to understand the dataset and discover patterns related to customer churn.

### 1. Data Understanding

* Display the first and last few records.
* Examine the dataset shape and column names.
* Identify numerical and categorical features.
* Check the data types of each column.

### 2. Data Cleaning

* Identify and handle missing values.
* Check for duplicate records.
* Examine inconsistent values and data formats.
* Identify unnecessary columns that do not contribute to prediction.

### 3. Univariate Analysis

Analyze individual features using:

* Histograms
* Count plots
* Box plots
* Distribution plots

### 4. Bivariate Analysis

Explore the relationship between customer churn and relevant features, such as:

* Customer age
* Account balance
* Credit score
* Number of bank products
* Customer activity status
* Tenure with the bank
* Geography
* Gender

*The final feature list will depend on the columns available in the dataset.*

### 5. Correlation Analysis

* Examine relationships between numerical variables.
* Generate a correlation heatmap.
* Identify potential multicollinearity among predictors.

### 6. Key Insights

Summarize the major patterns observed during EDA and identify features that may be useful for predicting customer churn.

---

## ⚙️ Data Preprocessing

The following preprocessing steps are considered before building the model:

1. Handle missing values, if present.
2. Remove duplicate records, if necessary.
3. Separate independent variables and the target variable.
4. Encode categorical variables using suitable encoding techniques.
5. Split the dataset into training and testing sets.
6. Apply feature scaling where appropriate.
7. Address class imbalance if the EDA indicates that it is necessary.

The preprocessing pipeline will be fitted using the training data to help prevent data leakage.

---

## 🤖 Model Building

### Logistic Regression

Logistic Regression is a supervised machine learning algorithm used for classification problems.

In this project, it is used to estimate the probability that a customer will churn based on their characteristics.

### Model Development Steps

1. Import the required libraries.
2. Prepare the independent and dependent variables.
3. Split the dataset into training and testing sets.
4. Encode categorical features and scale numerical features where appropriate.
5. Train the Logistic Regression model using the training data.
6. Generate predictions on the test dataset.
7. Evaluate the model using multiple performance metrics.

---

## 📈 Model Evaluation

The model is evaluated using the following classification metrics:

| Metric           | Description                                                                                                     |
| ---------------- | --------------------------------------------------------------------------------------------------------------- |
| Accuracy         | Measures the proportion of correct predictions.                                                                 |
| Precision        | Measures how many customers predicted as churners actually churned.                                             |
| Recall           | Measures how many actual churners were correctly identified.                                                    |
| F1-Score         | Represents the harmonic mean of precision and recall.                                                           |
| Confusion Matrix | Shows true positives, true negatives, false positives, and false negatives.                                     |
| ROC-AUC Score    | Measures the model's ability to distinguish between churners and non-churners across classification thresholds. |

### Why Multiple Metrics?

Accuracy alone may not provide a complete picture if the dataset contains significantly more non-churning customers than churning customers.

For ABC Bank, **recall and precision are particularly relevant**:

* Recall helps measure how many customers at risk of leaving are identified.
* Precision helps measure how many customers flagged as potential churners actually churn.

The choice of classification threshold should consider the costs of missed churners and unnecessary retention interventions.

---

## 💡 Business Applications

The predictions generated by this model may help ABC Bank:

* Identify customers who may be at risk of leaving.
* Develop targeted customer retention campaigns.
* Improve customer engagement and satisfaction.
* Prioritize retention efforts for customers identified as potentially at risk.
* Understand customer characteristics associated with churn.
* Support data-driven customer relationship management decisions.

**Important:** Model predictions should be treated as decision-support information rather than guarantees that a customer will leave.

---

## 📂 Project Structure

```text
Bank-Customer-Churn-Prediction/
│
├── data/
│   └── README.md
│
├── notebooks/
│   └── bank_customer_churn_prediction.ipynb
│
├── images/
│   └── eda_visualizations.png
│
├── README.md
└── requirements.txt
```

*The structure above is a suggested organization. Update the filenames to match the files actually included in your repository.*

---

## 🚀 How to Run the Project

### Step 1: Clone the Repository

```bash
git clone <your-repository-url>
```

### Step 2: Navigate to the Project Directory

```bash
cd Bank-Customer-Churn-Prediction
```

### Step 3: Install the Required Libraries

```bash
pip install -r requirements.txt
```

### Step 4: Download the Dataset

Download the dataset from Kaggle:

https://www.kaggle.com/datasets/gauravtopre/bank-customer-churn-dataset

Place the downloaded dataset in the appropriate directory and update the notebook's dataset path if necessary.

### Step 5: Run the Notebook

```bash
jupyter notebook
```

Open the notebook inside the `notebooks` directory and execute the cells sequentially.

---

## 📦 Requirements

The project uses the following Python libraries:

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

---

## 📋 Expected Outcomes

After completing the project, the following outcomes are expected:

* A detailed understanding of the bank customer churn dataset.
* Identification of important customer characteristics associated with churn.
* A trained Logistic Regression classification model.
* Evaluation of the model using multiple performance metrics.
* Business insights that may support customer retention strategies.

*Actual results, model performance scores, and feature importance findings should be added after running the analysis.*

---

## 🔮 Future Enhancements

Potential future improvements include:

* Comparing Logistic Regression with other classification algorithms.
* Applying hyperparameter tuning.
* Evaluating different classification thresholds.
* Investigating methods to handle class imbalance.
* Developing a simple web application to demonstrate churn predictions.
* Monitoring model performance as new customer data becomes available.

---

## 👩‍💻 Author

**Thameena M.**

B.Sc. Computer Science (Cyber Security)

PSGR Krishnammal College for Women

---

## 📜 License

This project is intended for educational and learning purposes. Check the dataset's licensing and usage terms before redistributing the dataset or using it for commercial purposes.
