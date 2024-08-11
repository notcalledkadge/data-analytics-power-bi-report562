# Data Analytics Power BI Report.
## Milestone 2
### Task 2. Load and Transform the "Orders" Table.
The main focus of Milestone 2 was to import the necessary elements required to produce this report into Power BI, the first part of the puzzle was the **Orders** table. Described in the task as the 'main fact table', the process to import the **Orders** table was simple in that it was laid out for me. Using the provided server name, I was ablo to access the dummy Azure SQL Database via the *Get Data* and *SQL Server Database* options, and then to import the **Orders** table directly into Power BI. 

As per the project guidance, I removed the 'Card Number' column of the **Orders** table to help with ensuring customer's data privavcy. The next part was then to use the *Split Column* feature to seperate the columns previously known as "Order Date" and "Shipping Date" into two distinct columns of their own, illustrating the time and date of the order and shipping seperately.
