# Customer Segmentation Analysis

The dataset looks sales of bikes and bike-related products, along with customer and product data.

## Business Problem: How can we increase revenue?

The goal was to identify **customer segments** and retention strategies to increase revenue.
I grouped customers into 3 segments based on their spending behaviour:
1. **VIP**: Customers with at least 12 months of history and spending more than 5,000
2. **Regular**: Customers with at least 12 months of history but spending 5,000 or less
3. **New**: Customers with a lifespan less than 12 months
   
Tools used: SQL, Excel

## Workflow
## Step 1: Which customer segment generated the most revenue?
### Revenue concentration
The biggest proportion of customers were new (nearly 80%).
VIP customers made up only 9% of all customers.

![img_alt](https://github.com/Comp-coder-4/Customer-Segmentation-Analysis/blob/6753ca55f85c183d50cf5acc64602bb5b81c0390/Screenshot%202026-09-30%20104523.png)

Then we look at the total revenue and percentage contribution from each customer segment. Things look very interesting...
Although VIP make up just 9% of all customers, they contributed only 1.1% less revenue than New customers (which make up ~80% of all customers)!

![img_alt](https://github.com/Comp-coder-4/Customer-Segmentation-Analysis/blob/969fe618e937cbe4a14e0a3ae62358df12109fd1/Screenshot%202026-09-30%20110217.png)

This is a good indicator that VIP's are generating more revenue per customer.

### Average Order Value
As expected, VIP has highest average order value (AOV). 

![img_alt](https://github.com/Comp-coder-4/Customer-Segmentation-Analysis/blob/2d785bcf65ccbd14bb9a79d37441c834eb673ff2/Screenshot%202026-09-30%20113444.png)

This further confirms that VIP's are generating most revenue. It could be useful to create strategic ways to encourage regular customers to become VIP, which we will see in the analysis soon...

### Moving forward: 
We've found that VIP customers bring highest revenue concentration and average order value.
Our target now is to find where we can make effort to increase customer retention and upsell customers in order to increase revenue.

Aim:
1. Retain VIP customers
2. Upsell regular customers to VIP

## Step 2: Are any customers nearly at the VIP threshold?
A regular customer is *__likely to become VIP__* if they have a lifespan of at least 12 months and their total spending is between 4500 and 5000 (VIP total spending threshold = 5000)

![img_alt](https://github.com/Comp-coder-4/Customer-Segmentation-Analysis/blob/89185f059df0dd3dc3ed7bbfe62ab89c2b66971d/Screenshot%202026-09-30%20115938.png)

20% of regular customers are likely to become VIP

### Recommendation:
Give customers near the VIP threshold a loyalty reward that offers 15-20% discount on an upgraded version of a bike that the customer has already purchased. This would encourage the customer to repeat an order with a higher order value, thus increasing revenue.

## Step 3: How do we retain VIP customers?
We'll start off by looking at sales performance by VIP customers:

![img_alt](https://github.com/Comp-coder-4/Customer-Segmentation-Analysis/blob/e6adeb6df27bf86b3974929d19b146cdb532846c/Screenshot%202026-09-30%20144426.png)

The 5-month moving average (orange) shows underlying trends clearer.
- In 2013, sales peaked between May and August
- Both in 2011 and 2013, the sales were higher from Sept and Dec compared with Jan to April

Sales should be kept at the level it was in 2013. Let's look at Month-On-Month sales performance by VIP customers to see how to do this...

![img_alt](https://github.com/Comp-coder-4/Customer-Segmentation-Analysis/blob/5f334c42eccb97d3c373be708dce885e2a6acd92/Screenshot%202026-09-30%20145905.png)

VIP Sales are highest in summer months.

### Recommendation
To ensure sales are kept at this level in the next year, I recommend offering premium service including exclusive access to new bikes and a fast delivery option for VIP customers in late spring to encourage more customers to make a purchase. This can help boost sales just before and during summer months since this is the time of year people look to purchase bikes.

It would be worth offering the same premium service (exclusive access to new bikes) and faster delivery options for VIP customers in months between September and December as well, since sales are high during this time of year.

-----------------------------------

## Key Insights & Recommendations
1. **Insight:** 20% of Regular customers are near the VIP threshold.
   **Recommendation:** Loyalty reward which offers 15-20% discount on an upgraded version of a bike the customer has already purchased. The business could do a family bundle deal for bikes to increase the order value and spending
2. **Insight:** Looking at the Month-on-Month VIP performance, sales are highest during summer months.
   **Recommendation:** To ensure sales are kept this way, I recommend offering premium service including exclusive access to new bikes and fast delivery option

## File Structure
All files are numbered.
- Exploratory Data Analysis:
  - Each file has a number and 'EDA'
  - Files numbered from 01 to 06. Example: 01_EDA_Database_Exploration
- Customer Segmentation Analysis:
  - **07_Customer_Segmentation.sql**
- Customer Retention Analysis:
  - **08_Customer_Retention.sql**
  - **08_Customer_Retention_VIP_Performance.xlsx**

Bonus:
- There is also a Customer Report and Product Report in sql files numbered 09 and 10
___________
This project is a continuation of what I completed as part of Data with Baraa's "SQL Mastery for Data Analytics and Business Intelligence" course and my own ideas. I gave the project a business problem and business context.

Data credit: Data Wih Baraa
