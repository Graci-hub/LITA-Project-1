# Introduction
### This report analyzes sales data using tools like Excel, SQL, and Power BI to uncover key trends and insights. The data contains fields such as Order ID, Customer ID, Products, Region, Order Date, Quantity, Unit Price, Total Sales, Order Year, and Year. The objective is to perform data cleaning, calculations, and visualizations to derive actionable conclusions about sales performance.
### Tools used:
- Excel: Data cleaning, initial exploration, and calculation of key metrics.
- Structured Query Language (SQL): Querying the dataset for deeper analysis and performing aggregations.
- Power BI: Visualizing the data and summarizing key findings through interactive reports and dashboards.
### Data Cleaning, Preparation, and Metrics (EXCEL)
- Removing Duplicates: The raw dataset has multiple entries which could have twisted the total sales. I used the excel feature 'Remove duplicates' to eliminate the repetitive rows and to extract the unique datas (i.e Order id's, Customer id's and products).;
- Pivot tables: In Excel, i used pivot tables to group sales by region, year, month and product category, allowing me to quickly spot which areas were underperforming.
- Formulas and Functions: During the analysis, Excel’s powerful functions were used extensively to calculate key sales metrics and derive actionable insights from the data. By leveraging these formulas, I was able to perform complex calculations quickly and efficiently.
  1. COUNT(): After removing duplicates to extract the unique datas, i used the COUNT function to count the number of cells with numeric values within a specified range. E.g Unique Order Id  (=COUNT(M2:M21))
  2. COUNTA(): After extracting the unique datas such as Unique customer Ids and products, i used the COUNTA function to count cells with variable characters (numbers and texts). E.g Unique customer Id (=COUNTA(S2:S7))
  3. COUNTIF(): To determine the number of times a particular product was sold, I utilized the COUNTIF() function. This helped identify high-selling products. (=COUNTIF(Table3[Product],"shirt")).
  4. AVERAGEIF(): To determine the average price per product, i used the AVERAGEIF() function. It helped to determine the average price of each particular product E.g (=AVERAGEIF(Table3[Product],"gloves",Table3[Total sales])).
  5. SUMIF(): To determine the total sales of a specific product, i used the SUMIF function. E.g (SUMIF(Table3[Product],"shirt",Table3[Total sales])).
  6. TEXT(): Using a TEXT() function in Excel, i was able to isolate the order month and year from the date data. E.g. (=TEXT(E2,"MMM")), (=TEXT(E3,"YYYY"))
  7. Adding calculated column: I added the calculated column below:
  - Total sales = Quantity * Unit price
### Data Organization and Filtering
The dataset was filtered by Region, Year, and Product to explore trends in different segments, making the data easier to analyze.


    
