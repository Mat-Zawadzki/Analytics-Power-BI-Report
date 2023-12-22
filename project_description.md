# Step-by-Step

## Loading and Transforming Tables:
#### Orders Table
The Orders table is your main fact table. It contains information about each order, including the order and shipping dates, the customer, store and product IDs for associating with dimension tables, and the amount of each product ordered. Each order in this table consists of an order of a single product type, so there is only one product code per order.

Connected to the Azure SQL Database
Deleted the column named [Card Number] to ensure data privacy 
Used the Split Column feature to separate the [Order Date] and [Shipping Date] columns into two distinct columns each: one for the date and another for the time
Filtered out and remove any rows where the [Order Date] column has missing or null values to maintain data integrity
Renamed the columns in your dataset to align with Power BI naming conventions, ensuring consistency and clarity in your report

#### Products Dimension table
The Products table contains information about each product sold by the company, including the product code, name, category, cost price, sale price, and weight.

Remove Duplicates function on the product_code column to ensure each product code is unique

Follow the steps below to clean and transform the data in the weight column

In Power Query Editor, use the Column From Examples feature to generate two new columns from the weight column - one for the weight values and another for the units (e.g. kg, g, ml). You might need to sort the weight column by descending to get enough different examples to work with.
For the newly created units column, replace any blank entries with kg
For the values column, convert the data type to a decimal number
If any errors arise during the conversion, replace those error values with the number 1
From the Data view, create a new calculated column, such that if the unit in the units column is not kg, divide the corresponding value in the values column by 1000 to convert it to kilograms
Return to the Power Query Editor and delete any columns that are no longer needed

Rename the columns in your dataset to match Power BI naming conventions, ensuring a consistent and clear presentation in your report