# Indian Retail Store — Sales & Profitability Analysis

An end-to-end Power BI project analyzing retail transaction data across Indian cities to identify where a retail chain should focus for revenue growth and, more importantly, profit growth.

## Business Question
Which cities, product categories, and store formats should this retail chain prioritize to grow profit — not just revenue?

## Data
- 1,500 retail transactions across 20 states and 50+ cities in India (January–March 2025)
- Fields: transaction ID, customer, city, state, product category, quantity, revenue, cost, profit, margin %, payment method, store type, and visit date
- Data cleaning performed in Power Query:
  - Removed duplicate transaction records
  - Standardized inconsistent city name formatting (casing, extra spaces)
  - Handled missing payment method values by labeling them as "Unknown" rather than dropping them
  - Converted date fields and built a dedicated Date dimension table for time-based analysis

## Approach
- Built a star schema data model (Sales fact table + Date dimension table)
- Created custom DAX measures including Total Revenue, Total Profit, Profit Margin %, Average Basket Value, Revenue Month-over-Month growth, and category/city revenue rankings
- Designed a 4-page interactive report:
  1. **Executive Overview** — high-level KPIs, monthly revenue trend, category mix
  2. **Customer Behaviour** — payment method preferences, store type performance, weekday vs weekend spending patterns
  3. **Geographic Insights** — state and city-level revenue and profit breakdown
  4. **Category Deep Dive** — profitability comparison across product categories and store types

## Key Insights
1. **Electronics drives the most revenue but the thinnest margins.** It accounts for 68.6% of total revenue but only an 8.8% profit margin — nearly a third of Clothing's 27.6% margin. Revenue leadership doesn't equal profit leadership.
2. **UPI is the dominant payment method**, making up 37.9% of total revenue, ahead of Cash, Credit Card, and Debit Card.
3. **Mall Stores are the top-performing store format** by total revenue, ahead of Supermarkets and Local Stores.
4. **Maharashtra and Uttar Pradesh are the top two revenue-generating states**, with Bhubaneswar and Nagpur leading at the city level.
5. **Weekday transactions carry a higher average basket value than weekend transactions**, suggesting different shopping behavior (e.g., planned/bulk purchases on weekdays vs. casual weekend visits).
6. **Clothing and Stationery are the most profitable categories by margin** (27.6% and 20.0% respectively), despite contributing far less to total revenue than Electronics.

## Recommendation
Given Electronics' high revenue but low margin, the business should explore renegotiating supplier costs or bundling higher-margin accessories with electronics purchases. Meanwhile, Clothing's strong margins suggest an opportunity to grow that category's share through targeted promotions, especially in top-performing states like Maharashtra and Uttar Pradesh.

## Tools Used
Power BI Desktop, Power Query, DAX

## Report Preview
*(Screenshots of all 4 pages are included in this repository)*

---
**Author:** Komal Verma
