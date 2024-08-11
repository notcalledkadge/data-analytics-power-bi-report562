# Data Analytics Power BI Report.
> Milestone 2

### Task 2: *Load and Transform the **'Orders'** Table*

The main focus of Milestone 2 was to import the necessary elements required to produce this report into Power BI, the first part of the puzzle was the **Orders** table. Described in the task as the "main fact table", the process to import the **Orders** table was simple in that it was laid out for me. Using the provided server name, I was ablo to access the dummy Azure SQL Database via the 'Get Data' and 'SQL Server Database' options, and then to import the **Orders** table directly into Power BI. 

As per the project guidance, I removed the 'Card Number' column of the **Orders** table to help with ensuring customer's data privavcy. To do this, using the 'Power Query Editor', I simply selected the 'Data' tab, hovered over 'Card Number', right clicked, and pressed "Delete from model".

The next part was then to use the 'Split Column' feature to seperate the columns previously known as "Order Date" and "Shipping Date" into two distinct columns of their own, illustrating the time and date of the order and shipping seperately. To do this, I opened up the Order Date and Shipping Date columns individually in the Power Query Editor (via "Transform Data") and used the Split Colummn function. As the Dates and Times were already seperated by a space, I used this as the Delimiter.

The final part of Task 2 was to remove missing or null values from the Orders Date column in order to maintain data integrity. In order to do this, I loaded the Orders Date column into the Power Query Editor and used the Reduce Rows function to remove all of the empty rows.

### Task 3: *Import and Transform **'Products'** Dimension Table*
