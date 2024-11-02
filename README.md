# Customer-Churn-Analysis-Insights-Predictive-Modeling

# Customer Churn Analysis

This repository contains a detailed analysis of customer churn for an organization, focused on identifying patterns and factors associated with churn. Customer churn is a critical issue that impacts business profitability, and understanding its causes can aid in devising strategies to improve customer retention. In this analysis, we examine demographic and behavioral factors linked to customer churn, using descriptive statistics and visualizations to highlight key insights. In a future update, a predictive model will be introduced to anticipate churn risk, allowing for proactive customer retention measures.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Information](#dataset-information)
- [Data Preparation](#data-preparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Key Insights](#key-insights)
- [Future Work](#future-work)
- [Getting Started](#getting-started)
- [License](#license)

---

## Project Overview
This project investigates customer churn to provide insights into customer behavior and factors influencing churn. The main objectives of this analysis are:
1. To understand the proportion of customers who have churned.
2. To identify characteristics and service features associated with higher churn.
3. To set the foundation for a predictive model to forecast which customers are at risk of churning.

Our initial findings suggest significant trends that can inform retention strategies, while further analyses and modeling will refine these insights.

## Dataset Information
The dataset, `Customer Churn.csv`, includes the following information:
- **CustomerID**: Unique identifier for each customer.
- **Demographics**: Information on customer characteristics, such as whether they are senior citizens.
- **Account Information**: Tenure, monthly charges, and total charges.
- **Service Details**: Types of services used (e.g., internet service, phone service).
- **Churn Status**: Indicates whether the customer has churned.

### Key Variables Analyzed
1. **Demographic Variables**: Age, gender, senior citizen status.
2. **Account Tenure**: Duration of the customer’s subscription with the company.
3. **Charges**: Monthly charges and total charges.
4. **Services**: Types of services subscribed (e.g., internet, phone).

## Data Preparation
Several preprocessing steps were taken to ensure data consistency and accuracy:
1. **Data Cleaning**:
   - Replaced empty values in `TotalCharges` with "0" and converted it to `float` for consistency in calculations.
   - Checked and removed duplicate entries to maintain data quality.

2. **Feature Engineering**:
   - Converted the `SeniorCitizen` column from binary (0 and 1) to categorical values ("Yes" and "No") for better readability in analyses.

3. **Handling Missing Values**:
   - Verified that there are no missing values that would affect subsequent analysis.

## Exploratory Data Analysis (EDA)
The EDA phase involved analyzing the overall distribution and characteristics of churned vs. non-churned customers through visualizations and descriptive statistics.

### Churn Distribution
- **Objective**: To understand the overall churn rate.
- **Method**: Created bar and pie charts to visualize churned and non-churned customers.
- **Result**: 
  - Approximately **26.54%** of customers have churned. This relatively high rate signals the need to investigate factors driving churn to inform retention strategies.

### Demographic Analysis
- **Senior Citizen Analysis**: Examined if senior citizens are more likely to churn.
- **Service Usage Patterns**: Analyzed if churn rates vary significantly based on service type (e.g., customers with internet service vs. without).
  
### Service and Financial Factors
- **Monthly Charges and Total Charges**:
  - Investigated the correlation between monthly/total charges and churn.
  - Initial findings suggest that customers with higher monthly charges may have a slightly higher tendency to churn.
  
- **Tenure**:
  - Analyzed the relationship between customer tenure and churn, with early findings indicating that customers with shorter tenure have higher churn rates, which may suggest an issue with early retention.

## Key Insights
Based on the exploratory data analysis, several key insights were identified:

1. **Churn Rate**:
   - **26.54%** of the customers have churned, highlighting the need for targeted retention efforts.

2. **Demographic Factors**:
   - Preliminary results indicate that certain demographics, such as senior citizen status, may have a relationship with churn rates. For example, senior citizens may churn at different rates compared to other age groups.

3. **Financial and Service Patterns**:
   - **Monthly Charges**: Customers with higher monthly charges tend to show a slight increase in churn likelihood.
   - **Tenure**: Churn is more common among customers with shorter tenure, suggesting potential improvements in initial customer experience or engagement could help retain new customers longer.

4. **Service Types**:
   - Customers who subscribe to multiple services (e.g., both phone and internet) may exhibit different churn patterns compared to those with a single service, although further analysis is needed.

## Future Work
Future analysis will involve building a predictive model to forecast customer churn. The model will use a combination of demographic, account, and service variables to identify customers with a high likelihood of churning, enabling proactive retention strategies. Planned steps include:
1. Feature selection and engineering to enhance model accuracy.
2. Model training and validation using techniques like logistic regression, decision trees, or more advanced machine learning models.
3. Assessment of model performance and tuning for deployment readiness.

## Getting Started
To replicate or extend this analysis, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/UdayKiranVanapallio/Customer-Churn-Analysis-Insights-Predictive-Modeling.git

This `README.md` structure summarizes the current analysis and highlights the main insights while also outlining the next steps for predictive modeling. Let me know if you'd like further customization!
