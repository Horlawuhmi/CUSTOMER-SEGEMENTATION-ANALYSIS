# CUSTOMER-SEGEMENTATION-ANALYSIS
Customer segmentation is the process of dividing a customer base into distinct groups of individuals that share similar characteristics. These characteristics can include demographics, psychographics, purchasing behavior, and customer preferences.
# INTRODUCTION
The purpose of this project is to conduct an indepth customer segmentation analysis. This involves categorizing customers into unique segments based on common characteristics and attributes. By doing so, the analysis aims to derive insights that can help businesses define and refine their marketing strategies, leading to better customer engagement and satisfaction.
# ABOUT THE DATA
Data was imported into Excel for analysis, there are 2241 rows and 27 columns, the content includes:

People

* ID: Customer’s unique identifier
* Year_Birth: Customer’s birth year
* Education: Customer’s education level
* Marital_Status: Customer’s marital status
* Income: Customer’s yearly household income
* Kidhome: Number of children in customer’s household
* Teenhome: Number of teenagers in customer’s household
* Dt_Customer: Date of customer’s enrollment with the company
* Recency: Number of days since customer’s last purchase
* Complain: 1 if the customer complained in the last 2 years, 0 otherwise

Products

* MntWines: Amount spent on wine in last 2 years
* MntFruits: Amount spent on fruits in last 2 years
* MntMeatProducts: Amount spent on meat in last 2 years
* MntFishProducts: Amount spent on fish in last 2 years
* MntSweetProducts: Amount spent on sweets in last 2 years
* MntGoldProds: Amount spent on gold in last 2 years

Promotion

* NumDealsPurchases: Number of purchases made with a discount
* AcceptedCmp1: 1 if customer accepted the offer in the 1st campaign, 0 otherwise
* AcceptedCmp2: 1 if customer accepted the offer in the 2nd campaign, 0 otherwise
* AcceptedCmp3: 1 if customer accepted the offer in the 3rd campaign, 0 otherwise
* AcceptedCmp4: 1 if customer accepted the offer in the 4th campaign, 0 otherwise
* AcceptedCmp5: 1 if customer accepted the offer in the 5th campaign, 0 otherwise
* Response: 1 if customer accepted the offer in the last campaign, 0 otherwise

Place

* NumWebPurchases: Number of purchases made through the company’s website
* NumCatalogPurchases: Number of purchases made using a catalogue
* NumStorePurchases: Number of purchases made directly in stores
* NumWebVisitsMonth: Number of visits to company’s website in the last month



# Analysis to be conducted with the data

* Customer Demographics Analysis
* Household Composition Analysis
* Customer Behavior Analysis
* Product Purchase Analysis
* Promotion Response Analysis
* Purchase Channel Analysis

# Data Cleaning and Exploration

The income column had 25 missing values, which was formatted to currency type, this was replaced with the median value. The column also had an outlier value ‘$66,666,666’ which was removed.

![median replace](https://github.com/user-attachments/assets/e78c7c5b-f6bb-4ca5-b184-3bea195058be)  

The Year_Birth column was further converted into age using the present year(2024) to calculate the age of customers.
There were no duplicate values.

![age calculation](https://github.com/user-attachments/assets/e8dbe90c-8e27-498d-a885-7c8928822f60)


# Customer Segmentation Analysis
![count by edu](https://github.com/user-attachments/assets/e46d5014-56b8-4971-9133-bfa00041d8c4)       
_Education Level Analysis: Distribution of education levels among customers._

![COUNT OF MARRIAGE](https://github.com/user-attachments/assets/b9a64448-62e9-4fd5-a3fc-f0f71326c31c)      
_Marital Status Analysis: Distribution of marital status categories._

![age group](https://github.com/user-attachments/assets/27542c65-ce99-43f4-a1ba-4645d46bdd1d)      
The age column was converted into age groups for proper analysis and segementation with 20 years difference.

![count by age grioup](https://github.com/user-attachments/assets/d96a3161-26ed-467c-923f-ad06cb9110dc)      
_Age Distribution: Calculated the age of customers using the Year_Birth and the age distribution._

![income calc](https://github.com/user-attachments/assets/8caa1ab1-1e28-4e62-bb7c-dfa4329eb802)      
_Income: Distribution of household income BY Average and standard deviation._
The mean gives an idea of the average income level, but without knowing the standard deviation, we don’t know how representative that average is. The standard deviation tells how much incomes vary around the average, giving insight into the spread and inequality of the income distribution.

![income range](https://github.com/user-attachments/assets/39c55689-825a-46dd-9e9d-521a0e5f57a4)       
_Customer segementation based on income_

# Household Composition Analysis

![kid vs teen](https://github.com/user-attachments/assets/98d4d0ca-af03-4220-a66b-f98b70e057a7)           
_Distribution of households with children (Kidhome) and teenagers (Teenhome)_

![no of children](https://github.com/user-attachments/assets/96e098a8-6041-4e6a-af87-dbce28f0f3de)         
_The total number of kid and teenagers in each household and analyze the household size distribution_

# Customer Behavior Analysis

![complaint analysis](https://github.com/user-attachments/assets/2012c092-abe5-457a-ad3b-1205ac7655a8)    
_Complaint Analysis: The percentage of customers who have complained in the last 2 years (Complain)_  

![renencyy](https://github.com/user-attachments/assets/0a81610d-f656-49a5-bd57-6cc8298b992f)   
_Recency Distribution: Number of days since customer’s last purchase_

![response](https://github.com/user-attachments/assets/4e1f7078-1559-40c2-b33c-f047969ccb54)    
_Response Distsribution: Total number of customer response to all campaign_

![spent range](https://github.com/user-attachments/assets/6d26ad90-4816-421f-9491-407896e1e064)      
_Purchase analysis: Total spent by customers in a range_

# Product Purchase Analysis

![prodct catg](https://github.com/user-attachments/assets/7d0f5b33-b726-484c-88ae-2cacc222efc6)     
_The total amount spent on different product categories_

![avg spent by age group](https://github.com/user-attachments/assets/41db2337-82c6-4b6a-a6fc-6f1d7b70ebb1)     
_Average income spent on each products by Age group_

![avg speny by marital](https://github.com/user-attachments/assets/9201185f-0db5-4582-8e00-5dcc29a5e87b)        
_Average income spent on each products by Marital status_

Total amount spent and the average on each product shows “MntWines” was the most purchased product.

# Promotion Response Analysis

![acpt rate of cmp](https://github.com/user-attachments/assets/ca16fa22-7920-416c-84ff-baed27ebd6b4)        
_Campaign Effectiveness: Analyzed the acceptance rates of various campaigns (AcceptedCmp1 to AcceptedCmp5, Response)_

# Purchase Channel Analysis

![total and avg purchase](https://github.com/user-attachments/assets/f1feb3ae-e165-40c2-a386-119d4e59e916)       
_Online vs Offline: Compare the number of purchases made through the website (NumWebPurchases), catalog (NumCatalogPurchases), and in stores (NumStorePurchases)_

![webvisit](https://github.com/user-attachments/assets/3dc48894-e37c-41bc-9b35-e7509a23125d)     
_Website Engagement: Analyzed the frequency of website visits in the last month (NumWebVisitsMonth)_

# Insights and Recommendations

* Customer Demographic Analysis
  
Education: Graduation had the highest count of customers at 1,126, followed by PhD with 486, and the least was Basic education at 54.

Recommendation: Focus marketing and engagement strategies on graduates and PhD holders, as they represent a significant portion of the customer base.

Marital Status: Married individuals had the highest count at 864, followed by ‘Together’ at 579, with ‘YOLO’ and ‘Absurd’ having the least at 2 each.

Recommendation: Tailor campaigns to married customers and those in relationships, as they form the majority of the customer base.

Age Group: The 40–59 age group had the highest count at 1,232, followed by 60–79 at 767.

Recommendation: Develop age-specific products and marketing strategies targeting the 40–59 age group, as they constitute the largest segment.

Income: Customers aged 80 and above had the highest average income at $63,957, followed by 60–79 at $57,074, with the 20–39 age group having the least at $46,341.

Recommendation: Design premium products and services for older customers who have higher average incomes.

Income Range: Customers with income between $20,000-$50,000 had the highest count at 933, while those earning below $20,000 were 127.

Recommendation: Focus on offering value-based products for the largest income group ($20,000-$50,000) and explore ways to engage lower-income customers.

* Household Composition Analysis
  
Teenhome: Homes with 0 teens were 1,157, 1 teen at 1,030, and 2 teens at 52.
Kidhome: Homes with 0 kids were 1,293, 1 kid at 898, and 2 kids at 48.
Total Children: The total number of homes with 0 children was highest, with 1,293 homes for kids and 1,157 homes for teens.

Recommendation: Create family-oriented products and services, targeting households with children.

* Customer Behavior Analysis
  
Complaints: Out of 2,240 customers, 21 complained, representing 0.94%, while 2,219 were satisfied (99.1%).

Recommendation: Maintain high satisfaction levels and address the root causes of the few complaints to further improve customer retention.

Recency: The 0–30 days range had the highest recency count at 723, while 91+ days had the least at 198.

Recommendation: Implement retention strategies for customers with a recency of 91+ days to re-engage them.

Campaign Response: 0–1 campaign responses had the highest count at 2,000, while 4+ responses had the least at 46.

Recommendation: Optimize campaign strategies to increase engagement rates across all campaigns.

* Product Purchase Analysis
  
Total Spend: The highest spending range was <=$500 with 1,245 customers, while $2,000+ had the least customers at 50.
Top Products: ‘MntWines’ had the highest total spending at $680,807, followed by ‘MntMeatProducts’ at $373,950, and ‘MntFruits’ had the least at $58,908.

Recommendation: Continue promoting top-performing products and explore strategies to increase spending on lower-performing products.

Age and Marital Status: All age groups and marital statuses had the highest average spending on ‘MntWines’ and the lowest on ‘MntFruits’. 

Recommendation: Focus promotional efforts on high-spending categories like wines and meats while identifying opportunities to boost fruit product sales.

* Promotion Response Analysis
  
Campaign Effectiveness: The acceptance rate across all campaigns was 7%.

Recommendation: Review and refine campaign strategies to improve acceptance rates and overall campaign effectiveness.

* Purchase Analysis
  
Online vs Offline: Website purchases totaled 9,147 (avg 4.09), catalog purchases were 5,962 (avg 2.66), and in-store purchases were 12,967 (avg 5.79).

Recommendation: Enhance the online shopping experience to increase web purchases and balance the distribution between online and offline channels.

Website Engagement: Website visits ranged from 0 to 20, with the highest frequency at 20 (2,235 visits) and the lowest at 0 (11 visits).  

Recommendation: Develop strategies to increase website engagement and visits, especially focusing on customers with low visit frequencies.

# Conclusion
By analyzing customer demographics, household composition, behavior, product purchases, and promotion responses, businesses can gain important insights into their customer base. 

These insights can inform targeted marketing strategies, product development, and customer engagement initiatives,driving growth and customer satisfaction. Continuous monitoring and optimizing these factors will help businesses with long-term success and competitiveness in the market.









