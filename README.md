# BI-project

#### Amazon Sales Report 
![image](https://github.com/AmanBaker06/BI-project/assets/168013894/24794f01-23bb-4db9-bc9f-6b0f04ed4c8f)










### Problem Statement 
This Report uses the data of the e-commerce platform Amazon to analyze its sales data and performance across categories. The data encompasses the sales records from March-June of 2022.The analysis is intended to help understand the most popular and profitable products during the given period. This study will help to determine which products to focus on and promote on the e-commerce platform.
# ETL Stage
- The dataset contains two excel files "Amazon" and "Amzon-fashion-YT"
- Amazon Table: Steps
  Promoted first row as Headers
  Changed Data Type of columns accordingly
  Filtered the null and blank rows from the ship-state column that were not required
- Amanzon-fashion-YT: 
  Replaced values for numerous columns from null to blank or from blank to other or NA for 
  better categorization of data points
  Added a custom column by adding values from three category columns in order to make a single category column and removed the previous three.

  ![image](https://github.com/AmanBaker06/BI-project/assets/168013894/42a13f2b-eae4-42b6-93d4-b9d9abbbfeee)

  
- Created a new column for Gender-based category by splitting the new category column. Column   name "Section"
- Replaced blanks with the value "other" in color column
- Merged both tables into Amazon table to input the size column for sales by product size 
  analyses
- The "large" column contained numerous image links for categories. Used split column to only 
  keep the required link in each row and removed other columns

# Modelling 
- The following measures were made for specific calculations:
  Calculated Column for Total Amount - Total Amount = 'amazon-fashion - YT'[Qty]*'amazon-       fashion - YT'[sales_price]
  Total Revenue generated - SumAmount = sum('amazon-fashion - YT'[Total Amount])
  Total Quantity sold- SumUnit = sum('amazon-fashion - YT'[Qty])
  
- Status Column values in Amazon Table grouped for Analysis through Shipping/Delivery status
  ![image](https://github.com/AmanBaker06/BI-project/assets/168013894/1ae75adc-1293-4367-bf19-517f068b2637)

# Report
Overview Page
Overview of Units sold by each category across different states and cities
Region slicer provided for navigation along with category images for better understanding and engagement. 
The total amount and units sold are represented through the respective card visuals for a quick overview and the table provides access to the real data for reference if needed

Revenue Distribution Page 
Provides an in-depth analysis while providing user engagement for a better understanding of revenue distribution among different regions, products, and categories. 
The Decomposition tree will help in understanding the division of Revenue among states, categories, and product sizes, helping to understand the biggest contributors and slow performers. 
The table provides the top 10 categories by revenue
The pie chart represents revenue by shipping status (Important as different products are at different stages of the delivery process. The chart will help assess the following :
1) Potential Revenue through Shipping in process and pending delivery status 
2) Actual revenue collected to date through Shipped and received status
3) Lost revenue by unsuccessful status

   
![image](https://github.com/AmanBaker06/BI-project/assets/168013894/83917d9d-cffa-437e-942f-fafd25f78b18)



  
  
  
