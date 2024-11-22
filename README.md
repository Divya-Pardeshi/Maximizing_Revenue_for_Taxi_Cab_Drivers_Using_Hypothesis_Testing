# Maximizing Revenue for Drivers Through Payment Type

## Overview
In the fast-paced taxi booking sector, maximizing revenue is crucial for long-term success and driver satisfaction. This project uses data-driven insights to help maximize revenue streams for taxi drivers, focusing specifically on the relationship between payment type and fare amounts.

Our goal is to determine whether different payment methods (card vs. cash) influence fare pricing and explore how we can nudge customers towards payment methods that generate higher revenue for drivers without negatively impacting the customer experience.

## Research Question
- **Is there a relationship between total fare amount and payment type?**
- **Can we encourage customers to choose payment methods that generate higher revenue for drivers?**

## Data Overview
The dataset used in this analysis is the **NYC Taxi Trip Records**, which includes key features related to each taxi trip. For this research, we focused on the following relevant columns:

- `passenger_count`: Number of passengers (1 to 5)
- `payment_type`: Type of payment (Card or Cash)
- `fare_amount`: Total fare amount
- `trip_distance`: Distance of the trip (miles)
- `duration`: Duration of the trip (minutes)

## Methodology
### Step 1: **Descriptive Analysis**
We performed statistical analysis to summarize the key aspects of the data, with a particular focus on **fare amounts** and **payment types**.

### Step 2: **Hypothesis Testing**
A T-test was conducted to evaluate whether there is a significant relationship between payment type and fare amount. The null hypothesis states that there is no difference in fare amounts between card and cash payments.

### Step 3: **Regression Analysis**
We implemented linear regression to investigate how **trip duration** (calculated from pickup and dropoff times) affects the fare amount, considering other variables.

## Analysis and Findings

### 1. **Journey Insights**
- Customers paying with **cards** tend to have a slightly higher average trip distance and fare amount compared to those paying with **cash**.
    - **Card Payments:**
        - Average Fare Amount: $13.7 (Standard Deviation: $6.5)
        - Average Trip Distance: 3.23 miles (Standard Deviation: 2.32 miles)
    - **Cash Payments:**
        - Average Fare Amount: $12.25 (Standard Deviation: $6.2)
        - Average Trip Distance: 2.8 miles (Standard Deviation: 2.23 miles)

This indicates that customers tend to opt for card payments when they have longer trips with higher fares.

### 2. **Payment Type Preferences**
- **Card payments** make up **67.5%** of all transactions, significantly higher than **cash payments**, which account for **32.5%**. This suggests that customers prefer card payments, likely due to the convenience, security, or incentives associated with cards.

### 3. **Passenger Count Analysis**
- Among card payments, **single-passenger rides** represent **40.08%** of all transactions.
- For cash payments, **single-passenger rides** make up **20.04%** of all transactions.
- Larger groups tend to use taxis less frequently or may opt for other transportation options, influencing the payment type choice.

### 4. **Hypothesis Testing Results**
- **Null Hypothesis**: There is no difference in average fare between card and cash payments.
- **Alternative Hypothesis**: There is a significant difference in average fare between the two payment methods.

With a **T-statistic** of 165.5 and a **P-value** less than 0.05, we reject the null hypothesis, indicating a significant difference in average fare amounts between card and cash payments.

## Recommendations
Based on our findings, we recommend the following strategies to maximize revenue for taxi drivers:

1. **Encourage Card Payments**: Since card payments tend to have higher average fares and longer trips, incentivizing customers to choose this payment method could significantly boost revenue.
   - **Action**: Offer incentives or discounts for card payments to make them more attractive to customers.
  
2. **Optimize Payment Options**: Ensure that the card payment process is seamless, fast, and secure to improve the overall customer experience and encourage the adoption of this payment method.
  
3. **Targeted Marketing**: Focus on promoting card payments to passengers who typically opt for cash, emphasizing the convenience and benefits (e.g., rewards, promotions) of paying with a card.

## Conclusion
Maximizing taxi driver revenue involves understanding customer behavior and payment preferences. Our analysis indicates that encouraging customers to choose card payments—especially for longer trips—can significantly enhance revenue. Implementing incentives, ensuring smooth payment experiences, and strategically marketing card payments are key to achieving this goal.

---

Thank you for reviewing the findings! For more details or to contribute, feel free to open issues or submit pull requests.
