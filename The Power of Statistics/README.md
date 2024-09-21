# Fare Amount Analysis by Payment Type
## Overview
This project analyzes the relationship between different payment types and the fare amount customers pay. The dataset contains payment_type encoded as integers, with the following values:

- 1: Credit card
- 2: Cash
- 3: No charge
- 4: Dispute
- 5: Unknown

The goal of this analysis is to investigate whether there is a statistically significant difference between the average fare amounts for customers who pay by credit card and those who pay by cash. A two-sample t-test is conducted as part of an A/B test to assess this.

## Research Question
Is there a significant difference in the average fare amount paid by customers who use credit cards compared to customers who use cash?

## Hypotheses
- Null Hypothesis (H₀): There is no significant difference in the average fare amount between customers who use credit cards and those who use cash.
- Alternative Hypothesis (H₁): There is a significant difference in the average fare amount between customers who use credit cards and those who use cash.

## Steps
- Descriptive Statistics: The first step in the analysis is to compute summary statistics, such as the mean, median, and standard deviation of fare amounts for each payment type. This helps explore the data and identify trends.
- Hypothesis Testing: A two-sample t-test is conducted to compare the mean fare amounts for credit card and cash payments. The significance level for this test is set at 0.05.

## Business Insights
The results of the hypothesis test provide insight into whether payment method influences the fare amount. If a significant difference is found, businesses may consider tailoring promotions or incentives based on payment method preferences.

## Assumptions & Limitations
- The dataset assumes independent transactions between payment methods.
- Factors like trip distance, time, or customer demographics are not accounted for, which may affect the fare amount.
- This analysis simplifies real-world complexities for educational purposes.

## Requirements
- Python 3.x
- Libraries: pandas, numpy, scipy, seaborn, matplotlib

## Conclusion
This analysis offers a simplified approach to A/B testing by comparing fare amounts based on payment type. The results provide actionable business insights, though real-world data would require further refinement and more comprehensive modeling.
