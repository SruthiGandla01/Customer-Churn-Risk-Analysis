# 🔁 Customer Churn Risk Analysis: Predicting Customer Attrition in Banking

This project focuses on predicting customer churn in the banking sector using machine learning models. By analyzing customer behavioral and demographic data, the framework identifies key indicators of churn and enables the development of proactive strategies to retain high-risk customers. The insights derived from this analysis can directly support tailored customer engagement and retention programs.

---

## **📚 Table of Contents**
- **Project Overview**  
- **Dataset**  
- **Libraries Used**  
- **Data Preprocessing**  
- **Exploratory Data Analysis (EDA)**  
- **Feature Engineering**  
- **Model Development & Evaluation**  
  - Logistic Regression  
  - Decision Tree  
  - Random Forest  
- **Results**  
- **Conclusion**  
- **Contributors**

---

## **📌 Project Overview**

Customer churn — the loss of clients or customers — is a critical KPI in banking and has direct revenue implications. This project aims to develop a predictive model that can anticipate customer churn using historical data and machine learning algorithms. By understanding why customers leave, banks can implement effective, data-driven retention strategies.

---

## **📊 Dataset**

The dataset used was obtained from Kaggle and includes information on 10,000 customers with 14 variables each. It covers both personal attributes and behavioral indicators relevant to churn prediction.

**Key Features Include:**
- `CreditScore`, `Age`, `Tenure`, `Balance`, `EstimatedSalary`
- `Geography`, `Gender`, `NumOfProducts`, `IsActiveMember`, `HasCrCard`
- `Exited`: Target variable (1 = churned, 0 = retained)

---

## **🧰 Libraries Used**
- **Pandas, NumPy** – Data handling and wrangling  
- **Matplotlib, Seaborn, Plotly** – Data visualization  
- **Scikit-learn** – ML models, metrics, pipelines  
- **Imbalanced-learn (SMOTE)** – Handling class imbalance  

---

## **🧹 Data Preprocessing**

To ensure model accuracy, data cleaning and preprocessing were performed:
- Dropped non-informative columns (`RowNumber`, `CustomerId`, `Surname`)
- Renamed the target column (`Exited` → `ChurnedOrNot`)
- Encoded categorical variables (One-Hot Encoding)
- Verified absence of null values and duplicates

---

## **📊 Exploratory Data Analysis (EDA)**

Visualizations revealed meaningful trends:
- **Age and Balance**: Older customers with higher balances were more likely to churn
- **Geography**: Churn rate varied significantly across regions
- **IsActiveMember**: Inactivity had a strong correlation with churn
- Charts used: Box plots, bar graphs, pie charts, correlation matrices

---

## **🏗️ Feature Engineering**

- Created new categorical bins for numerical features like `Balance` and `NumOfProducts`
- Simplified feature interpretation for models
- Feature distributions were compared across churn vs. non-churn segments

---

## **🤖 Model Development & Evaluation**

### **Logistic Regression**
- **Accuracy**: 72.05%  
- **F1 Score**: 0.7205  
- **AUC**: 0.76  
- Identified significant predictors like product usage and activity level

### **Decision Tree**
- **Training Accuracy**: 89.15%  
- **Testing Accuracy**: 83.4%  
- **F1 Score**: 0.834  
- Visualized decision paths and key splits

### **Random Forest**
- **Training Accuracy**: 90.61%  
- **Testing Accuracy**: 84.2%  
- **F1 Score**: 0.84  
- **AUC**: 0.86  
- Most robust model in terms of generalization and predictive power

---

## **✅ Results**

The Random Forest model delivered the best overall performance, achieving **84.2% test accuracy** and **AUC of 0.86**. It demonstrated excellent balance between sensitivity and specificity, making it well-suited for deployment in customer retention programs.

---

## **📌 Conclusion**

This project demonstrates the effectiveness of machine learning in identifying churn-prone customers in the banking sector. With actionable insights from models like Random Forest, institutions can focus efforts on customer engagement, thereby reducing attrition. Future work could explore deep learning models and real-time prediction systems for further improvement.

---

## **👥 Contributors**

- **Sruthi Gandla** – gandla.s@northeastern.edu  
- Aravind Swamy – swamy.ar@northeastern.edu  
- Jayasurya Jagadeesan – jegadeesan.j@northeastern.edu  
- Keshika Arunkumar – arunkumar.k@northeastern.edu  
- Samyuktha Kapoor – rajeshkapoor.s@northeastern.edu

