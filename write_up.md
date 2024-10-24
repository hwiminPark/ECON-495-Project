# Predicting Individual Savings Potential: A Regression Model of Financial Behavior
![image](https://github.com/user-attachments/assets/a9a64393-896c-4ca9-a2e6-689c0d49ac50)

## Introduction
   - **Objective:** 
     The goal of this project is to predict individual savings potential based on demographic, educational, and financial data. By understanding the factors that influence savings, businesses and policymakers can better target financial planning services and improve marketing strategies.
   
   - **Significance:** 
     Understanding how different factors like age, education, and income influence savings behavior can have significant implications for financial services. Accurate savings predictions can enhance the personalization of financial advice and improve overall profitability by enabling targeted financial products.

   - **Scope:** 
     The analysis involves a dataset of over 22,000 individuals from the Federal Reserve's Survey of Consumer Finances and uses regression techniques to identify key factors affecting savings potential.

## Data Overview
   - **Dataset Source:**
     This project uses data from the Federal Reserve's Survey of Consumer Finances, consisting of 22,975 individuals and 5,473 features, covering various aspects of personal financial behavior.

   - **Key Features:**
     - **Roth IRA Balance:** The total amount in a Roth IRA account.
     - **Age:** The individual's age at the time of the survey.
     - **Savings Account Balance:** The amount of money saved in a savings account.
   
   - **Preprocessing:** 
     - **Data Cleaning:** Removed invalid values to ensure the dataset's integrity and reliability for analysis.
	- **Outlier Treatment:** Employed Winsorization to address right-tail outliers, which capped extreme values to reduce their impact on model performance.

## Methodology
   - **Exploratory Data Analysis (EDA):**
     Conducted analysis on the distribution of key features such as age, income, and savings. Correlation analysis revealed low to moderate relationships between features and savings, with age and checking account balance emerging as key predictors.

   - **Modeling Approach:**
     The Random Forest regression model was chosen due to its ability to handle complex relationships and feature importance ranking. The model was evaluated using RMSE and R² metrics for accuracy.

## Results
   - **Model Performance:**
     The Random Forest model was the best performer, with an RMSE of 2.302 and an R² of 0.804, indicating that the model explains a substantial amount of variance in savings potential.

   - **Key Findings:**
    - **Age and Checking Account Balance:** These were identified as the top two predictors of savings potential.
	- **Low to Moderate Correlations:** The correlation matrix showed that most individual features had only mediocre relationships with savings, suggesting that savings behavior is influenced by a combination of factors rather than any single variable.

   - **Visualizations:**
    - Feature importance bar chart
      ![image](https://github.com/user-attachments/assets/0e16dfbe-09db-40da-98fb-6c48ef427def)
	- Residual plots to check model accuracy
      ![image](https://github.com/user-attachments/assets/3ae29ce9-f9d6-404e-9c6e-9217aab12691)
	- Correlation matrix
      ![image](https://github.com/user-attachments/assets/4b6e5ede-c95c-4829-8c79-e7d4451e73cf)

## Evaluation Metrics
- **Root Mean Squared Error (RMSE):**
    RMSE of 2.302, indicating the average error between predicted and actual savings.
    
- **R² (Coefficient of Determination):**
    R² of 0.804, showing the percentage of variance in savings explained by the model.

## Summary of Findings
   - **Key Results:**
     The analysis reveals that age and checking account balance have the most significant impact on savings potential. Other features like education level and income also play a role but are less impactful.
   
   - **Trends and Patterns:**
     Cluster analysis identified distinct financial profiles that can help financial institutions personalize their services.

## Implications
   - **Impact:**
     These findings can help financial institutions tailor financial products to different age groups and income brackets, improving profitability through personalized services.

   - **Applications:**
     This model can assist in predicting savings behavior to inform product offerings, financial advising, and marketing strategies.

## Limitations
   - **Data Constraints:** 
     Some key behavioral variables, such as spending habits or risk tolerance, were not included in the dataset, limiting the model’s predictive power.
   
   - **Generalizability:**
     The model may have reduced applicability to financial profiles that deviate significantly from the norm due to the presence of outliers and high variability in the data.

## Improvements
   - **Future Research:** 
     Future research could consider panel data to analyze changes in savings behavior over time, particularly as major life events (such as marriage or retirement) occur.
   
   - **Model Updating:** 
     Regularly updating the model with new data and retraining it will improve accuracy, as financial behaviors evolve over time.

## Conclusion
   - **Reflection:** 
     This project has provided valuable insights into the key factors influencing individual savings potential. The Random Forest model was effective, but future work could incorporate additional behavioral data to improve predictions.

## References
- **Data Source:** 
     [Survey of Consumer Finances](https://www.federalreserve.gov/econres/scfindex.htm)
- **Supporting Literature:** 
  - Fernández-Villaverde, J., & Krueger, D. (2001). _Consumption and Saving over the Life Cycle: How Important are Consumer Durables?_ National Bureau of Economic Research.
  - Fagereng, A., Holm, M. B., Moll, B., & Natvik, G. (2019). _Saving Behavior Across the Wealth Distribution: The Importance of Capital Gains_. National Bureau of Economic Research.
  - Mahdzan, N. S., & Tabiani, S. (2013). _The Impact of Financial Literacy on Individual Saving: An Exploratory Study in the Malaysian Context_. _Transformations in Business and Economics_. 12(1), 41-55.
 
## Additional Resources
- **Github Repository:** [Link to Github](https://github.com/hwiminPark/Predict_Individual_Savings/)
- **Portfolio Website:** [View Project Details](https://hwiminpark.github.io/#projects)
