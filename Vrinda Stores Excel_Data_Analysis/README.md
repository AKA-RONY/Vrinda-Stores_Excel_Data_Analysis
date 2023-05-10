# DETAILED EXPLAINATION OF THE PROJECT... #


 ##### DATASET =>  Vrinda Store Dataset.xlsx #####
 ##### MAIN FILE => Vrinda Stores Excel_Data_Analysis.xlsx #####


PROBLEM STATEMENT:- 
-------------------------
You are hired as a data analyst for 'VRINDA STORE'. They asked you to analyse the data of 2022 and give an annual report, that will help them to understand the existing 
customers in better way and how they can grow their business next year, i.e 2023.


THINGS I WORKED ON:-
--------------------------
1. Data Cleaning
2. Data processing
3. Data Analysis
4. Data Visualization
5. Reports
6. Insights & next Step
----------------------------

THINGS I DO GENERALLY BEFORE WORKING ON DATASET:-
---------------------------------------------------
-> Highlevel overview of data <br>
-> what are the data points <br>
-> can it solve the business problem or not <br>


QUESTIONS I FORMED AFTER GOING THROUGH THE DATASET:-
--------------------------------------------------
1. Compare  the sales and orders with respect to month using single chart. 
2. Which month got the highest sales and orders in 2022?
3. Who purchased more? men or women in 2022 ?
4. What are the different order status in 2022 ?
5. List top 5 states contributing to sales.
6. Relation between age and gender, based on number of sales.
7. Which channel is contributing to maximum sales?
8. Highest selling category?
-------------------------------------------------------------- 


MAIN PART:-
---
A) DATA CLEANING - In data cleaning we first cross check the data of every column,whether all the data is correct or not. <br>
   i) There should be no duplicate/repeating or  null value <br>
   ii) The values should be consistent. ex- gender column has some inconsistent values(men, m, women, w) & qty column has some inconsistent values, make them in proper format<br>
   iii) Their should be no outliers, go through every column carefully!<br>
   iv) check if any values are mispelled.<br>
   
B) DATA PROCESSING -It means we want to calculate some values or want to process any data that would help us in our analysis process. Includes working with formulas,etc. <br> 

Lets begin solving our qtns:- <br>
--
q6.soln:- <br>
 Relation between age and gender, based on number of sales.<BR>
 But if we want to see the relationship individually its not possible. So, to do that we have to create a column as Age_Group and then group the age values into teenage(<30 yrs ),adult(>=30-49 yrs), senior( >=50). <br>
apply this condition to every row:-  IF(E2>=50,"senior",IF(E2>=30,"Adult","teenager")) <br><br>

q2.soln:- <br>
which month got the highest sales & orders?<br>
=> create a separate column (month) and  write the formula =TEXT(G2,'mmm')/=TEXT(G2,'mmmm')# this will show the name of the month as JAN/JANUARY.<BR>

C) DATA ANALYSIS AND VISUALIZATION - here we will be analysing the data using pivot table and visualize it using various graphs. <br>
   q1.soln:- <br>
   Compare  the sales(amount) and orders(count of orders) with respect to month using single chart. <br>
   => Make a pivot table of amount and order count and put month in rows; you will get the month-wise distribution of sales and order-count. Then draw a combo chart. Now, we have    to format the sales amount values since its not convinient to read.<br>
   Right click the column(amount)->Format axis-> in number tab-> type-> 0.00,,"M"  , means after 1st number there will be 2 point decimal and a letter "M" for million.<br>
 <br>
 
  INSIGHTS:-<br>
     -> 1. we can see month wise sales which month got the highest sales. <br>
     -> 2. we can also see order count in each month.<br>
     -> 3. highest sales and highest order are on 'March'. <br>
   <br>
    q3.soln:- <br>
    Who purchased more? men or women in 2022 ? <br>
    => same draw a pivot table for gender(in rows) and sales(as values) columns. you can see that female does more shopping. visualize it with pie graph. do the rest formatting. <br>
 <br>
 
  INSIGHTS:- <br>
     -> 1. We can see that Female do the most shopping. <br>
 <br>
    q4.soln:-<br>
    What are the different order status in 2022 ? 
    => same create pivot table for status (in rows) & order_count(values). Then draw a pie graph, you can see the distribution  of status throughout the channels.<br>
    <br>
  INSIGHTS:- <br>
     -> 1. we came to know that majority of the orders had been delivered(90%), 2% of entire order were refunded, 3% were returned & 3% were cancelled.<br>
     -> 2. Among the channels Amazon had the highest number of deliveries, & Mesho had the least number of deliveries.<br>
 <br>
    q5.soln:-<br>
    List top 5 states contributing to sales.<br>
    => same draw a pivot table for states(rows) and amount(sales) as values. Then sort the amount to largest to smallest. Then filter the states for top 5. Draw a bar chart. Format the chart, refactor the data into millions i.e 0.00,,"M" for sales amount & 0.0,,"M" for X-axis.<br>
 <br>
 INSIGHTS:- <BR>
     -> we can see that Maharastra is the state where maximum numbers of orders are comming from various channels. And you had sales of amount 2.99M last year<br>
     -> Followed by Karnataka,Uttar Pradesh, Telengana, Tamil Nadu are top 4 states after Maharastra.<br>
 <br>
    q6.soln:-<br>
    Relation between age and gender, based on number of sales.<BR>
    => since we had previously grouped the age. Now make a pivot table for age_group(as rows),gender(as columns) & order_id(as values). then show the values as %of grand total.Then build a bar graph. <br>
 <BR>
 INSIGHTS:- <BR>  
     -> We can see that women of adult group does the shopping more i.e(between 30-49 yrs)<br>
  <br>
    q7.soln:-<br>
    Which channel is contributing to maximum sales?
    => same make a pivot table format the data into percentge then make a pie chart. As we want to show the distribution of each channel within 100%.<br>
  <br>
 INSIGHTS:- <BR>
     -> We can see Amazon has the highest number of orders & sales.<br>
  <br>
    q8.soln:-<br>
    Highest selling category.<br>
    => same draw a pivot  table for caregory and order_count, then draw a bar graph and format it.<br>
  <br>
 INSIGHTS:- <BR>
     -> Sets & Kurtas are highest selling Categories.<br>
 <br>
  ### INSIGHTS AND NEXT STEPS: ###
After analysing the entire data we came to below mentioned conclusions:-
1. Women are the prime customers, and are more likely to purchase as compared to men(~65%).
2. Maharastra,Karnataka and Uttar Pradesh are top 3 states.
3. Adult Age_group(30-49 yrs) is max contributing (~50%).
4. Maximum orders are coming from Amazon,Flipkart,Myntra channels(~80%).Among them Amazon is the Highest.


FINAL CONCLUSIONS TO IMPROVE 'VRINDA STORE' SALES:
-> Target Women Customers of Age_group(30-49 yrs) living in Maharastra,Karnataka,Uttar pradesh by showing ads/offers/coupons available on Amazon,Flipkart, and Myntra.


  
  
    
    
 

    
 
    






