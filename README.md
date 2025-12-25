# IBM HR Analytics - Employee Attrition Analysis

## 1. Objective

The goal of this analysis is to understand the key factors driving **employee attrition** in the organization. By identifying these drivers, HR can design targeted retention strategies to reduce turnover and improve employee satisfaction.

---

## 2. Data Overview

The dataset contains information about employees’ demographics, job roles, performance, and work environment. After careful examination, irrelevant or low-impact features were dropped to focus on variables most likely to influence attrition:

- Dropped columns: `EducationField`, `DailyRate`, `HourlyRate`, `MonthlyRate`, `Department`, `EmployeeCount`, `Over18`, `MaritalStatus`

---

## 3. Key Insights

### 3.1 Salary and Attrition
- Employees earning **0–5k** have a significantly higher attrition rate.  
- Implication: Low-compensation employees are at higher risk of leaving, highlighting the need for targeted compensation strategies.

### 3.2 Department & Role
- Employees from **HR and Sales**, particularly those in ground-level roles, exhibit higher attrition.  
- Suggests workload or job nature may influence turnover, and role-specific retention plans may be beneficial.

### 3.3 Travel Frequency
- Employees who **rarely or frequently travel** show elevated attrition rates, with **rare travel** showing slightly higher turnover.  
- Indicates travel patterns impact employee satisfaction differently depending on role or job expectations.

### 3.4 Gender
- **Male employees** have a higher attrition rate compared to females.  
- Suggests potential demographic trends or engagement differences that may need HR attention.

### 3.5 Job Level
- Attrition is **inversely proportional to Job Level**:
  - Low-level employees (JobLevel 1–2) with low **JobSatisfaction** have the highest attrition.
  - High-level employees (JobLevel 4–5) have very low attrition, likely due to seniority, higher compensation, and stronger organizational attachment.
- Recommendation: Retention efforts should **focus on early-career employees**.

### 3.6 Job Satisfaction
- Employees who stayed have similar JobSatisfaction levels across most groups, indicating consistent engagement among retained employees.

### 3.7 Work-Life Balance
- Attrition is **evenly spread** across WorkLifeBalance ratings, suggesting it may not be a strong predictor of turnover in this dataset.

### 3.8 Performance Rating & Overtime
- Employees with **mid-level PerformanceRating (3)** show a slight increase in attrition regardless of overtime.  
- Implication: Average performers may feel under-recognized; overtime contributes slightly but is not the dominant factor.

---

## 4. Feature Selection Decisions

- Dropped features due to low impact or redundancy:
  - `EducationField`  
  - `DailyRate`, `HourlyRate`, `MonthlyRate`  
  - `Department`, `EmployeeCount`, `Over18`, `MaritalStatus`

These decisions help focus the analysis on variables with actionable insights for HR decision-making.

---

## 5. Next Steps

1. **Statistical Validation**: Apply tests (Chi-square, t-tests, logistic regression) to confirm significance of insights.  
2. **Predictive Modeling**: Use the selected features to build a model predicting employee attrition.  
3. **Actionable Recommendations**: Translate insights into HR interventions, e.g., tailored retention strategies for low-level, low-salary, or high-travel employees.  
4. **Visualization**: Create charts to communicate findings to stakeholders effectively.

---

**Conclusion:**  

This analysis identifies the key drivers of employee attrition in the organization. Salary, job level, department, travel frequency, and performance are primary factors influencing turnover. HR interventions focused on **early-career, low-salary employees** and **role-specific engagement strategies** are likely to have the most significant impact on retention.
