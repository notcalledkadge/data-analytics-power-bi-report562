# Data Analytics Power BI Report.
## Contents
- Milestone 2
- Milestone 3
- Milestone 4
- Milestone 5
- Milestone 6
- Milestone 7
- Milestone 8
- Milestone 9

## Milestone 2

The main focus of Milestone 2 was to import the necessary elements required to produce this report into Power BI. The elements that I imported were: **Orders**, **Products**, **Stores** and **Customers**.

Each import involved a different process to follow through Power BI which involved some problem solving. I have attempted to maintain a consistent and clear presentation of the data, with naming conventions matching between the elements and their relevant columns. 

### Task 2: *Load and Transform the 'Orders' Table.*

Described in the task as the "main fact table", the process to import the **Orders** table was simple in that it was laid out for me. Using the provided server name, I was ablo to access the dummy Azure SQL Database via the 'Get Data' and 'SQL Server Database' options, and then to import the **Orders** table directly into Power BI. 

As per the project guidance, I removed the 'Card Number' column of the **Orders** table to help with ensuring customer's data privavcy. To do this, using the 'Power Query Editor', I simply selected the 'Data' tab, hovered over 'Card Number', right clicked, and pressed "Delete from model".

The next part was then to use the 'Split Column' feature to seperate the columns previously known as "Order Date" and "Shipping Date" into two distinct columns of their own, illustrating the time and date of the order and shipping seperately. To do this, I opened up the Order Date and Shipping Date columns individually in the Power Query Editor (via "Transform Data") and used the Split Colummn function. As the Dates and Times were already separated by a space, I used this as the Delimiter.

The final part of Task 2 was to remove missing or null values from the Orders Date column in order to maintain data integrity. In order to do this, I loaded the Orders Date column into the Power Query Editor and used the Reduce Rows function to remove all of the empty rows.

### Task 3: *Import and Transform the 'Products' Dimension Table.*

Task 3 was to import and transform the **Products** table, which this time was provided as a .CSV file. Once again, I used the built-in 'Get Data' function that Power BI has and selected the .CSV filetype. 

As per project guidance, I removed duplicated rows from the 'Product Code' column to ensure that each product code was unique. To do this, I loaded the newly-imported Products Table into the Power Query Editor, used the "Reduce Rows" function, chose Product Code, and selected "Remove Duplicates".

### Task 4: *Import and Transform the 'Stores' Dimension Table.*

Task 4 did not have too much in the way of guidance in the way of what to do once the **Stores** table had been imported into Power BI. It was more educational on how to work with Azure Blob Storage in Power BI and problem solve with other import types. 

Using the Get Data function as usual, I used the Azure Blob Storage datatype as what I would be importing. Through the course materials, I was provided an Account Name, Account Key and Container Name. The blob function first asked me for the Account Name, followed by the Key. I identified the container name, as provided and imported what was stored on the Blob.  The stored file was parts a web link, which when used with the 'Get Data' - 'Web' function, allowed me to import the Stores.csv table.

### Task 5: *Import and Transform the 'Customers' Table.*

The final task for this Milestone involved importing three provided .CSV files into Power BI and merging them using the inbuilt tools. As part of importing the three files at the same time via 'Get Data' - '.CSV', one of the provided options was to 'Combine and Transform', which effectively merged the three together, meaning that I had a much more accessbile table with all of the **Customers** data in one place.

The next part of working with the **Customers** table was to create a new column titled "Full Name" which merged the customers' First and Last name columns together. I used the Power Query Editor and the function 'Merge Columns' to be able to do this. By highlighting the First and Last name columns and pressing 'Merge Columns', I was then able to specify how I wanted them to be arranged in the new column that was created.
