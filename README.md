# Providing Data-Driven Suggestions for Salifort Motors HR Using Machine Learning
This capstone project for Salifort Motors, focusing on providing data-driven suggestions for the Human Resources (HR) department. The project involves analyzing employee survey data to predict employee retention using machine learning models.

## 📑 Project Description

The HR department at Salifort Motors aims to improve employee satisfaction and reduce attrition. By analyzing a dataset of 15,000 employees with variables like job satisfaction, workload, salary, and promotions, this project builds predictive models to identify factors contributing to employee turnover.

### 🛠️ Project Goals
- Predict whether an employee will leave the company using a regression or machine learning model.
- Provide actionable insights to improve employee retention.
- Develop visualizations to support data-driven decisions.

## 🧬 Dataset

The dataset consists of 15,000 rows and 10 columns:
- `satisfaction_level`: Job satisfaction level [0–1]
- `last_evaluation`: Performance review score [0–1]
- `number_project`: Number of projects
- `average_monthly_hours`: Average work hours per month
- `years_at_company`: Tenure at the company
- `work_accident`: Work accident history (0/1)
- `left`: Whether the employee left the company (0/1)
- `promotion_last_5years`: Promotion history (0/1)
- `department`: Department of the employee
- `salary`: Employee's salary level (low/medium/high)

## 🔍 PACE Methodology

The project followed the PACE (Plan, Analyze, Construct, Execute) framework:

### Plan Stage
- **Understand the business scenario:** HR wants to reduce employee turnover.
- **Identify stakeholders:** HR department, senior leadership, and employees.
- **Define the problem:** What factors contribute to employees leaving the company?

### Analyze Stage
- **Performed EDA:** Explored relationships between variables and visualized data.
- **Initial Observations:**
  - 23.8% of employees left the company.
  - Lower satisfaction levels strongly correlated with attrition.
  - High workloads and low salary categories linked to higher turnover.

### Construct Stage
- **Modeling Techniques:**
  - Logistic Regression: Accuracy of 79.2%, AUC Score: 0.64
  - Random Forest Classifier: Accuracy of 99.1%, AUC Score: 0.98
  - Random Forest outperformed with higher accuracy and robustness.

### Execute Stage
- **Key Insights:**
  - Low satisfaction and high workload lead to higher attrition.
  - Lack of promotions and low salary contribute to turnover.
  - Sales and Technical departments have higher turnover rates.
- **Recommendations:**
  - Improve job satisfaction through surveys and initiatives.
  - Implement work-life balance strategies to prevent burnout.
  - Offer competitive salaries and clear promotion paths.

## 📊 Data Cleaning and Preprocessing
- Renamed columns to snake_case.
- Handled missing values and dropped 3,008 duplicate rows.
- Standardized numerical features for Logistic Regression.
- One-hot encoded categorical variables (e.g., salary levels).
- Addressed outliers in 'years_at_company' using IQR method.

## 📈 Data Visualization
- Countplots for employee retention by department and salary.
- Boxplots showing satisfaction levels by attrition status.
- Heatmap to visualize correlations between features.

## 🛠️ Tools & Libraries
- **Pandas, Numpy** - Data manipulation
- **Matplotlib, Seaborn** - Data visualization
- **Scikit-learn** - Machine learning models
- **Jupyter Notebook** - Interactive coding environment

## 🤝 Contributing
Feel free to fork this repository, create a branch, and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.


