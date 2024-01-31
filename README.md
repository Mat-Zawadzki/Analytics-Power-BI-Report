# Analytics Report in Microsoft Power BI

<img src="https://github.com/Mat-Zawadzki/Analytics-Power-BI-Report/blob/main/Images/ExecutiveSummary.png?raw=true" alt="alt text" width="max">

## Contents

1. [Project Overview](#project-overview)
2. [File structure ](#File-structure)
3. [Loading in Data](#Loading-in-data)
4. [Creating Data Model](#Creating-data-model)
5. [Downloading](#Downloading)
6. [Pages and Visuals Created](#Pages-and-visuals-created)
7. [License](#License)

## Project Overview
This project focuses on analyzing and visualizing data from various sources to gain valuable insights into business operations. In this readme file, we'll guide you through the initial steps of the project, specifically the downloading, importing, and transformation of data within the following tables: Orders, Products, Sales, and Customers.


## File structure 
![Alt text](https://github.com/Mat-Zawadzki/Analytics-Power-BI-Report/blob/main/Images/tree.png)

> - Clips contains the videos used in the Readme
> - Images contains images used 
> - Tables contains all the csv table files


## Loading in Data
The project relies on four key tables: Orders, Products, Sales, and Customers. Each table provides essential information that contributes to a comprehensive understanding of the business data.

> - **Orders:** Contains details about each order, including the order and shipping dates, the customer, store and product IDs for associating with dimension tables, and the amount of each product ordered.

- **Products:** Encompasses information about each product sold by the company, including the product code, name, category, cost price, sale price, and weight.

- **Stores:** Contains information on each store, including the store code, store type, country, region, and address.

> - **Customers:** Stores customer-related information, including customer ID, name, and geographical location.

## Creating Data Model
Using the loaded in data I created a star schema with active, many-to-one relationships on the orders table. I created my own Date table using dax expressions.

## Downloading
To download and view the report on your local machine, run the command in the correct directory you wish to download it into:

`git clone https://github.com/Mat-Zawadzki/Analytics-Power-BI-Report`

Can also change the name of the folder:

`mv Analytics-Power-BI-Report <YOUR_NAME_CHANGE_HERE>`

## Pages + Visuals Created

---

### Executive Summary

> - Total Orders by Category - Clustered Bar 
> - Total Revenue by Date - Line 
> - Total Rev by Country and store - Donut
> - Total KPIs
> - On metric KPIs 

<br>
<br>

---

### Customer Detail


https://github.com/Mat-Zawadzki/Analytics-Power-BI-Report/assets/114954374/10f89868-4bb5-42ee-8589-94f7c161ec9b


---

### Product Detail


https://github.com/Mat-Zawadzki/Analytics-Power-BI-Report/assets/114954374/3640bbbb-9357-46d8-85be-03b903501be0


---

### Stores Map + Stores Drill Through



https://github.com/Mat-Zawadzki/Analytics-Power-BI-Report/assets/114954374/eda7621b-641d-4930-8cca-a60a1603fefa



---


## License