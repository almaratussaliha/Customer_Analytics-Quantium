# Quantium Virtual Internship Experience Program in Data Analytics

## Background
We need to present a strategic recommendation to Julia that is supported by data which she can use for the upcoming category review. 
The client is particulary insterested in customer segments and their chip purchasing behaviours.

#### `Main Goals of this task are:`
- Examine data: check missing data, anomalies, outliers and clean them.
- Data analysis and customer segments: create charts or graphs, insight and recommendations.
- Metrics analysis: monthly sales and monthly customers.

### About the datasets
- The transaction dataset has 8 characteristics with 264,863 rows, while the purchase behaviour dataset has 3 characteristics with 72,637 rows. these datasets were merged. 
- There are no missing values.
- The date characteristic was in integer format, so it was changed to datetime format.
- The prod_qty and tot_sales features have extremely high values.
- Some product_names are written in more than one way. Examples: Dorito and Doritos, Smith and Smith, Red and RDD.

## Data Cleaning
- Date feature changed to date/time format.
- Extremely high values changed to median data.
- Split the first word of the product_name feature to get the brand name. 
- Some brands were misspelled. They have been cleaned up.
- Split numbers from product_name feature to get package size.

## Exploratory Data Analysis

### `How are sales performing?`
- This dataset is a year's sales. There are 365 days in a year. But there are only 364 transactions. 
It was a Christmas day where there was no transaction because the shop was closed.
- Sales increase in December exactly one week before Christmas Day.
![alt text](https://github.com/almaratussaliha/Customer_Analytics-Quantium/blob/master/img/salesdist.png?raw=true)

### `Which brands are bought the most and contribute to sales?`
- There are 21 brands. 
- The most popular is <b>Kettle</b>, followed by Smiths, Doritos and Pringles. 
These brands also contribute to high sales.
- Kettle brand achieved sales of $390,239.
![alt text](https://github.com/almaratussaliha/Customer_Analytics-Quantium/blob/master/img/totsales.png?raw=true)

### ` Which pack sizes are most bought and contribute to sales?`
- There are 21 pack sizes, with the 175g pack being the most popular, followed by the 150g pack. 
This pack size also contributes to high sales.
- 175g pack size has 66,390 products sold with sales of $48,5437.
![alt text](https://github.com/almaratussaliha/Customer_Analytics-Quantium/blob/master/img/package.png?raw=true)

### `Which lifestage customers contribute to high sales?`
- There are 7 life stages. Most customers are older singles/couples, followed by retirees and older families.
- The Older Singles/Couples has the highest number with $402,427 in sales.
- New families have the lowest number of transactions among the segments.
![alt text](https://github.com/almaratussaliha/Customer_Analytics-Quantium/blob/master/img/custsales.png?raw=true)

### `Who spends the most on transactions based on life stages and customer segments?`
- By segment, Mainstream - Young Singles/Couples has the highest number of customers, followed by Mainstream - Retirees. 
New Families have the lowest number of customers across all segments.
![alt text](https://github.com/almaratussaliha/Customer_Analytics-Quantium/blob/master/img/custbyseg.png?raw=true)

- Looking at sales by segment, Budget - Older Families, Mainstream - Retirees and Mainstream - 
Young Singles/Couples are the largest contributors to sales.
![alt text](https://github.com/almaratussaliha/Customer_Analytics-Quantium/blob/master/img/custtrx.png?raw=true)
- Although, Mainstream - Young singles/couples have the highest number of customers but don't contribute to high sales. 

### `How many chips are purchased per customer by segment?`
- In all segments, older families purchase more chips per customer. That's why they make the biggest contribution to sales.
![alt text](https://github.com/almaratussaliha/Customer_Analytics-Quantium/blob/master/img/chippercust.png?raw=true)
- In fact, new families buy more chips than young singles/couples. They also contribute the least to sales.
- Older Families and Young Families purchase more chips per customer than any other segment because
they are likely to have children or relatives.

### `How many sales are achieved each month?`
- The average monthly sales is $161,094.
- The highest sales are in December which is $167,913 and the lowest sales are in February which is $150,665.
![alt text](https://github.com/almaratussaliha/Customer_Analytics-Quantium/blob/master/img/monthlysales.png?raw=true)

### `How many customers monthly? `
- The average customer each month is 18,440.
- The highest customer is in December which is 19.076 and the lowest customer is in February which is 17.249.
![alt text](https://github.com/almaratussaliha/Customer_Analytics-Quantium/blob/master/img/monthlycust.png?raw=true)


## Recommendations:
- Stocks need to be high in December before Christmas Day.
- Kettle, Smiths, Doritos and Pringles need to be stocked as they sell out the most.
- Budget - Older Families, Mainstream - Retirees, and Mainstream - Young Singles/Couples need to be noticed as they generate high sales.
- Based on customers by segment, offer different promotions. For example, older families who spend $50 save $5.
- Multi-buy promotions for new families (i.e. buy 2 get 1 chip - 70 gr) 
