<h2 align="center">Ultimate Data Science Challenge</h2>

This analysis focuses on user login patterns over a specified period, aiming to uncover key trends in activity and engagement. Through visualizations of hourly, weekly, and monthly login data, I examined fluctuations in user behavior, identifying peak times and periods of lower activity. The objective was to interpret these patterns and provide actionable insights for optimizing user engagement, particularly in terms of timing and seasonality. This report also highlights potential areas for further investigation, such as anomalies in specific months, to help refine strategic efforts and improve overall user satisfaction.

### Summary of Findings from Visualizations
- **Hourly Patterns**: Through visualizations, I observed that most logins occur during the first four hours of the day, indicating a peak in user activity early on. However, there is a significant dip in logins between 6 AM and 9 AM, likely due to users transitioning into their daily routines.
  
- **Weekly Average Logins**: My analysis of weekly averages revealed that from the first week of January to the first week of February, logins were consistently below average. This pattern suggests a post-holiday slowdown in engagement. Notably, the highest average logins were around March 15, indicating a resurgence in user activity, possibly linked to marketing efforts or seasonal events.
  
- **Monthly Average Logins**: The monthly analysis showed that April had the highest overall logins, yet both January and April experienced periods of below-average activity. This suggests that while user engagement peaked in April, fluctuations might have been influenced by competing events or significant holidays.

### Interpretation of Results
- **Engagement Opportunities**: The concentration of logins in the early morning hours suggests a strategic opportunity for targeted promotions or notifications during this peak period.
  
- **User Availability**: The decline in activity from 6 AM to 9 AM emphasizes the need to tailor engagement efforts to user availability.
  
- **Seasonal Trends**: The below-average logins at the start of the year highlight potential opportunities for campaigns aimed at boosting engagement during quieter months.
  
- **Anomaly Investigation**: The fluctuations observed in April, despite high overall logins, warrant further analysis to understand user behavior and optimize future strategies.

### Conclusion
In conclusion, my visualizations provided critical insights into user login patterns, allowing me to interpret key trends and behaviors. These insights can inform engagement strategies, ensuring that efforts align with user availability and preferences to enhance interaction and satisfaction.

---

## Part 2 - Experiment and Metrics Design

The neighboring cities of Gotham and Metropolis have complementary circadian rhythms: on weekdays, Ultimate Gotham is most active at night, and Ultimate Metropolis is most active during the day. On weekends, there is reasonable activity in both cities.

However, a toll bridge, with a two-way toll, between the two cities causes driver partners to tend to be exclusive to each city. The Ultimate managers of city operations for the two cities have proposed an experiment to encourage driver partners to be available in both cities, by reimbursing all toll costs. 

### Key Measure of Success
- **Metric**: Driver Utilization Rate in Both Cities

- **Reason for Choice**: The driver utilization rate in both cities is a direct measure of the effectiveness of the experiment. By comparing the percentage of drivers who operate in both Gotham and Metropolis before and after implementing the toll reimbursement, we can assess whether the reimbursement incentivizes drivers to cross the bridge and serve both areas. This metric reflects changes in driver behavior that directly result from the policy change, making it a clear indicator of success.

---

### Experimental Design

1. **Implementation of the Experiment**
   - **Selection of Participants**: Randomly select a cohort of driver partners from both cities. Ensure a mix of drivers who typically operate exclusively in either Gotham or Metropolis.
   - **Control and Treatment Groups**:
     - **Control Group**: A group of drivers who will not receive toll reimbursement.
     - **Treatment Group**: A group of drivers who will receive toll reimbursement for any trips made between the two cities.
   - **Duration**: Run the experiment for a defined period (e.g., 8 weeks) to capture sufficient data on driver activity patterns.
   - **Data Collection**: Collect data on the following metrics:
     - Number of trips made by each driver in both cities.
     - Total revenue generated from rides in both cities.
     - Toll costs incurred by drivers, including those reimbursed.

2. **Statistical Test(s)**
   - **Descriptive Statistics**: Calculate the average utilization rate (trips in both cities) for both the control and treatment groups before and after the experiment.
   - **Statistical Test**: Use a two-sample t-test to compare the means of driver utilization rates between the control and treatment groups:
     - **Null Hypothesis (H0)**: There is no difference in the driver utilization rate between the two groups.
     - **Alternative Hypothesis (H1)**: The driver utilization rate is significantly higher in the treatment group.
   - **Significance Level**: Set a significance level (e.g., α = 0.05) to determine statistical significance.

---

### Interpretation of Results and Recommendations

Based on the model evaluations, the Random Forest algorithm demonstrates the most balanced performance for predicting whether a user will be active in their 6th month. While Naive Bayes and Logistic Regression have higher precision, they suffer from lower recall, meaning they fail to capture a significant number of active users. The Support Vector Machine (SVM) and K-Nearest Neighbors (KNN) models perform moderately well, with SVM showing improved recall and KNN providing a decent balance between precision and recall. However, Random Forest stands out with its strong recall of 0.60 and balanced precision of 0.59, making it the most reliable model for accurately identifying both retained and non-retained users. This balanced performance is critical in ensuring that the model minimizes false positives and false negatives, making Random Forest the optimal choice for Ultimate's user retention prediction.

The validity of the models can be evaluated based on several performance metrics, such as accuracy, precision, recall, and the F1-score. These metrics provide insight into how well the model generalizes to new data and its ability to make reliable predictions.

Random Forest Performance:
Accuracy: 69.47% – This indicates that approximately 69% of the predictions made by the model are correct.
Precision: 0.59 – This means that when the model predicts a user is retained, it is correct 59% of the time.
Recall: 0.60 – This shows that the model is able to correctly identify 60% of the users who were actually retained.
F1-Score: The F1-score balances precision and recall, indicating the model’s effectiveness at predicting active users. While the accuracy and precision are moderate, the recall score of 0.60 is notable as it suggests the model can successfully identify a substantial proportion of retained users. This balance of precision and recall, along with a decent accuracy, indicates that the model is reasonably valid for predicting user retention. However, improvements could be made by further tuning the model, using more features, or employing advanced techniques like ensemble learning.
Key indicators such as the confusion matrix further support the model’s performance by showing a balance between true positives and true negatives. Random Forest’s ability to generalize well is reflected in its competitive performance across multiple metrics, making it a valid choice for predicting rider retention.

---

### Caveats

- Consider external factors that could influence driver behavior, such as changes in demand, local events, or seasonal variations.
- Ensure that the sample size is adequate to capture diverse driving behaviors across different demographics.

By implementing this experiment, city operations can effectively gauge the impact of the proposed toll reimbursement on driver partners, allowing for data-driven decision-making to improve service efficiency in both Gotham and Metropolis.
