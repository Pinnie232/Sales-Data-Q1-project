# SALES DATA ANALYTIC PROJECT

## OVERVIEW 

## REQUIREMENTS
Clean the data
• Analyze the data using appropriate Excel formulas/functions
• Create a Dashboard using Excel as well.
• Which Month has the highest revenue?
• Which product is the best selling in terms of qty and revenue?
• What is the AOV(average order value)?
• Which state did we get the most number of orders from?
• Which state is generating the highest number of revenue?

### Steps to clean data:
- 1. Change the date format to short date.
- 2. I delete April which was 01/04/2019 out of the data because we are working with jut quarter 1 and it didn’t make the data look nice.

- 3. There was a lot of  missing data and there is also duplicate data. I deleted the duplicate data and then the missing data. 

- 4. In the purchase address I deleted the last letter because they weren’t necessary, and it didn’t look right it was wrong (867 Willow St_XYZJDS) to (867 Willow St) using the Left and Len function.

- 5. I then added the information in the location and product workbook into the sales workbook using the VLOOKUP function.
     
 =VLOOKUP(G2,Location!$A$2:$B$11,2,FALSE) State
 =VLOOKUP(B2,Products!$A$2:$B$20,2,FALSE) Products 
 =VLOOKUP(I2,Products!$B$2:$C$20,2,FALSE) Price Each
6.	Edited the price each column (added the dollar sign)
7.	Created table and named it Sales data

### PIVOT TABLE
- 1.	Created pivot table
- 2.	To calculate the average order value, I used the DAX measures. 
Steps:
a.	Right click on the sales data
Average Order Value ='Sum of Revenue' / 'Count of Order ID'
