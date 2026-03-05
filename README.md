# Ecommerce Sales Analysis 

## 📖 Table of Contents
- [Project Overview](#-project-overview)
- [Data Source](#-data-source)
- [Tools & Technologies](#-tools--technologies)
- [Data Cleaning & Preparation](#-data-cleaning--preparation)
- [Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
- [Key Insights](#-key-insights) and Recommendations
- Conclusion

## 📊 Project Overview

Analyzing different sales trend based on the given dataset using Dashboard.

The given Dataset contains four tables such as Customer table, Product table, Store table and Sales fact table each containing 2000 records.


## 🗂️ Data Source
**Source:** web scraping

**Size:** 1,055 KB

**Key variables:** Sales_ID, Order_Date, Customer_ID, Product_ID, Store_ID, Quantity, Unit_Price, Discount, Payment_Type, Total_Amount.


## 🛠️ Tools & Technologies


- **Visualization:** MS Excel 
- **Documentation:** MS Word


## 🧹 Data Cleaning & Preparation

**Customer Table:**

1.Converted entire data into table format

2.Changed all data types, removed duplicates in customer ID column

3.Corrected inconsistencies and made Name column into proper case using clean, trim and proper functions

4.Replaced C- into CUST in customer Id column using find and replace method.

5.Found blank values in Loyalty level column and replaced with “unknown” using formula

                 =if(isblank(H1),”unknown”,H1)  Since it is non -numerical value.
  
6.Copied formula to every row and pasted as values.

**Product Table:**

1.Converted entire data into table format

2.Changed all datatypes, removed duplicates in product ID column

3.Replaced P- into PROD in product Id column using find and replace method

4.Found blank values in “cost” and “stock” column and replaced with average value

               =if(isblank(F2),Average(F1:F101),F2) 
               
               =if(isblank(G2),Average(G1:G101),G2) 
               
5.Copied formula to every row and pasted as values

6.Since it is numerical value


**Store Table:**

1.Converted entire data into table format

2.Removed duplicates in store ID column

3.Changed all data types


**Sales-fact Table:**

1.Converted entire data into table format

2.Changed all data types

3.Changed order date from YYYY-MM-DD format to DD-MM-YYYY format

4.Sorted date column from latest to oldest

5.Found missing values in quantity and price column and replaced with average value

                    =if(isblank(F2),Average(F2:F2001),F2) 
                    
                    =if(isblank(G2),Average(G2:G2001),G2) 
                    
6.Copied formulas for entire row and pasted as values. Since it is numerical value

7.Corrected total amount column for replaced blank values in quantity and unit price using formula


      =([@[unit_Price]]-([@Discount]*[@[unit_price]]))*[@Quantity]

      


## 🔍 Exploratory Data Analysis (EDA) 

•	Comparing total quantity sold and total amount based on product category the Sports category has highest sales and Beauty category has lowest sales

•	Comparing average sales of product category based on stores the Flagship stores ranked higher than Online and Outlet stores.

•	The overall sales performance seems to be quite linear. So, no changes required in the current strategy.

•	2024 has highest sales compared to 2023 and 2025.

•	Comparing the sales of different regions the west region seems to be significantly low. So, it would be effective when focused on some ideologies like discounts and promotions.

<img width="1633" height="801" alt="image" src="https://github.com/user-attachments/assets/f96f9bed-679b-4009-8097-65a89aa05219" /> 







## 💡 Key Insights and Recommendations:


• Based on the analysis of given dataset the sales are very good in the North region and comparatively low in the West region.

• Similarly, Flagship store ranks good in sales compared to outlet store.

• The sales trend looks linear so changes may not be required in the current strategies.

• The sports category products also show good sales volume compared to other categories. 

• The Beauty category product shows low sales.


## Conclusion:

• The integration of Excel proved effective for end-to-end data analysis, from raw data to visual reporting.
