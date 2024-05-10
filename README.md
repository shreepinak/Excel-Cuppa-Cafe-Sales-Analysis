# Excel-Cuppa-Cafe-Sales-Analysis

# Dataset: Taken from Maven Analytics. [source]( Free Data Sets & Dataset Samples | Maven Analytics)
# Aim: To analyze retail sales of Cuppa Café shop.
# Systematic Procedure: 
1)	Data Cleaning by power query editor:
•	Adding conditional column separating size of product from product detail. 
•	Transforming the various columns e.g. Total Bill column.
•	Removing unnecessary date. e.g. Converting date & time format to time format.


2)	Formulae used:
•	Total Bill = Transaction quantity*unit_Price 
•	Total Sales = Sum ([Total Bill]) (Dax formula in power pivot)
•	Footfall = DISTINCTCOUNT (Transaction [Transaction_id]) (Dax formula in power pivot)
•	Average Bill/Person = 
•	Sum (Transactions [Total_bill])/DISTINCTCOUNT (Transaction [Transaction_id]) (Dax formula in power pivot)
•	Average Order/Person = Sum (Transactions[transaction_qty])/DISTINCTCOUNT (Transaction [Transaction_id]) (Dax formula in power pivot)

3)	Feature Engineering:
•	Add a new column named `Hours’ to give insight of sales in the Morning, Afternoon and Evening. This will help answer the question on which part of the day most sales are made.
•	Add a new column named `Day_name` that contains the extracted days of the week on which the given transaction took place (Sunday to Saturday). This will help answer the question on which week of the day, shop is busiest.
•	Add a new column named `Month_name` that contains the extracted months of the year on which the given transaction took place (Jan to June). Help determine which month of the year has the most sales & orders.


# Analysis: Based on listed below questions
1) What is the total sales revenue and Footfall?
**Ans) The total sales revenue is $698812.33 & Footfall is 149116.**

3) What is the average price/order per person?
**Ans) Average price per person is $4.69 & Average order per person is 1.44.**

4) What is quantity ordered based on hours?
**Ans) The maximum orders are taken during morning hours between 8 to 10 am.**


5) What is percent of categories distribution based on sales?
**Ans)    From the pie chart, we can observe that coffee, tea, bakery, and drinking chocolate generate most revenue but coffee beans, loose tea, flavors, branded, and packaged chocolate have low revenues. 
        Business should offer discounts, advertise more for these low revenue categories as well as make some improvements in them for the growth of these categories.**

6) What is percent of size distribution based on orders?
**Ans) The regular has large number of purchases followed by Large, and undefined sizes.
     Since the small size order has very less in number of sales, the business should consider discontinuing them.**

7) What is the footfall and sales over various store locations?
**Ans) The Hell’s kitchen generated largest sales and footfalls followed by Astoria & Lower Manhattan.
Various strategies should be implemented to capitalize the high sales in Astoria & Lower Manhattan.**

9) What are top 5 products based on sales?
**Barista Espresso
  Brewed Chai tea
  Hot Chocolate
  Gourmet brewed coffee
  Brewed black tea**

10) What are total number of orders day wise?
**Ans) Most sales are made on Friday. Sales increase on Mondays, Thursdays, and Fridays. Strategies should be developed to boost sales on other days. For e.g. Weekends have lowest sales, so business should research why footfall is less? **
