
# SaaS Customer Churn Analysis

Comprehensive churn analysis for a fictional SaaS company using real-world styled data. This project applies logistic regression and random forest models to predict customer churn, supported by exploratory analysis, feature engineering, and visualization. Key performance metrics, model comparisons, and business recommendations are included to inform customer retention strategies.

---

## Purpose

This project aims to identify drivers of customer churn and build predictive models that enable proactive retention efforts. The analysis combines rigorous data preprocessing, interpretable modeling, and visual storytelling to demonstrate how machine learning can be applied in a SaaS business setting.

---

## Dataset Overview

- **customer_churn_dataset-training-master.csv**: Training data for model development  
- **customer_churn_dataset-testing-master.csv**: Holdout test set for validation

---

## Tech Stack

- **Python** (pandas, matplotlib, seaborn, scikit-learn)  
- **Jupyter Notebook** (EDA, modeling, visualization)  
- **GitHub Pages + Jekyll** (Portfolio publishing)

---

## Key Questions Answered

### 1. What features best predict whether a SaaS customer will churn?
### 2. Can we build an interpretable, accurate model to identify at-risk customers?
### 3. How do customer behaviors (e.g. support calls, payment delays, tenure) relate to churn likelihood?

---

## Featured Visualizations

### Churn by Subscription Type
- ![Subscription Type](assets/images/ChurnBySubscriptionType.png)

### Churn by Contract Length
- ![Contract Length](assets/images/ChurnByContractLength.png)

### Tenure by Churn Status (Boxplot)
- ![Tenure Boxplot](assets/images/TenureBoxplot.png)

### Support Calls by Churn Status
- ![Support Calls](assets/images/SupportCallsBoxplot.png)

### Last Interaction by Churn Status
- ![Last Interaction](assets/images/LastInteractionBoxplot.png)

### ROC Curve - Logistic Regression vs. Random Forest
- ![ROC Curve](assets/images/ROC_LR_RF_Comparison.png)

### ROC Curve - Logistic Regression vs. Tuned Random Forest
- ![ROC Curve](assets/images/ROC_LR_RFT_Comparison.png)

### Feature Importance - Random Forest (Original vs Tuned)
- ![RF Importance](assets/images/FeatureImportance_RF.png)

### Coefficients - Logistic Regression
- ![Log Coefficients](assets/images/LogisticRegressionCoefficients.png)

---

## Model Performance Summary

| Model                | AUC  | Accuracy | Churn Recall | Stay Recall |
|---------------------|------|----------|--------------|-------------|
| **Logistic Regression** | 0.79 | 71%      | 77%          | 67%         |
| **RF (Default)**        | 0.62 | 50%      | 95%          | 22%         |
| **RF (Tuned)**          | 0.68 | 56%      | 93%          | 25%         |

---

## Additional Findings from Feature Importance Visualizations

- **Support Calls** is the top predictor in both models. Customers requiring more assistance are highly prone to churn.
- **Total Spend** is strongly associated with retention. High-spending customers are significantly less likely to leave.
- Logistic Regression coefficients provide clear **directionality**: Payment Delay and Last Interaction increase churn probability; Tenure and Usage Frequency reduce it.
- The Tuned Random Forest model redistributed importance slightly, emphasizing behavioral features more evenly.

---

## How to Reproduce

1. Clone the repository:
```bash
git clone https://github.com/SebastianMarrero/SaaS_Churn_Analysis.git
```
2. Open the notebook `CustomerChurnEDA.ipynb` in Jupyter Lab or VS Code  
3. Run the notebook cells sequentially  
4. View generated visualizations in `/assets/images` or inline  
5. Optional: Customize preprocessing or model tuning parameters

---

## Contact

Created by **Sebastian Marrero**  
Email: sebastianmarrero64@gmail.com  
LinkedIn: [linkedin.com/in/sebastianmarrero](https://linkedin.com/in/sebastianmarrero)
