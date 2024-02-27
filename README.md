# Sales_Insights_DataAnalysis-

Data Analysis Project on Sales Insights using MySQL, PowerBI

The following steps were done to do the analysis:
1. Understand the Problem statement :
       Atliq Global - A hardware company which sells the manufacturing parts wants to know about their sales insights (the company wants to track their sales in 
       the dynamically growing market) since the overall sales is declining.
2.Data Discovery
   Analyse the Data obtained from Falcon company (Atliq global uses the Falcon software for billing purposes)
3. Data Analysis using SQL:
   The data obtained from Falcon company has the following tables sales_market, sales_transaction, sales_product, sales_customer and sales_date.
   Execute the below Queries in Mysql to analyse the data:
   Select * from sales_market
   select * from sales_transaction
   select * from sales_product
   select * from sales_date
   select * from sales_customer
   select DISTINCT(transactions.currency)  from transactions
   select * from transactions where sales_amount='-1' or sales_Amount='0'
   select count(*) from transactions where currency='INR\r' 
   select * from transactions where currency='USD' or currency='USD\r'
   

   Once the above queries are executed the following observations were made:
   currency has both INR and USD.
   sales amount has 0 or -1.
   there are duplicate records in the database.

5. Data Cleaning and ETL in Power BI
   We find the data forms a star schema where sales transaction is the fact table and the remianing are dimension table
   To Clean the data below steps are performed in Power BI
   1. USD is converted to INR
   2. Duplicate records are removed and the rows were removed where sales amount is 0 or -1

5 Build POWER BI DASHBOARD
6. Feedback from Stakeholders
7. Publish a Report

   

 
   
   
   
 


