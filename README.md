## NewBank Customer Churn Analysis: Data-Driven Insights and Recommendations

# PROJECT OVERVIEW
This work presents a comprehensive data analysis of  NewBanking customer churn, directly addressing the critical business requirements laid out by our executive team in order to increase our competitive in the financial landscape, understanding and mitigating customer attrition is paramount to maintaining our profitability and market share.

Our primary objective with this project was to leverage the provided Bank Customer Churn data to gain actionable insights into why our customers are churning. Specifically, our analysis set out to answer key business questions, including:

  1. Determining the overall churn rate and identifying demographic segments most susceptible to churn (e.g., by gender, age, and geographical region).

  2. Investigating how financial attributes (credit score, account balance, estimated salary) and product usage (number of bank products, active membership, credit card ownership)            correlate with churn likelihood.

  3. Ultimately, providing data-driven recommendations for proactive retention strategies and opportunities for optimizing our service offerings.


# Overall Churn Landscape

Overall Customer Churn Rate:
The data indicates an overall churn rate of 20.4%. This means approximately one-fifth of our customers are churning, which represents a significant opportunity for improvement in retention.

Gender:

The "Customers Count by Gender" chart shows a relatively even distribution of male (45.43%) and female (54.57%) customers. While not explicitly shown as "Churn Rate by Gender," if the churn rates are similar across genders, then the higher count of female customers might imply a higher absolute number of female churners, but the dashboard doesn't directly support a disproportionate churn rate by gender. Further drill-down would be needed here.

Age Groups:

The "Churn Rate by Age Group and Activity Status" chart reveals a distinct pattern:

  -Churn rates are relatively low for customers under 30.  
  -Churn rates begin to increase for customers in the 31-40 and 41-50 age groups.  
  -The highest churn rates are observed in the 51-60 and 61-70 age groups, peaking around 51-60 years old.
  -Churn rates then significantly decline for customers over 71.

This suggests that our mid-to-older age segments (50s and 60s) are particularly vulnerable to churn.

Geographical Regions (Country): The "Customers Count by Country" shows our customer base is split between France (50.14%), Spain (24.77%), and Germany (25.09%).

The "Churn Rate by Age Group and Country" chart further elaborates: France consistently exhibits the highest churn rate across most age groups, especially peaking significantly in the 51-60 age group (over 60%). Germany follows with high churn rates, also peaking in the 51-60 age group. Spain generally shows lower churn rates compared to France and Germany across all age groups, although it still experiences a peak in the 51-60 age group.

This indicates a critical issue in France, particularly with our mature customer segment, followed closely by Germany.


# Financial Behavior and Product Usage Impact

1. Credit Score Correlation with Churn:

Customers with very low credit scores ≤400 exhibit an exceptionally high churn rate, approaching 100%.  
Churn rates drop dramatically and remain relatively low and stable for customers with credit scores above 400 (e.g., 401-500, 501-600, 601-700, 701-800, and ≥801.

This strongly suggests that customers with poor credit scores are highly likely to churn.


2. Account Balance Correlation with Churn:

The "Churn Rate by Acc Balance" graph shows a non-linear relationship:

Customers with no account balance (0) have a moderate churn rate. Customers with balances in the $1K-$10K range exhibit an extremely high churn rate, potentially reaching 100%. Although it may seem like a significant finding, during the EDA process it was discovered that there was not enough entries to make a judgement. Churn rates then decrease for balances in the $10K-$100K and $100K-$200K ranges. Interestingly, churn rates begin to rise again for customers with balances >$200K.

This indicates that customers with a very high-balance customers might be at a higher risk than mid-range ones.


3. Number of Products and Churn Probability:

The "Churn Rate and Customers Count by Products" chart shows a clear relationship:

Customers holding Product 1 and Product 2 have relatively lower churn rates. Customers holding Product 3 show an extremely high churn rate, potentially nearing 100%. Customers with Product 4 also exhibit a very high churn rate, though slightly lower than Product 3.

This is a critical finding: holding Product 3 or Product 4 is a strong indicator of high churn risk. We also see that the customer count for Product 3 and 4 is very low, which implies that these might be niche or problematic products.


4. Active Membership and Credit Card Ownership Influence on Churn:

Active Membership (Activity Status):

The "Customers Count by Activity Status" shows an almost even split between active (48.49%) and inactive (51.51%) customers. The "Churn Rate by Age Group and Activity Status" implies that inactive customers have a consistently higher churn rate across all age groups compared to active customers. This is expected but reinforces the importance of engagement.


5. Credit Card Ownership (Has Credit Card):

The "Customers Count by Has Credit Card" shows that 70.55% of customers own a credit card, while 29.45% do not.The "Churn Rate by Age Group and Has Credit Card" indicates that customers who do NOT own a credit card ("Not Owned") generally have a slightly higher churn rate across age groups compared to those who do ("Owned"), although the difference is not as dramatic as other factors.

The "Churn Rate by Tenure and Has Credit Card" further suggests that customers without a credit card show more volatility in churn rates across different tenures, often spiking higher than those with a card.

# Strategic Insights & Retention Initiatives

Based on the analysis, the primary drivers of customer churn, prioritized by their apparent impact, are:

1. Specific Products (Product 3 & Product 4): Customers holding Product 3 and Product 4 show exceptionally high churn rates. This suggests fundamental issues with these products, their target audience, or the experience they provide.
2. Low Credit Scores ≤400: These customers almost invariably churn. This could indicate financial distress, dissatisfaction with banking services for this segment, or a lack of suitable product offerings.
3. Age Group (51-70 years old): Our mature customer base is significantly more prone to churn, especially in France and Germany.
4. Geographical Region (France and Germany): Customers in these countries consistently have higher churn rates, particularly within the vulnerable age groups.
5. Inactive Customer Status: Less engaged customers are more likely to churn, reinforcing the need for continuous engagement.


Actionable Recommendations to Reduce Churn:

Immediate Review of Product 3 and Product 4:

1. Deep Dive: Conduct an urgent investigation into the design, pricing, customer support, and target audience for Product 3 and Product 4. Are these products meeting customer needs? Are there fundamental flaws?

2. Re-evaluation/Retirement: Consider re-designing these products entirely or, if they are unprofitable and driving significant churn, consider phasing them out or offering alternatives to customers currently holding them.

3. Migration Strategy: For existing customers with Product 3 or 4, proactively offer transitions to more stable products (Product 1 or 2) with attractive incentives.

4. Targeted Intervention for Low Credit Score Customers ≤400: Segmentation: Identify these customers immediately. Specialized Support: Instead of letting them churn, explore if tailored financial literacy programs, limited-feature accounts, or specific credit-building products could serve them better and retain them, or at least understand their reasons for leaving. This might also involve re-evaluating our risk appetite for this segment.

5. Product Upsell/Cross-sell: Strategically offer additional products (e.g., credit cards if they don't have one, or a loan product) that could deepen their relationship and increase stickiness, while being mindful of their financial profile.

6. Region-Specific & Age-Targeted Retention Campaigns (France & Germany, Age 51-70):

  -Automated Triggers: Implement automated systems to identify customers whose activity levels are declining.
  
  -Re-engagement Campaigns: Develop targeted campaigns (email, SMS, personalized calls) to re-engage inactive customers with relevant offers, reminders of benefits, or invitations to       branch events.

7.Credit Card Promotion: As customers without credit cards show slightly higher churn, a targeted campaign to encourage credit card adoption (for eligible customers) could subtly increase stickiness and potentially ARPU through card fees or interest.

