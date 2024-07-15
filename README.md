# Food Delivery Cost and Profitability Analysis

### Business Problem 
---
A food delivery service is experiencing challenges in achieving profitability across its operations. This project aims to understand the dynamics of its cost structure and profitability to identify strategic opportunities for improvement. Using a dataset of 1,000 food orders, we will conduct a detailed cost analysis, evaluate profitability, and provide strategic recommendations for enhancing profitability. We will also simulate the financial impact of the proposed strategies.

### Approach
---
#### Exploratory Data Analysis (EDA):
  1. **Loading and Inspecting the Dataset**:
     - Checked the dataset's structure and characteristics.
       
  2. **Data Processing and Feature Engineering**:
     - Converted date-like features to their respective data types.
     - Checked for missing values.
     - Discounts & Offers: Extract and clean the discount percentage from the column.
       
#### Feature Engineering Steps
  1. **Statistical Summary**:
     - Checked the statistical summary of the derived dataset.
       
  2. **Created Columns**:
     - Created a new column, discount_amount, from discounts_%.
     - Created a column total_cost to understand the company's total cost components.
     - Created a column revenue to analyze revenue trends or track income streams.
     - Created a column total_profits to analyze assess profitability.
     - Created a simulated commission fee to determine optimal commission, ensuring profitability across all orders
     - Created simulated discount amounts to identify an optimal "sweet spot" for commission and discount percentages, ensuring profitability across orders.
     - Created a simulated total costs and simulated profit column based on the newly created discount amount  and commission fee column to simulate the financial impact of recommended strategies on profitability.

  3. **Univariate Analysis**:
     - Conducted a univariate analysis to understand data distribution and detect outliers.

  4. **Multivariate Analysis**:
     - Conducted a multivariate analysis to understand relationships and patterns.

  5. Created a Tableau dashboard to present the analysis.
     
### Insights
---
1. Delivery Fees - More than half of the orders have a delivery fee of Rs30 or less, with significant variation (std dev: 16.95) due to differences in delivery time and distance. Delivery fee distribution is bimodal, mostly greater than Rs10.
2. Commission Fee - More than half of the commission fees are Rs127 or less. Commission fee data has heavy tails and is close to a normal distribution.
3. Discounts and Offers - Discount amounts have a right-skewed distribution, with many orders receiving close to zero or between zero and Rs200.
4. More than half of the refunds/chargebacks are valued at Rs0 or less.
5. Usage of payment methods is relatively equal across Credit Card, Digital Wallet, and Cash on Delivery.
    - Payment processing fees are highest for Cash on Delivery, followed by Credit Card, and lowest for Digital Wallet.
    
#### Profitability Analysis
  1. The average profit per order is -Rs105.71, indicating overall losses.
  2. Profit distribution is highly skewed, with most orders incurring losses.

##### Impact of Discounts
- Discounts are a significant cost component, heavily impacting overall profitability.
- There is a positive correlation between Order Value and Discount Amount, meaning higher order values tend to receive higher discounts.

### Strategic Recommendations
---
##### Commission and Discount Rates
1. To improve profitability, aim for a commission rate closer to **31%** and a discount rate around **6%**.
    - For profitable orders, the average commission percentage is 30.50% and the average discount percentage is 5.87%.
2. Adjusting Payment Methods
    - Encourage the use of Digital Wallets due to lower payment processing fees compared to Cash on Delivery and Credit Cards.
    - **Introducing Unified Payments Interface (UPI)** - UPI is a popular payment method in India, known for facilitating instant real-time payment transactions with very low processing fees.
    - UPI transactions generally incur fees ranging from 0% to 0.3% per transaction, often capped at a small maximum amount (e.g., ₹5-10).
