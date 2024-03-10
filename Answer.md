1) Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.
   => The relationship between the "product" table and the "product category" table is typically a one-to-many relationship. This means that one product can belong to only one product category, but one product category can have multiple products associated with it.

   

2) How could you ensure that each product in the "Product" table has a valid category assigned to it?
   => To ensure that each product in the "product" table has a valid category assigned to it, we can make referential integrity through the use of foreign key constraints. 
In the "product" table, we would have a column that serves as a foreign key referencing the primary key of the "product category" table. This foreign key constraint ensures that every value in the "product" table's category column points to a valid category in the "product category" table. If an attempt is made to insert or update a row in the "product" table with a category that doesn't exist in the "product category" table, it would be rejected to maintain data integrity in the table.
