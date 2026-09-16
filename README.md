# Retail Data Case Study
This is a full Data Analytics case study using a Retail Company's data where we go from cleaning the data, to finding insights and suggesting recommended actions to boost their revenue through targeted marketing campaigns towards their high value and one-time customers.

For the full code, refer to retail-data-case-study saved.ipynb

## Business Task
Analyse customer behaviours and purchasing patterns to find out what affects customer retention and find opportunities to increase repeat purchases. Recommend solutions to promote repeat purchasing and increase revenue from current customers.

## Business Questions
What are the different customer segments?

What factors influence whether customers become repeat customers?

How do one-time customers behave after their purchases?

What are the key differences between one-time and repeat customers?

What opportunities exist to improve customer retention and encourage repeat purchases?

How are current high value customers being treated?

## Tools
Python for Data Cleaning, Data Transformation and Data Analysis. 

Tableau for Data Visualisation.

## Dataset
The dataset is publicly available on [Kaggle](https://www.kaggle.com/datasets/raghavendragandhi/retail-customer-and-transaction-dataset/data).

## Brief Data Overview
This project uses fictional and sample data from various sources within a retail business environment. The dataset combines more than 30,000 purchase transactions, customer demographics, marketing campaigns and support tickets.

The datasets can be primarily linked through customer_id allowing for analysis of customer purchasing patterns, customer engagement and support experiences.

## ER Diagram for datasets used - Lucid Chart

<img src="https://github.com/user-attachments/assets/e663c491-a31d-4cf6-9c54-eeac1c4a0334" width="50%" alt="image" />

## Key Findings
### 1) Age groups 20-29,30-39,40-49 are most frequent and high value spenders. However they aren't being marketed to as aggressively. 
<img width="851" height="665" alt="image" src="https://github.com/user-attachments/assets/5b86f7ac-6941-4c5a-bc31-3d713ac3688f" />
<img width="920" height="460" alt="image" src="https://github.com/user-attachments/assets/7cb916c9-2a28-4187-b067-c3424334d970" />


We find that the 3 customers segments : Adults, High-value Customers and Loyal customers which fit the ages 20 to 49, have fewer marketing campaigns and are not being targeted aggressively enough although they bring in majority of sales revenue. 

### 2) One-time customers are significantly (57%) less likely to complete their purchase interactions.
<img width="914" height="258" alt="image" src="https://github.com/user-attachments/assets/c13ebdfe-205d-464a-9835-d5d23069fda3" />
<img width="921" height="638" alt="image" src="https://github.com/user-attachments/assets/b2fbb8b9-8dae-4b0d-8989-838ca6269fc3" />

One-time customers are more likely to abandon the final stage of purchasing which is filling in payment details. We identified the payment stage as the drop-off point after discovering that purchase interactions exceeded completed transactions. Specifically, one-time customers logged more purchase interactions than repeat customers which is a pattern that is only possible if users are abandoning the process of filling in payment details. Therefore purchase interactions refer to pressing of the purchase button and not completed transactions.

### 3) One-time customers have much higher, high intent interactions specifically checkouts that increase with time after their first transaction.
This are days after their first transaction.
<img width="915" height="162" alt="image" src="https://github.com/user-attachments/assets/ce8d3902-0b1d-40bb-b9b8-e767e26a7340" />

The biggest difference is in checkout interactions where they had 1.5x more interactions.
<img width="926" height="267" alt="image" src="https://github.com/user-attachments/assets/2549074b-5369-441f-ba12-9fe5b31f647e" />

## Recommended Actions
### For the first finding: Age groups 20-29,30-39,40-49 are most frequent and high value spenders. However they aren't being marketed to as aggressively. 

The recommendation is to increase the number of campaigns for these customer segments, specifically campaign types that have higher ROIs, lower cost per conversions and average conversions per 1000 dollars spent. We analysed the campaigns ran for each customer segment and split them into either online, store or other campaign types with the code below.  

<img width="1092" height="606" alt="image" src="https://github.com/user-attachments/assets/715644ef-8f82-465a-b166-4c6e5a0a4315" />

We then find out which campaign types have performed the best. Refer below. 


<img width="1097" height="576" alt="image" src="https://github.com/user-attachments/assets/88da2871-de7d-4ac6-8783-5e7aeed4117d" />


After repeating the process for all 3 customer segments we find that for the 'Adults (26-40)' customer segment, "Other" campaign types work the best. Specifically, they should focus on Print and Radio Advertisement. 

For the 'High-Value Customers' customer segment, "Online" campaign types work the best. Specifically, they should focus on Online Display Ads and Social Media.

<img width="1091" height="574" alt="image" src="https://github.com/user-attachments/assets/4dc8548c-d20a-4c65-aee3-e665aed26cf9" />

For the 'Loyal Customers' customer segment, "Online" campaign types work the best. Specifically, they should focus on Social Media and Online Display Ads.

<img width="1093" height="492" alt="image" src="https://github.com/user-attachments/assets/67eb26f5-b9c6-4476-ad4b-21bc8d4bb6ad" />


### For the remaining findings, we first do process mapping to visualise the customer journey.

## Process Mapping - Customer Journey

The mapping below illustrates the customer journey from start to purchase.

<img src="https://github.com/user-attachments/assets/59ab739b-26cb-4a9c-bba3-5a694ca3297c" width="30%" alt="image"/>

From our analysis we found that customer drop offs for one time customers happens after the purchase interaction. This is the page where customers key in payment details and hit confirm to save their details (refer below.)

<img width="30%" height="30%" alt="image" src="https://github.com/user-attachments/assets/4dc125d0-fdbc-4878-bc3c-e81a7723e775" />

Furthermore one time customers' biggest issue is billing and when compared to repeat customers, they have proportionately more. This further solidifies the need to address the final payment section of the customer journey for one time customers.


<img width="100%" alt="image" src="https://github.com/user-attachments/assets/f1aa4a83-3d48-4cbf-ade1-4cd927f7850a" />

## Recommended Actions (cont'd)

### For the second finding: One-time customers are significantly (57%) less likely to complete their purchase interactions.

Firstly, a new interaction_type called 'completed_transactions' should be created to accurately track completed purchases as the current 'purchases' interaction_type only measures the number of clicks on the purchase button and not completed transactions. 

The recommended action is to run a Checkout Abandonment Campaign that would target one-time customers who initiate checkout but do not proceed to a completed purchase interaction. The campaign would focus on recovering immediate purchase opportunities. 

Refer below for the campaign workflow:

<img width="50%" height="50%" alt="image" src="https://github.com/user-attachments/assets/47d1b79a-944d-4d2b-a0be-2babbe4d2b88" />
<p></p>

The initial reminder can be a personalised email to remind the customer about the checkout that they have started. It should contain a direct link to the checkout rather than to the website home page.

If the customer does not return, a second reminder should be sent after 24-48 hours and it could introduce a small incentive such as: Free shipping, Discount Code, Loyalty points etc. If there is still no purchase, the campaign should be exited and the data should be monitored through KPIs that will be introduced below.

### To complement the above solution, billing issues faced by one-time customers have to be addressed as well.

The main issues that customers face are 'Billing address verification failed during checkout' and 'Customer couldn't apply discount code at checkout'.

<img width="1184" height="228" alt="image" src="https://github.com/user-attachments/assets/9ec6057b-b9fc-47d5-9299-83b3c6f1a55a" />

For the address verification, if it fails, some of the options are as follows:
- Prompt the customer to correct their address
- Provide suggested address options where possible
- Allow the customer to retry without restarting checkout
- To provide easy support escalation through live chatbots

For the failed discount codes, some of the options are as follows:
- Display proper error codes such as expired, minimum spend not met rather than "invalid code"
- If there are eligible alternative promotions, to suggest them to the customer
- If the fault is on the company such as the customer actually being eligible, to immediately flag the issue and assign high urgency

### For the third finding: One-time customers have much higher, high intent interactions (specifically checkouts) that increase with time after their first transaction.

The recommended action is to run a personalised re-engagement campaign. This are customers who although only have one purchase, still show high-intent interactions. Instead of waiting for the customer to abandon checkout, the business should proactively engage them. 

The campaign would monitor post-purchase interactions such as product views, search, wish list additions to identify the products or categories a customer is interested in. personalised product recommendations can then be presented through website pop-ups or sent through the customer's preferred communication channel, such as email. 

If the customer subsequently adds a product to their cart or reaches checkout but does not complete their purchase, they would be transferred to the Checkout Abandonment campaign which focuses on recovering the abandoned purchased opportunity. This creates a continuous re-engagement process.

## KPIs to track to see if recommended actions prove successful. 

This section outlines the KPIs to be tracked for each solution.

### For the first solution for customers aged 20-49, 
no_of_campaigns = sum of campaigns per customer segment <- should increase by at least 5 per customer segment (Adult, Loyal, High-value)
cost_per_conversion = budget / conversions <- (<103 for Adults, <159 for Loyal <120 for High-value)
conversion_per_1000 = conversions / budget <- (>26 for Adults, >13 for Loyal, >16 for High-value)
roi <- (>944 for Adults, >387 for Loyal, >1704 for High-value)

The numbers are taken from the recommendations for finding one.

### For the second solution for one-time customers to complete their transactions,


## Conclusion









