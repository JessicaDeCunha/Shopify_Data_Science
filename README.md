
## Question 1: 
### Given some sample data, write a program to answer the following: click here to access the required data set

On Shopify, we have exactly 100 sneaker shops, and each of these shops sells only one model of shoe. We want to do some analysis of the average order value (AOV). When we look at orders data over a 30 day window, we naively calculate an AOV of $3145.13. Given that we know these shops are selling sneakers, a relatively affordable item, something seems wrong with our analysis. 

Think about what could be going wrong with our calculation. Think about a better way to evaluate this data. 
What metric would you report for this dataset?
What is its value?

## Answer:

Solely looking at the AOV can be misleading as it will only give you a partial picture of the customers purchase behavior. The AOV can be a helpful metric as it determines the mean of the data, however, it is crucial to also consider the median (the middle value of all orders) and the mode (the most frequently occuring order value) of the data to be able to formulate insights.

1. The problem with this metric in this case is that it takes the average order amount and divides it by the amount of rows in the dataframe. This will cause outliers for transactions that contain mulitple items, thus skewing the initial analysis report. This metric does not consider how many items were purchased in each transaction. To resolve this problem we need to sum all order amounts and divide by the quantity of items in the order. This way, we are calculating the average price per item.

2. Depending on the purpose of the anaysis there are a variety of metrics you could use. We may want to know which stores are the top 10 performing stores. This metric is helpful to determine which stores are performing the best. These top performers may have a very effective marketing strategy that could benefit other shops, these strategies could inlcude SEO optimization, promotions, and affiliate programs.

3. 

## Question 2:
### For this question you’ll need to use SQL. Follow this link to access the data set required for the challenge. Please use queries to answer the following questions. Paste your queries along with your final numerical answers below.

How many orders were shipped by Speedy Express in total?
What is the last name of the employee with the most orders?
What product was ordered the most by customers in Germany?

