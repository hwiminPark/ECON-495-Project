# Predicting Individual Savings Potential: A Regression Model of Financial Behavior
![image](https://github.com/user-attachments/assets/a9bf2ebd-b49d-4efe-bd47-155b1043d876)

## Project Overview
This project aims to predict individual savings potential by analyzing key demographic and financial factors such as age, education, and various financial assets. By building a regression model, the goal is to identify the factors that influence savings behavior and to accurately estimate savings potential. This analysis can provide valuable insights for financial institutions looking to design personalized savings products or financial planning services.

## Data

- **Dataset Source:** [Federal Reserve's Survey of Consumer Finances](https://www.federalreserve.gov/econres/scfindex.htm)
- **Description:** The dataset consists of **22,975 individuals** and **5,473 features**, offering a comprehensive view of personal finances and economic behavior.

### Data Description

Below are some of the key features used in this analysis:

- **Roth IRA balance (x6551):** The total balance in an individual’s Roth IRA account.
- **Savings account balance (x3730):** The amount of money held in an individual’s savings account.
- **Age of individual (x8022):** The age of the individual respondent.
- **Total education loan borrowed (x7805):** The total amount of student loans taken by an individual.
- **Highest level of educational attainment (x5931):** The highest level of education an individual has completed.
- **Current checking account balance (x3506):** The amount of money in an individual’s checking account.
- **Total brokerage account balance of family (x3930):** The total balance in the family’s brokerage accounts.
- **Typical year income (x7362):** The average annual income an individual typically earns.
- **Years in college (x5933):** The number of years an individual has spent in higher education.

### Preprocessing:
  - **Data Cleaning:** Corrected invalid or missing values, removed duplicates, and handled outliers using winsorizer for more robust analysis.
  - **Feature Engineering:** Developed interaction terms and polynomial features to capture non-linear relationships, enhancing model complexity.
  - **Log Transformation:** Applied logarithmic transformation to skewed numerical features, improving normality and reducing the influence of extreme values.
  
## Methodology
- **Exploratory Data Analysis (EDA):**
   - **Feature Distribution:** Examined the distribution of key features such as age, savings account balances, and educational loan amounts.

- **Modeling:**
   - **Base Models:** Multiple regression models were tested, including linear regression, decision trees, and random forest models.
   - **Best Model:** Random Forest Regression emerged as the best model, offering the highest predictive accuracy.
   - **Feature Importance:** The model highlighted **age** and **checking account balance** as the most significant predictors of individual savings.
![image](https://github.com/user-attachments/assets/904884f4-ffe8-43b3-b1f0-16fbebd23a99)


- **Evaluation Metrics:**
   - **Root Mean Squared Error (RMSE):** Used to assess model performance by measuring how much the predicted savings potential deviates from the actual values.
   - **R^2:** Shows how much of the variance in savings potential is explained by the model, reflecting its overall fit.
   - **Residual Analysis:** Evaluated residuals to detect any patterns in model errors, particularly for low-income individuals where residuals tended to be larger.
![image](https://github.com/user-attachments/assets/7c5434d2-5881-499f-be8d-35e0bb40caa5)


## Results
- **Model Performance:**
  - **Random Forest:** Achieved the best prediction accuracy, outperforming other models with the lowest prediction error.
  
- **Key Insights:**
  - **Age and Checking Account Balance:** These were the most influential factors in predicting savings potential. Older individuals and those with higher checking account balances tended to have higher savings.
  - **Residual Patterns:** Residuals analysis indicated a potential bias in predicting savings for low-income individuals, suggesting areas for further model refinement.

## Implications
- **Impact:** The findings of this project can help financial institutions target specific groups with personalized savings products and strategies.
- **Applications:** Insights from the model can be used to better design financial planning tools, targeted at younger individuals with lower savings or those nearing retirement with significant savings.

## Limitations
- **Outliers and Variability:** The dataset contained many outliers and high variance, which may have affected model performance. Additional behavioral variables like spending habits could improve the model’s predictive power.
- **Generalizability:** The model may not generalize well to individuals with non-traditional financial profiles.

## Future Work
- Future analyses could include **behavioral variables** such as risk tolerance and spending habits to improve model accuracy.
- **Longitudinal tracking** of savings behavior over time could provide deeper insights into how life events impact savings.

## Additional Resources
- **References:** Federal Reserve's Survey of Consumer Finances Dataset
- **Project Website** [View Project Details and Documentation](https://hwiminpark.github.io/#projects)
