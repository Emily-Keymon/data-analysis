# This project is currently in process
## Troubleshooting
1.  Currently the FC data does not have a customer name on every line item.  Working through a fix for this.  
2.  Creating the new dataframe to split the CSV into two columns is duplicating each line eight items for each date. 

---
# Data Analysis
The purpose of this project is to create a Customer Dashboard that includes open Sales Orders and Forecast from Oracle.  There is currently no reporting for Forecast from the Oracle module being utilized.  Forecast data is entered into Oracle Forms with no reporting structure that will return Customer Name and $.

---
## Data Sources


---
## Tools Used
* Jupyter Notebook
* Python - Pandas
* Microsoft Excel
* Oracle 12.1.3

---
## Tasks
* Step one - ETL data using sales order and forecast reporting for a business unit
### JAX-LEX FC DATA
### Extract Data
1	Import libraries
2	Load jax fc file
3	Read csv file into DataFrame, set Item as index

###	Transform Data
4	Remove extra columns 
5	New data frame with split value columns for Comment column
6	Make separate Customer column from new data frame 
7	Make separate Price column from new data frame 
8	Dropping 0 and 1 columns from new data frame
9	Merge jax_fc and new data frames
10	Change Current to Qty
11	Remove Qty 0
12	Check data types
13	Change Price data type from object to float
14	Recheck data types
15	Check total count against resource file to ensure data is correct
15	Add extended price column and populate with Price * Qty
16	Add column TYPE = FC
17	Add column Org = JAX or LEX
18	New data frame with deleted Comment column
19	Check total count against resource file to ensure data is correct
20	Sort by Date, then Item 

* Step two - Create visualizations for presentation in Sales, Inventory and Operations Planning review for business unit

---
## Oracle Information

![Oracle_info](https://user-images.githubusercontent.com/64673015/104372260-99d43f80-54e5-11eb-92f3-a0254e50a4b7.PNG)

---
## Initial Forecast Data

![FC1](https://user-images.githubusercontent.com/64673015/104372584-a6589800-54e5-11eb-9937-bd7cb9ef1e7c.PNG)


![FC2](https://user-images.githubusercontent.com/64673015/104372770-b2dcf080-54e5-11eb-8bf1-35aa7415871e.PNG)

---
## Results



