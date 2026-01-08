# Banco Mais: Marketing Strategy & Predictive Targeting

## 1. Background and Overview
Banco Mais is currently dealing with a 40% campaign success rate. This means that for every ten calls they make to sell term deposits, six are a waste of time and resources. I looked at 10,000 customer records to find the specific demographic and financial signals that actually predict a subscription. The goal was to find the specific signals that lead to a subscription so the bank can stop calling people who are likely to say no.

## 2. Data Structure Overview
I used Excel to work through the six steps of the Data Analytics Life Cycle. The dataset included 10,000 rows of information on customer age, jobs, bank balances, and existing loans. To get the data ready for a predictive model, I did a few things:

* I built a data dictionary to define every field and its data type.

* I used IFS functions to bin age groups and XLOOKUP to code categories.

* I ran a regression model to test which variables actually predicted a subscription.

## 3. Executive Summary
The data shows the bank is calling the wrong people. While the average success rate is 40%, people 64 and older convert at 51%. But customers who already have a personal loan only convert at 36%. The quickest way to fix this is to prioritize the 55+ demographic and stop calling people who are in debt. It is important to note that my model only explains a tiny part of why people subscribe. Most of the decision-making factors are still unknown, so while these findings help, they aren't the whole story.

## 4. Insights Deep Dive
**Age as the Primary Driver**
* Age is the strongest predictor I found. The 64+ age group converts at 51%, which is 11% higher than the bank's average. This suggests that older clients care more about the security of a term deposit. Right now, the bank is losing money by not focusing its efforts on these older segments.

**Existing Debt as a Red Flag**
* If a customer has a personal loan, the bank should stop calling them. This group converts at only 36%. Since that's lower than the 40% baseline, these calls are actually pulling the average down. People with debt are likely more focused on their liabilities than starting a new deposit.

**Model Limitations and Reality**
* During the validation phase, I found that while age and debt are statistically significant, they explain less than 1% of the behavior in the data. It was a good lesson in the difference between a signal and a total answer. The findings give the bank a direction for immediate improvement, but most of the factors driving a customer to say yes are still missing from this model.

## 5. Recommendations
* Focus marketing hours and budget on the 55+ and 64+ age groups.

* Remove anyone with a personal loan from the outbound call lists.

* Change the marketing message for older clients to focus on security and fixed rates.

* Use anonymous IDs and encrypted data to protect customer privacy.

* Go back to the data source to find the missing factors that my current model couldn't catch.

---
### 📂 Project Files
* [View Full Analysis Report (PDF)](Assignment%204_%20Validation%20%26%20Communicating%20Results.pdf)
* [View Data Workbook (Excel)](BankMarketing_F25.xlsx)
