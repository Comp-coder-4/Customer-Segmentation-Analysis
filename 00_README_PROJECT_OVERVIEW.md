# Bike Sales Analytics: Customer Segmentation Analysis

The dataset looks at bike and other bike-related product sales, along with customer data and product data.

## Business Problem: How can we increase revenue?

The goal was to identify **customer segments** and retention strategies to increase revenue.
I grouped customers into 3 segments based on their spending behaviour:
1. **VIP**: Customers with at least 12 months of history and spending more than 5,000
2. **Regular**: Customers with at least 12 months of history but spending 5,000 or less
3. **New**: Customers with a lifespan less than 12 months
   
Tools used: SQL, Excel

## Workflow
## Step 1: Which customer segment generated the most revenue?
The biggest proportion of customers were New (nearly 80%).
VIP customers made up only 9% of all customers.

![img_alt](https://github.com/Comp-coder-4/Customer-Segmentation-Analysis/blob/6753ca55f85c183d50cf5acc64602bb5b81c0390/Screenshot%202026-09-30%20104523.png)

Then we look at the total revenue and percentage contribution from each customer segment. Things look very interesting...
Although VIP make up just 9% of all customers, they contributed only 1.1% less revenue than New customers (which make up ~80% of all customers)!

![img_alt](https://github.com/Comp-coder-4/Customer-Segmentation-Analysis/blob/969fe618e937cbe4a14e0a3ae62358df12109fd1/Screenshot%202026-09-30%20110217.png)

This is a good indicator that VIP's are generating more revenue per customer.

## Key Insights & Recommendations
1. **Insight:** 20% of Regular customers are near the VIP threshold.
   **Recommendation:** Loyalty reward which offers 15-20% discount on an upgraded version of a bike the customer has already purchased. The business could do a family bundle deal for bikes to increase the order value and spending
2. **Insight:** Looking at the Month-on-Month VIP performance, sales are highest during summer months.
   **Recommendation:** To ensure sales are kept this way, I recommend offering premium service including exclusive access to new bikes and fast delivery option

## File Structure
All files are numbered.
- Exploratory Data Analysis SQL files are numbered from 01 to 06 and are labelled with 'EDA'. Example: 01_EDA_Database_Exploration.
- Customer Segmentation Analysis: file numbered 07.
- Customer Retention Analysis: files numbered 08.

Bonus:
- There is also a Customer Report and Product Report in sql files numbered 09 and 10
___________
This project is a continuation of what I completed as part of Data with Baraa's "SQL Mastery for Data Analytics and Business Intelligence" course and my own ideas. I gave the project a business problem and business context.

Data credit: Data Wih Baraa
