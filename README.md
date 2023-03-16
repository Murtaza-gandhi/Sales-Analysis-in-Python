# Sales-Analysis-in-Python

# Requairments are as follow ,  
1. Monthwise number of quantities sold
2. Category wise Qty sold
3. Sub-channel wise total sales
4. Highest sale in which month
5. Highest selling product

# The Analysis Steps
Importing nessesary library, 
Importing the data by using pandas, 
Checking if there is any null values by .info(),
Creating a Datafream by pandas 

# for  Requariment 1

Created a new colom using dt,strftime for extracting date from the given date column,

Then creating new Datafream using groupby with Month-year column and sum mathod to sum the values of the Quantitys

# for Requirement 2

Using pd.Groupby  by Catagory with the value of Quantity and storing the dataframe in a variable 

# for Requirement 3 

Creat a new Datafream of grouped data using groupby on Sub-channels with sum() of sales and storing it in a different Variable 

# for Requirement 4 

By appling sort_values in desanding order on an new datafream made by grouping month-year with sum() of sales  

# For Requirement 5

Creating new Copy of original Datafream 
as we have to make a colom of product name that don't have any numarical value, 

we creat a new colomn of productname in which, 

first we replace the numerical values with "---" triple hifon then split the name with "---" and get the desired value,   

then creat a new datafream grouping product name with the sum() of sales and sorting it in desending order by using Sort_values 

# For Requirement 6

Sorting the product name in decending order and storing it in a variable 

# For Requirement 7 

Last save all the variables into a excel file using pd.Excelwriter giving the path of where to save the file and using .to_excel for creating new sheets
