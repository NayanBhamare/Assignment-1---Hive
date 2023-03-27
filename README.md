# Assignment-1---Hive

a. Calculatye total sales per year

-> select year_id,sum(sales) as total sales from sales_order_orc group by year_id;

b. Find a product for which maximum orders were placed

-> select productline,sum(quantityorder) as max_order from sales_order_orc group by productline;

c. Calculate the total sales for each quarter

-> select qtr_id,sum(sales) as qtotal_sales form sales_order_orc group by qtr_id;

d. In which quarter sales was minimum

-> select qtr_id,sum(sales) as qtotal_sales form sales_order_orc group by qtr_id order by qtr_id;

e. In which country sales was maximum and in which country sales was minimum

-> select country,sum(sales) as t_sales from sales_order_orc group by country order by t_sales desc;

f. Calculate quartelry sales for each city

-> select qtr_id,city,sum(sales) as q_total from sales_order_orc group by qt_id,city order by otr_id,city;

h. Find a month for each year in which maximum number of quantities were sold

-> select mounth_id,year_id,sum(quantityorder) as q_order from sales_order_orc group by mounth_id;
