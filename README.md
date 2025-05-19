## RFM-ANALYSIS

This project performs (Recency, Frequency,Monetary) analysis to segment customers based on their purchasing behavior. RFM analysis is a powerful marketing tecnique used to identify the most valuable customers by examining how recently and how fequently they purchase, and how much money they spend.


![avp7apgm](https://github.com/user-attachments/assets/39019eda-60c5-4846-82b4-f8cf02891fd0)


## TABLE OF CONTENTS

- [INTRODUCTION](#INTRODUCTION)
- [PROJECT OVERVIEW](PROJECT-OVERVIEW)
- [PROJECT OBJECTIVE](PROJECT-OBJECTIVE)
- [DATA CLEANING](DATA-CLEANING)
- [DATA MINING](DATA-MINING)
- [RECOMMENDATION](RECOMMENDATION)
- [CONCLUSION](CONCLUSION)


## INTRODUCTION: This is a Frequency, Recency, Monetary dataset comprising of 2,216 customers in a super market. 


##PROJECT OVERVIEW: This dataset encompasses 27 columns and 2216 rows in the following sequence;


            Table                                                   Description
|----------------------------------|---------------------------------------------------------------------------------------------------------------------|
|ID                                |    Unique identifier for each customer                                                                              |
|Year_Birth                        |     Year the customer was born                                                                                      |
|Education                         | Level of education attained by the custome                                                                          |
|Marital_Status                    |    Marital status of the customer                                                                                   |
|Income                            | Annual income of the customer (in dollars)                                                                          |
|Kidhome                           | Number of children in the customer's household                                                                      |
|Teenhome                          | Number of teenagers in the customer's household                                                                     |
|Dt_Customer                       | Date when the customer was registered                                                                               | 
|Recency                           |Number of days since the customer last made a purchase                                                               |
|MntWines                          | Amount spent on wines in the last 2 years                                                                           |                           
|MntFruits                         |Amount spent on fruits in the last 2 years                                                                           |
|MntMeatProducts                   | Amount spent on meat products in the last 2 years                                                                   | 
|MntFishProduct                    |Amount spent on fish products in the last 2 years                                                                    |
|MntSweetProduct                   |Amount spent on sweet products in the last 2 years                                                                   |
|MntGoldProds                      |Amount spent on gold products in the last 2 years                                                                    |
-----------------------------------|---------------------------------------------------------------------------------------------------------------------|




## PROJECT OBJECTIVE: 
- Tasks: 1. Database Setup: - Create a new database to store the customer data. - Define appropriate data types for each column and create tables. - Load the dataset into the database. 

- 2. Data Cleaning and Preparation: Identify and handle missing or null values. - Correct data types where necessary (e.g., convert `Income` from string to numeric). - Ensure that date fields are in the correct format. 

- 3. Advanced Querying: - Write complex queries to extract meaningful insights from the data. - Use aggregate functions (SUM, AVG, COUNT, MAX, MIN) to calculate summary statistics. - Implement JOIN operations to combine data from multiple tables if necessary. - Utilize subqueries and common table expressions (CTEs) for more advanced data manipulation.

-  4. Customer Segmentation: - Create segments of customers based on demographics, purchasing behavior, and responses to campaigns. - Write queries to identify top-performing segments based on total spending, frequency of purchases, or campaign responses.

-  5. Marketing Campaign Analysis: - Analyze the effectiveness of different marketing campaigns. - Write queries to calculate the response rates for each campaign. 2 | P a g e - Identify customers who have accepted multiple campaigns and analyze their behavior. 

- 6. Recency, Frequency, Monetary (RFM) Analysis: - Perform an RFM analysis to identify high-value customers. - Write queries to calculate recency, frequency, and monetary value for each customer. - Segment customers into different RFM categories. 

- 7. Optimization and Indexing: - Optimize SQL queries for performance. - Implement indexing strategies to speed up query execution. - Analyze query execution plans to identify and resolve performance bottlenecks.

- 8. Documentation: - Document the database schema and the data cleaning process. - Provide detailed explanations of each query and its purpose. - Include a summary report highlighting the key insights and findings from the analysis. Tools and Technologies.





## DATA CLEANING: In the course of analyzing this dataset, the columns with abnormal data type were altered to the normal data type. 

- A new database named marketing was created for this project.


- 14 new columns were also added to the table, making a sum of 41 columns.


- The data was changed to ```set sql_safe_updates=0;





## DATA MINING: The followings were deduced from this analysis;

- 1.  The customers emanated from 8 countries of the world, having Spain as the country with the highest monetary value of $659,557.00.

- 2.  Spain have the highest number of graduates, post graduates and master degree holders’ of 1093 customers.

- 3.  The married customers spent more in this supermarket with the sum of $855,754 followed by the single customers with the sum of $289,301.


- 4.  The category of customers that accepted campaign were the married customers with a total of 427, followed by the single customers with a total of 137.


- 5. The customers that does not have children were the highest to accept campaign with the sum of 379(57.34%) in the children category.


- 6.  The customers without kids spent more in this supermarket with the sum of $699,662, followed by customers with a kid.

- 7.  The graduates accepted most of the campaign with 339 and they spent the most in the educational category with the sum of $4593,000.

- 8 .  Customers without children are more frequent to this supermarket than those with children.


- 9.   Alpha Generations are most frequent with 811, followed by the Millennials with 728, Generation X =647 and Generation Z = 558.

- 10. The Widow customers are mostly frequent with 728, followed by the complicated with 614, the single=611 and the married =599.


- 11.  The married customers spend more on web purchase with the sum of $5852 followed by the single customers with the sum of $1829.

- 12. The married spent more on purchase with $5852 out of 4 customer categories followed by the single with $1829.

- 13.  The customers were segmented into 3 segments based on recency (5), frequency (5) and monetary (5). 
- The whale customers (>12) = 523

- The moderate customers (<11) = 723

- The lapsed customers (<7) = 990.





## RECOMMENDATION:

- 1.	This organization should make marketing efforts  to the lapsed customers, this might be made to remind them that it’s been a while since their last transaction, while offering them an incentive to resume buying.

- 2.	For the moderate customers, there should be robust mail sent to them to remind them of new products with incentives attached to the products as well as migrating to the whale customers.
	
- 3.	The whale customers should be given loyalty benefits such as gift cards or vouchers with limited expiry date to encourage them to buy more products from the organization.

- 4.	The purchase cycle can be predicted—for example, when a customer needs to buy more groceries—marketing efforts may be directed toward reminding them when to visit the business when staple items run low.
  
- 5.	A natural inclination is to put more emphasis on encouraging customers who spend the most money to continue to do so. While this can produce a better return on investment (ROI) in marketing and customer service, it also runs the risk of alienating customers who have been consistent but may not spend as much with each transaction.

- 6.	The frequency of a customer’s transactions may be predicted by factors such as the type of product, the price point for the purchase, and the need for replenishment or replacement. Predicting this can assist marketing efforts directed at reminding the customer to visit the business again.
	
- 7.	Monetary value should be placed on customers that spend the most money, encouraging them to continue doing so. While this can produce a better return on investment (ROI) in marketing and customer service, it also runs the risk of alienating customers who have been consistent but have not spent as much with each transaction.
  
- 8.	This organization should endeavor to sell products that cut across all the Generations.
	
- 9.	The environment of this business outfit should be ecstatic to guarantee the customers relaxation when they come around.
 

## CONCLUSION



