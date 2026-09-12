# Retail Data Case Study
This is a full Data Analytics case study using a Retail Company's data where we go from cleaning the data, to finding insights and suggesting recommended actions to boost their revenue through targeted marketing campaigns towards their high value and one-time customers.

For the full code, refer to retail-data-case-study.ipynb

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

## ER Diagram for Datasets used - Lucid Chart

<img src="https://github.com/user-attachments/assets/e663c491-a31d-4cf6-9c54-eeac1c4a0334" width="50%" alt="image" />

## Key Findings
### 1) Age groups 20-29,30-39,40-49 are most frequent and high value spenders. However they aren't being marketed to as aggressively. 
<img width="851" height="665" alt="image" src="https://github.com/user-attachments/assets/5b86f7ac-6941-4c5a-bc31-3d713ac3688f" />
<img width="920" height="460" alt="image" src="https://github.com/user-attachments/assets/7cb916c9-2a28-4187-b067-c3424334d970" />


We find that the 3 customers segments : Adults, High-value Customers and Loyal customers have fewer marketing campaigns and are not being targeted aggressively although they bring in majority of sales revenue. 

### 2) One-time customers are significantly (57%) less likely to complete their purchase interactions.
<img width="914" height="258" alt="image" src="https://github.com/user-attachments/assets/c13ebdfe-205d-464a-9835-d5d23069fda3" />
<img width="921" height="638" alt="image" src="https://github.com/user-attachments/assets/b2fbb8b9-8dae-4b0d-8989-838ca6269fc3" />

One-time customers are more likely to abandon the final stage of purchasing which is keying in the card information. We found out that purchase interactions don't mean completed transactions as they had more purchase interactions than repeat customers and therefore purchase interactions refer to pressing of the purchase button.

### 3) One-time customers have much higher, high intent interactions specifically checkouts that increase with time after their first transaction.
This are days after their first transaction.
<img width="915" height="162" alt="image" src="https://github.com/user-attachments/assets/ce8d3902-0b1d-40bb-b9b8-e767e26a7340" />
The biggest difference is in checkout interactions where they had 1.5x more interactions.
<img width="926" height="267" alt="image" src="https://github.com/user-attachments/assets/2549074b-5369-441f-ba12-9fe5b31f647e" />

## Recommended Actions
### For the first finding: Age groups 20-29,30-39,40-49 are most frequent and high value spenders. However they aren't being marketed to as aggressively. 

The recommendation is to increase the number of campaigns for these customer segments focus on marketing campaigns types that have higher ROIs, lower cost per conversions and average conversions per 1000 dollars spent. We analysed the campaigns ran for each customer segment and split them into either online, store or other campaign types with the code below.  

<img width="955" height="682" alt="AdobeExpressPhotos_7b62e8aa11a643ba9499ead597b8346d_CopyEdited" src="https://github.com/user-attachments/assets/87aec91b-dd6b-45b2-823b-2731162ec85a" />

We then find out which campaign types have performed the best. Refer below. 

<img width="1065" height="477" alt="image" src="https://github.com/user-attachments/assets/ea42cb8f-b64a-4725-bb73-fede619f54d4" />

After repeating the process for all 3 customer segments we find that for the 'Adults (26-40)' customer segment, "Other" campaign types work the best. Specifically, they should focus on Print and Radio Advertisement. 

<img width="1839" height="404" alt="AdobeExpressPhotos_72757fc574af46179b80bd571feaef0e_CopyEdited" src="https://github.com/user-attachments/assets/74e23b50-bed8-41d1-9ee6-af7335b8e65e" />

For the 'High-Value Customers' customer segment, "Online" campaign types work the best. Specifically, they should focus on Online Display Ads and Social Media.

<img width="1848" height="545" alt="AdobeExpressPhotos_d034618b4d3a420490bf4c90036bb5db_CopyEdited" src="https://github.com/user-attachments/assets/9cb7354e-b114-4be6-81c3-e4217f3c1f18" />

For the 'Loyal Customers' customer segment, "Online" campaign types work the best. Specifically, they should focus on Social Media and Online Display Ads.

<img width="1842" height="466" alt="AdobeExpressPhotos_f1df897298d548fca5b47b952f5bb759_CopyEdited" src="https://github.com/user-attachments/assets/de316861-d28c-4399-b6bf-74585a9465b7" />

### For the remaining findings, we first do process analysis to visualise the customer drop offs during the customer journey.

## Process Mapping - Customer Journey

The mapping below illustrates the customer journey from start to purchase.

<img src="https://github.com/user-attachments/assets/59ab739b-26cb-4a9c-bba3-5a694ca3297c" width="50%" alt="image"/>

From our analysis we found that customer drop offs for one time customers happens after the purchase. This is the page where customers key in payment details and hit confirm to save their details (refer below.)

<img width="50%" height="50%" alt="image" src="https://github.com/user-attachments/assets/4dc125d0-fdbc-4878-bc3c-e81a7723e775" />



Furthermore one time customers' biggest issue is billing and when compared to repeat customers they have proportionately more. This further solidifies the need to address the final payment section of the customer journey for one time customers.


<img width="100%" alt="image" src="https://github.com/user-attachments/assets/f1aa4a83-3d48-4cbf-ade1-4cd927f7850a" />

## Recommended Actions (cont'd)

### For the second finding: One-time customers are significantly (57%) less likely to complete their purchase interactions.

The recommended action is to 

### For the third finding: One-time customers have much higher, high intent interactions specifically checkouts that increase with time after their first transaction.

## KPIs to track to see if recommended actions prove successful. 










