# Telco Customer Churn Analysis Dashboard

## Project Overview
This project analyzes the Telco Customer Churn dataset from Kaggle ([dataset link](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)) to identify patterns and factors that contribute to customer churn. The dashboard visualizes various dimensions affecting churn rates and provides insights into customer behavior.

You can view the interactive dashboard on Tableau Public ([here](https://public.tableau.com/views/Book1_17408627895420/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)).

## Development Process

### 1. Data Preparation
- Imported the Telco Customer Churn dataset from Kaggle
- Cleaned the data, handling missing values and standardizing formats
- Created calculated fields for analysis
  
### 2. Key Visualizations Created

#### Demographic Analysis
- **Churn by Gender**: Bar chart showing churn rates comparing female (26.92%) and male (26.16%) customers
- **Churn by Partner Status**: Bar chart comparing churn rates between customers without partners (32.96%) and with partners (19.66%)
- **Churn by Dependents Status**: Bar chart comparing churn rates between customers without dependents (31.28%) and with dependents (15.45%)
- **Churn by Senior Citizen Status**: Bar chart comparing churn rates between non-senior (23.61%) and senior citizens (41.68%)

#### Product Analysis
- **Churn Rate by Product Type**: Bar chart showing churn rates across different services:
  - Internet Service (31.83%)
  - Streaming Movies (29.11%)
  - Phone Service (26.71%)
  - Device Protection (22.50%)
  - Online Backup (21.53%)
  - Online Security (14.61%)
  - Streaming TV (11.56%)

#### Longitudinal Analysis
- **Churn Over Tenure**: Line chart showing the relationship between customer tenure (months) and churn rate, revealing significantly higher churn in the first few months

#### Contract and Service Analysis
- **Churn Rate by Contract and Internet Service**: Bubble chart visualizing the relationship between contract type, internet service type, and churn rate:
  - Month-to-month contracts show the highest churn (32.22% for DSL, 54.61% for fiber optic)
  - Two-year contracts show the lowest churn (1.91% for DSL, 7.23% for fiber optic)
  - Customers without internet service show varying churn rates based on contract length

#### Spending Pattern Analysis
- **Customer Spending Patterns by Churn Status**: Scatter plot showing the relationship between average monthly charges and average total charges, segmented by gender and contract type

### 3. Dashboard Design
- Created a cohesive layout with clear section headers
- Used a consistent color scheme with orange/amber tones on a dark background
- Added appropriate titles and labels for each visualization
- Included interactive filters for gender and contract type

## Key Insights and Analysis

1. **Contract Type Impact**: Month-to-month contracts show significantly higher churn rates (up to 54.61% with fiber optic) compared to one-year and two-year contracts. This suggests that longer-term commitments substantially reduce churn.

2. **Tenure Effect**: There is a strong negative correlation between customer tenure and churn probability. The first 12 months show the highest churn risk, with rates dropping dramatically after this period.

3. **Demographic Factors**:
   - Senior citizens have a much higher churn rate (41.68%) compared to non-seniors (23.61%)
   - Customers without partners (32.96%) or dependents (31.28%) are nearly twice as likely to churn as those with partners (19.66%) or dependents (15.45%)
   - Gender shows minimal impact on churn, with females (26.92%) showing only slightly higher churn than males (26.16%)

4. **Service Impact**:
   - Internet Service has the highest churn rate (31.83%)
   - Security-related services (Online Security, Online Backup) correlate with lower churn
   - Fiber optic internet shows higher churn than DSL across all contract types

5. **Spending Patterns**:
   - Month-to-month customers who churn tend to have higher monthly charges but lower total charges
   - Two-year contract customers show higher total spending and lower churn probabilities

## Recommendations

1. **Promote Long-term Contracts**: Develop compelling incentives for customers to sign one or two-year contracts instead of month-to-month agreements.

2. **Early Engagement Strategy**: Implement a specialized retention program focusing on the first 12 months of customer relationship when churn risk is highest.

3. **Target High-Risk Segments**: Create tailored retention strategies for senior citizens and customers without family attachments (no partners/dependents).

4. **Bundle Security Services**: Encourage adoption of security-related services which correlate with lower churn rates.

5. **Review Fiber Optic Offering**: Investigate the high churn rate among fiber optic customers to address potential issues with pricing, service quality, or expectations.

6. **Price Sensitivity Analysis**: Further analyze the relationship between monthly charges and churn rates to optimize pricing strategies, especially for the month-to-month segment.
