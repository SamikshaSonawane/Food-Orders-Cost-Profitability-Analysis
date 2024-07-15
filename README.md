# Food Delivery Cost and Profitability Analysis

### Project Overview
A food delivery service is experiencing challenges in achieving profitability across its operations. This project aims to understand the dynamics of its cost structure and profitability to identify strategic opportunities for improvement. Using a dataset of 1,000 food orders, we will conduct a detailed cost analysis, evaluate profitability, and provide strategic recommendations for enhancing profitability. We will also simulate the financial impact of the proposed strategies.

### Steps
1. Detailed Cost Analysis: Identifying the major cost components associated with delivering food orders, including direct costs like delivery fees and indirect costs like discounts and payment processing fees.
2. Profitability Evaluation: Calculating the profitability of individual orders and aggregating this data to assess overall profitability. This involves examining how revenue generated from commission fees measures against the total costs.
3. Strategic Recommendations for Improvement: Based on the cost and profitability analysis, identifying actionable strategies to reduce costs, adjust pricing, commission fees, and discount strategies to improve profitability. This includes finding a “sweet spot” for commission and discount percentages that ensures profitability across orders.
4. Impact Simulation of Proposed Strategies: Simulating the financial impact of the recommended strategies on profitability, using the dataset to forecast how adjustments in commission rates and discount strategies could potentially transform current losses into profits.

### Insights
1. Delivery Fees - More than half of the orders have a delivery fee of Rs30 or less, with significant variation (std dev: 16.95) due to differences in delivery time and distance. Delivery fee distribution is bimodal, mostly greater than Rs10.
2. Commission Fee - More than half of the commission fees are Rs127 or less. Commission fee data has heavy tails and is close to a normal distribution.
3. Discounts and Offers - Discount amounts have a right-skewed distribution, with many orders receiving close to zero or between zero and Rs200.
4. More than half of the refunds/chargebacks are valued at Rs0 or less.
5. Usage of payment methods is relatively equal across Credit Card, Digital Wallet, and Cash on Delivery.
    - Payment processing fees are highest for Cash on Delivery, followed by Credit Card, and lowest for Digital Wallet.
    
#### Profitability Analysis
##### Profit Distribution
1. The average profit per order is -Rs105.71, indicating overall losses.
2. Profit distribution is highly skewed, with most orders incurring losses.

##### Impact of Discounts
- Discounts are a significant cost component, heavily impacting overall profitability.
- There is a positive correlation between Order Value and Discount Amount, meaning higher order values tend to receive higher discounts.

### Strategic Recommendations
##### Commission and Discount Rates
1. To improve profitability, aim for a commission rate closer to **31%** and a discount rate around **6%**.
    - For profitable orders, the average commission percentage is 30.50% and the average discount percentage is 5.87%.
    
3. Adjusting Payment Methods
    - Encourage the use of Digital Wallets due to lower payment processing fees compared to Cash on Delivery and Credit Cards.
    - **Introducing Unified Payments Interface (UPI)** - UPI is a popular payment method in India, known for facilitating instant real-time payment transactions with very low processing fees.
    - UPI transactions generally incur fees ranging from 0% to 0.3% per transaction, often capped at a small maximum amount (e.g., ₹5-10).
