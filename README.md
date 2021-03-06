![construction_image](https://image.shutterstock.com/image-vector/abstract-under-construction-background-vector-260nw-79895734.jpg)

# This project is currently in process
## Troubleshooting
1.  Currently the FC data does not have a customer name on every line item.  Working through a fix for this.  
2.  Creating the new dataframe to split the CSV into two columns is duplicating each line eight items for each date. 

---
# Data Analysis
The purpose of this project is to create a Customer Dashboard that includes open Sales Orders and Forecast from Oracle.  There is currently no reporting for Forecast from the Oracle module being utilized.  Forecast data is entered into Oracle Forms with no reporting structure that will return Customer Name and $.

* Step one - ETL data using sales order and forecast reporting for a business unit
* Step two - Create visualizations for presentation in Sales, Inventory and Operations Planning review for business unit

---
## Data Sources
* [LOOKUP.xlsx](https://github.com/Emily-Keymon/data-analysis/files/5838729/LOOKUP.xlsx)
* https://github.com/Emily-Keymon/data-analysis/blob/main/Resources/JAX%20FC.csv
* https://github.com/Emily-Keymon/data-analysis/blob/main/Resources/LEX%20FC.csv
* https://github.com/Emily-Keymon/data-analysis/blob/main/Resources/JAX%20OPEN%20ORDERS.xlsx
* https://github.com/Emily-Keymon/data-analysis/blob/main/Resources/LEX%20OPEN%20ORDERS.xlsx

---
## Tools Used
* Jupyter Notebook
* Python - Pandas
* Microsoft Excel
* Oracle 12.1.3
* MongoDB

---
## Tasks
### Forecast Data
#### Extract 
1.	Import libraries
2.	Load jax fc file
3.	Read csv file into DataFrame, set Item as index

#### Transform 
4.	Remove extra columns 
5.	New data frame with split value columns for Comment column
6.	Make separate Customer column from new data frame 
7.	Make separate Price column from new data frame 
8.	Dropping 0 and 1 columns from new data frame
9.	Merge jax_fc and new data frames
10.	Change Current to Qty
11.	Remove Qty 0
12.	Check data types
13.	Change Price data type from object to float
14.	Recheck data types
15.	Check total count against resource file to ensure data is correct
16.	Add extended price column and populate with Price * Qty
17.	Add column TYPE = FC
18.	Add column Org = JAX or LEX
19.	New data frame with deleted Comment column
20.	Check total count against resource file to ensure data is correct
21.	Sort by Date, then Item 
22. Save file to csv
23. Save file to Excel

#### Repeat Steps 1 - 23 for LEX FC Data

----
### Sales Order Data
#### Extract 
1.  


---
#### Transform
1.  



#### Repeat Steps 1 - 23 for LEX SO Data


---
### Forecast + Sales Orders
#### Merge
1. 

---
#### Visusalizations
1.  


---
#### Load
1.  

---
## Oracle Information

![Oracle_info](https://user-images.githubusercontent.com/64673015/104372260-99d43f80-54e5-11eb-92f3-a0254e50a4b7.PNG)

---
## Initial Forecast Data Sample

![FC1](https://user-images.githubusercontent.com/64673015/104372584-a6589800-54e5-11eb-9937-bd7cb9ef1e7c.PNG)


![FC2](https://user-images.githubusercontent.com/64673015/104372770-b2dcf080-54e5-11eb-8bf1-35aa7415871e.PNG)

---
## Initial Open Orders Report Sample

![OO1](https://user-images.githubusercontent.com/64673015/105095794-c4854180-5a6b-11eb-91d5-b9929448d7fc.PNG)

## Results

---
____



