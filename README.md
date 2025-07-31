# IBM HR Analytics: Employee Attrition Prediction and Analysis

## Project Overview

Employee attrition presents a significant challenge for organizations, leading to the loss of talent, increased recruitment costs, and operational disruptions. This project analyzes IBM's HR dataset to identify key factors influencing employee attrition and develops predictive models to classify employees at risk of leaving. The objective is to assist HR teams in making data-driven decisions for talent retention and workforce planning.

---

## Tools and Technologies

- **Language**: Python  
- **Libraries**:  
  - pandas, numpy – Data manipulation  
  - matplotlib, seaborn – Data visualization  
  - scikit-learn – Machine learning (Random Forest, Logistic Regression, Decision Trees, GridSearchCV)  
  - imbalanced-learn – SMOTE for handling class imbalance  
  - LIME – Model explainability  
- **Business Intelligence**: Power BI  
- **Dataset Source**: [IBM HR Analytics Dataset on Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)

---

## Process Breakdown

### 1. Exploratory Data Analysis (EDA)

- Dataset: 1,470 employees with 35 features  
- Target Variable: `Attrition` (Yes/No) — imbalanced with 237 "Yes" and 1,233 "No"  
- Key Insights:  
  - Higher attrition among employees with lower job satisfaction, poor work-life balance, and extended overtime  
  - Roles with limited career growth and lower income showed greater attrition  
- Visualizations: Histograms, boxplots, bar charts, correlation heatmaps

### 2. Data Preparation and Feature Engineering

- Encoded categorical variables using label encoding and one-hot encoding  
- Normalized continuous variables using StandardScaler  
- Applied SMOTE to balance the class distribution of the target variable  

### 3. Model Development and Evaluation

- Algorithms evaluated:  
  - Logistic Regression  
  - Decision Tree  
  - Random Forest Classifier (selected for final deployment)  
- Hyperparameter tuning with GridSearchCV  
- Evaluation metrics:  
  - Confusion Matrix  
  - Classification Report (Precision, Recall, F1-Score)  
  - ROC-AUC Score  
- Model interpretability using LIME to explain individual predictions  

### 4. Visualization and Reporting

- Power BI dashboards highlighting attrition trends by department, job role, and income  
- Python plots for feature importance, correlation, and model performance  
- LIME visualizations to provide local explanations for specific employee attrition predictions  

---

## Outcome and Impact

### Key Insights

1. Overtime: Employees working overtime were 30 percent more likely to leave  
2. Job Satisfaction: Low job satisfaction doubled the likelihood of attrition  
3. Work-Life Balance: Poor balance increased attrition risk by 2.5 times  
4. Age Range: Employees aged 25 to 35 showed the highest attrition rates  

### Strategic Recommendations

- Revise overtime policies and workload distribution  
- Enhance career development opportunities for roles with limited growth  
- Develop targeted retention programs for early-career professionals  
- Use predictive models to proactively identify high-risk employees  

### Business Impact

- Estimated 20 percent reduction in hiring and onboarding costs  
- Improved employee engagement through targeted HR programs  
- Strengthened HR decision-making using interpretable machine learning insights  

---

## Summary and Key Takeaways

This project demonstrates the value of using machine learning, data visualization, and model explainability to address workforce attrition. By identifying critical factors contributing to employee turnover and deploying predictive models, organizations can make proactive and informed HR decisions. The approach is scalable and adaptable for real-world business environments.

---

