# Sales-Insights-Power-BI
# Problem statement
AtliQ hardware is a company which delivers computer hardware & peripheral Manufacturers to his clients, which has several branches throughout India. The sales director of the company is facing a lot of issues in terms of understanding how the business is performing and what are all the problem company is facing currently as the sales are not as expected and declining gradually. And whenever he calls the regional managers to get the current status of the sales and market, as a human behaviour, these people sugar cote the truth and send tons of Excel files instead of disclosing the truth, which made the sales director more frustrated. Humans are not comfortable in consuming numbers from excel files, which is obvious reason for the frustration.

# Solution
Sales director of the AltiQ hardware, decided to build a PowerBI Dashboard for converting the data into visual representation to make data driven decisions. So, he hired a team of data people to complete this task.

# AIMS Grid
By using the AIMS grid project management tool, we made sure what are the purpose, stakeholder, end result and success criteria of our project.
![Screenshot (202)](https://github.com/user-attachments/assets/005d5ed2-3619-41d0-a196-28196c03f697)
# Data Analysis Using SQL
Data Analysis Using SQL
Show all customer records

SELECT * FROM customers;

Show total number of customers

SELECT count(*) FROM customers;

Show transactions for Chennai market (market code for chennai is Mark001

SELECT * FROM transactions where market_code='Mark001';

Show distrinct product codes that were sold in chennai

SELECT distinct product_code FROM transactions where market_code='Mark001';

Show transactions where currency is US dollars

SELECT * from transactions where currency="USD"

Show transactions in 2020 join by date table

SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;

Show total revenue in year 2020,

SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transactions.currency="USD\r";
Show total revenue in year 2020 in Chennai

SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.market_code="Mark001";
# Key Learnings
Learned about what real business data sets look like.
Learned about how to write some major analysis queries in MySQL.
how to connect the database’s tables to Power Bi and how to clean & modify the unwanted data in Power Query.
Learned about some major practical DAX functions and measures.
Learned about some major analytical visuals and reports.
# Final result
# Key Insights
![Screenshot (204)](https://github.com/user-attachments/assets/075a98b5-0e33-4c7a-b390-2450f8669ec7)

# Profit Analysis
![Screenshot (200)](https://github.com/user-attachments/assets/317cb92b-5dfd-4306-a7ff-fdf1b80cd131)

# Perfomance insights
![Screenshot (201)](https://github.com/user-attachments/assets/30348a61-b3c4-4b80-af7e-8397e15cf207)

