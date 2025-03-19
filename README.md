# A/B Testing & Conversion Analysis

## Overview
This project analyzes an **A/B test** to evaluate whether a new webpage design improves conversion rates. We apply **statistical methods** and **machine learning models** to identify key factors influencing user conversions.

## Key Findings
✅ **The A/B test results do not support the full rollout of the new page**, as there is no significant difference in conversion rates.  
✅ **Country and time spent on the page have no significant effect on conversion**, suggesting the need for additional user behavior data.  
✅ **Machine learning models (Random Forest) struggled to predict conversions**, indicating that current variables are insufficient.  

##  Methodology
###  Data Cleaning & Exploration
- Removed inconsistent entries and checked data balance across experiment groups.  
- Examined key features: `group`, `country`, and `time_spent`.  

### A/B Testing (Statistical Analysis)
- Conducted **hypothesis testing** to compare conversion rates between the **control** and **treatment** groups.  
- Used **logistic regression** to assess the impact of `group`, `country`, and `time_spent` on conversion.  

###  Machine Learning Approach
- Implemented **Random Forest** to explore potential non-linear relationships.  
- Using `class_weight='balanced'` for class imbalance , but the model still struggled to predict conversions.  
