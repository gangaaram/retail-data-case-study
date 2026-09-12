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

### 2)<u> One-time customers are significantly (57%) less likely to complete their purchase interactions.</u>
<img width="914" height="258" alt="image" src="https://github.com/user-attachments/assets/c13ebdfe-205d-464a-9835-d5d23069fda3" />
<img width="921" height="638" alt="image" src="https://github.com/user-attachments/assets/b2fbb8b9-8dae-4b0d-8989-838ca6269fc3" />

One-time customers are more likely to abandon the final stage of purchasing which is keying in the card information. We found out that purchase interactions don't mean completed transactions as they had more purchase interactions than repeat customers and therefore purchase interactions refer to pressing of the purchase button.

### 3) One-time customers have much higher, high intent interactions specifically checkouts that increase with time after their first transaction.
This are days after their first transaction.
<img width="915" height="162" alt="image" src="https://github.com/user-attachments/assets/ce8d3902-0b1d-40bb-b9b8-e767e26a7340" />
The biggest difference is in checkout interactions where they had 1.5x more interactions.
<img width="926" height="267" alt="image" src="https://github.com/user-attachments/assets/2549074b-5369-441f-ba12-9fe5b31f647e" />

### 4) One time customers' biggest issue is billing and when compared to repeat customers they have proportionately more.
<img width="923" height="731" alt="image" src="https://github.com/user-attachments/assets/f1aa4a83-3d48-4cbf-ade1-4cd927f7850a" />

## Recommended Actions
### For the first finding: Age groups 20-29,30-39,40-49 are most frequent and high value spenders. However they aren't being marketed to as aggressively. 

The recommendation is to increase the number of campaigns for these customer segments focus on marketing campaigns types that have higher ROIs, lower cost per conversions and average conversions per 1000 dollars spent. We analysed the campaigns ran for each customer segment and split them into either online, store or other campaign types with the code below.  

<img width="955" height="682" alt="AdobeExpressPhotos_7b62e8aa11a643ba9499ead597b8346d_CopyEdited" src="https://github.com/user-attachments/assets/87aec91b-dd6b-45b2-823b-2731162ec85a" />

We then find out which campaign types have performed the best. Refer below. 

<img width="1065" height="477" alt="image" src="https://github.com/user-attachments/assets/ea42cb8f-b64a-4725-bb73-fede619f54d4" />

After repeating the process for all 3 customer segments we find that for the Adults (26-40) customer segment, "Other" campaign types work the best. Specifically, they should focus on 

## Process Mapping

## KPIs to track to see if recommended actions prove successful. 










