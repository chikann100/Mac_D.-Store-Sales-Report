# Mac_D Store Sales Analysis

### Project Overview 
---

this data analysis project aims to provide insists into the sales performance of Mac_D store over the past year. by analysis various aspects of the sales data, i was able to identify trends and data-driven recommendation and gain an understanding of the company's performance.




<img width="532" alt="mad_d" src="https://github.com/chikann100/Mac_D.-Store-Sales-Report/assets/149578332/7a52d7e2-8295-450a-8002-b11d0e5c8590">

### Data sources

data: the dataset used for this analysis is the "mac_D Transaction_1998.csv", "mac_D Transaction_1997.csv", "mac_D products.csv". constaining detailed information for each sales made by the company.

### Tools

- Excel - Data cleaning
   - [downloade here](https://microsoft.com)
- SQL server - Data analysis
    - [downloade here](https://sqlserver.com)
- PowerBi - Creating a reports
   - [downloade here](https://microsoft.com)


### Data cleaning/preparation

in the beginning of the data preparation phase the following tasks was performed
1. Data loading and inspection
2. Handling missing values
3. Data cleaning and formatting.


### Exploratory Data Analysis
EDA involved exploring the sales data to answer key questions such as:
- what is the overall sales trend?
-  which products are the top sellers?
-   what are the peak sales periods?


### Data Analysis

``` sql
select
  product name, product id
from product
order by product name
limit 5;
```

``` sql
select product id, sum(quantity)
from
(select product id, quantity
union all
select product id, quantity
from transaction_1997
group by product id;
```


### Result/findings
The analysis results are summarised as follows:

- Revenue Trended up resulting in a 10,119.30% increase between 1996 and 1998
- the most sold products in terms of sales and renveune are:
    1. carles head cheese
    2. Washington apple drink
    3. bravo noodle soup
    4. moms_ foot_ long hot dogs
    5. Urban small eggs
-Awareness should be centered more in countries like Mexico and Canada
- profit jumped from 100,378.84 to 112.282,77 during its steepest incline between july 1996 and december 1996.

## Recommendations

Based on the analysis, we recommend the following actions:
- foucse on getting more outlet in countries like mexico and canada
- focuse on expanding  and promoting the most sold products in terms of sales and revenue
- invest in marketing and promotion during peak sales seasons to maximize revenue.

## Limitation:

i have to remove all zero values from my dataset because they would affect the accuracy of my conclusion

### Reference
[SQL essentials for business analysts and data professionals](https://www.udemy.com)

😄
💻


 
    

  

  

