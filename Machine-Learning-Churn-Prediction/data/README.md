# 📊 Machine Learning: Telecommunication Customer Churn Prediction  

## 📺 Project Overview  
This project focuses on predicting customer churn in the telecom industry through a **comprehensive end-to-end machine learning workflow**, optimizing **model performance and interpretability**. The objective is to identify key factors influencing churn and develop a robust model to help telecom providers retain customers.  

### **Key Contributions:**  
- **Data Processing & Exploration:** Conducted thorough **data cleaning and exploratory data analysis (EDA)** to identify inconsistencies and key patterns.  
- **Machine Learning Pipeline:** Designed a **streamlined ML pipeline** for **automated data preparation, feature engineering, and leakage prevention**.  
- **Model Development & Optimization:** Implemented and fine-tuned **Gradient Boosting, Decision Trees, Random Forests, Logistic Regression, and Support Vector Machines (SVMs)**.  
- **Class Imbalance Handling:** Applied **SMOTE, Tomek Links, and class weight adjustments** to balance the dataset.  
- **Feature Engineering & Selection:** Performed **feature selection** and optimized class weights to enhance **model accuracy and generalization**.  
- **Ensemble Learning:** Explored **Voting Ensembles and Model Stacking** to improve predictive performance.  
- **Robust Evaluation:** Assessed models across **customer segments and data subsets** to ensure real-world applicability.  
- **Experiment Tracking & Reproducibility:** Utilized **MLflow** for logging, monitoring, and maintaining reproducibility.  

---

## 🛠️ Technologies & Libraries Used  
- **Python**  
- **Pandas, NumPy** → Data processing & analysis  
- **Matplotlib, Seaborn** → Data visualization  
- **Scikit-learn** → Machine learning models & evaluation  
- **Imbalanced-learn (SMOTE, Tomek Links, SMOTE-ENN)** → Class balancing  
- **MLflow** → Experiment tracking  
- **Statsmodels** → Statistical analysis  

---

## 📊 Key Insights & Findings  

### **1️⃣ Customer Behavior & Churn Trends**  
- **Senior citizens and customers without dependents or partners** were more likely to churn, highlighting the influence of **demographics** on customer retention.
- **Service-related factors** such as **fiber optic internet** and the absence of add-ons like **online security or tech support** were strongly associated with **higher churn rates**, suggesting dissatisfaction with the value or quality of services.
- **Contract and billing preferences** emerged as the strongest predictors:
- **Month-to-month contracts** and **electronic check payments** showed the **highest churn rates**.
- **Long-term contracts** and **automated billing methods** were linked to **greater retention**.

### **2️⃣ Model Performance & Challenges**  
- **Every base model struggled with recall for churned customers (class 'YES')**, likely due to **class imbalance**.
- **All models delivered decent precision (~70%) but struggled with recall (~48%).**
- **Feature selection slightly decreased performance**, meaning the models could work with a reduced feature set while maintaining predictive power.
- **Hyperparameter tuning (Grid Search) had little impact**, except for **Random Forest**, which saw a slight improvement.
- **Using class weights improved recall but reduced precision**, also degrading predictive power for **class 'NO'**.
- **Oversampling and undersampling increased recall but at the cost of precision**, except **Tomek Links**, which found the best balance.
- **Voting ensembles and stacking did not significantly improve metrics**, but Tomek Links achieved a slightly better recall-precision balance.

### **3️⃣ Best Model Selection**  
After extensive testing, the **best model for this dataset** is:  
#### ✅ **Logistic Regression with Tomek Links Undersampling**
- **Achieves ~80% accuracy** with a **balanced precision-recall (~60%)**.
- **Performs similarly to complex models** (Voting Ensembles & Stacking) but is **simpler, more interpretable, and computationally efficient**.
- **Avoids overfitting** and remains stable with new data.
- **Logistic Regression provides feature coefficients**, allowing **interpretability** and insights into what influences churn the most.

---

## **Data Sources:**
📂 **Kaggle:** [Telecom Customer Churn](https://www.kaggle.com/datasets/tarekmuhammed/telecom-customers/data)

---
## 📂 Dataset Information  

📂 **Dataset Location:** [`/data/`](https://github.com/AsenSirakov/Data-Science-Projects/tree/main/Machine-Learning-Churn-Prediction/data)
This project utilizes **telecom customer data** with features such as:
- **Demographics:** Age, gender, senior citizen status  
- **Service Details:** Internet type, contract type, additional services  
- **Billing Information:** Monthly charges, total charges, payment method  
- **Churn Status:** Whether a customer left the company or remained

---

## ▶️ How to Run the Project  

### **1. Clone the Repository**  
```bash
git clone https://github.com/AsenSirakov/Data-Science-Projects.git
cd Machine-Learning-Churn-Prediction
```

### **2. Open the Jupyter Notebook**  
Run the following command to start Jupyter Notebook:  
```bash
jupyter notebook Telecom_customer_churn.ipynb
```

### **3. Execute the Notebook**  
- Run all cells sequentially.  
- The notebook covers **data preprocessing, model training, evaluation, and visualization**.  

---
