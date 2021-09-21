# Spotify-Winter-2022-Data-Science-Intern-Challenge
# Data-Science-Challenge

## Question 1:

 Given some sample data, write a program to answer the following: (link to data set here https://docs.google.com/spreadsheets/d/16i38oonuX1y1g7C_UAmiK9GkY7cS-64DfiDMNiR41LM/edit#gid=0)
 
 On Shopify, we have exactly 100 sneaker shops, and each of these shops sells only one model of shoe. We want to do some analysis of the average order value (AOV). When we look at orders data over a 30 day window, we naively calculate an AOV of $3145.13. Given that we know these shops are selling sneakers, a relatively affordable item, something seems wrong with our analysis. 

1. Think about what could be going wrong with our calculation. Think about a better way to evaluate this data.
2. What metric would you report for this dataset?
3. What is its value?

## Answers: 

1. The incorrect AOV calculation of $3145.13 was most likely arrived at by mistakenly calculating the total_items with the count() function instead of sum(). Whereas count() will only provide the total count of the number of rows, sum() will more accurately provide the AOV value by adding together all of the values in the total_items column. 

2. To determine the correct Average Order Value (AOV), the reporting metrics are the respective sums of both 'order_amount' and 'total_items':<br/>

   sum_orderAmount = df['order_amount'].sum()\
   sum_totalItems = df['total_items'].sum()

   Next divide the total order amount (sum_orderAmount) by the total items amount (sum_totalItems).Hence\
   AOV = sum_orderAmount/sum_totalItems

3. The Average Order Value (AOV) is: $357.92 

VIEW CODE HERE: https://github.com/Creative-Dave/Spotify-Winter-2022-Data-Science-Intern-Challenge/blob/main/Winter%20Data%20Science%20Challenge.ipynb

## Question 2: 

For this question you’ll need to use SQL. Follow this link (https://www.w3schools.com/SQL/TRYSQL.ASP?FILENAME=TRYSQL_SELECT_ALL) to access the data set required for the challenge. Please use queries to answer the following questions. Paste your queries along with your final numerical answers below.

1. How many orders were shipped by Speedy Express in total?
2. What is the last name of the employee with the most orders?
3. What product was ordered the most by customers in Germany?

## Answers: 

1. How many orders were shipped by Speedy Express in total? 
       \54


2. What is the last name of the employee with the most orders?

   Employee: Peacock\
   Most orders: 40

3. What product was ordered the most by customers in Germany? <br/>

   Product:       Camembert Pierrot\
   Quantity:      40\
   Orders:        300\
   TotalOrdered:  12000
   
VIEW CODE HERE: https://github.com/Creative-Dave/Spotify-Winter-2022-Data-Science-Intern-Challenge/blob/main/DataScience_Intern_Challenge.sql
