# PostgreSQL Joins
https://www.postgresqltutorial.com/postgresql-joins/

* joins work on common columns - usually the *primary key* of the first table and the *foreign key* columns of the second table

* **inner joins** matches values between tables and combines the data

* ***left joins** select data from the left table. It compares values in the fruit_a column with the values in the fruit_b column in the basket_b table. If these values are equal, the left join creates a new row that contains columns of both tables and adds this new row to the result set.

* **left outer joins** return rows from the left table that do *not* have matching rows on the right table.

* you can do the reverse of both of these with **right join** and **right outer join** instead.

* **full join** returns all of the data

* **full outer join** returns all unique data from both tables (no matching data)

# One-to-one (data model)
https://en.wikipedia.org/wiki/One-to-one_(data_model)

* "In a relational database, a one-to-one relationship exists when one row in a table may be linked with only one row in another table and vice versa. It is important to note that a one-to-one relationship is not a property of the data, but rather of the relationship itself."

# One-to-many (data model)
https://en.wikipedia.org/wiki/One-to-many_(data_model)

* "In a relational database, a one-to-many relationship exists when one row in table A may be linked with many rows in table B, but one row in table B is linked to only one row in table A."

# Many-to-many (data model)
https://en.wikipedia.org/wiki/Many-to-many_(data_model)

* "In a relational database management system, such relationships are usually implemented by means of an associative table (also known as join table, junction table or cross-reference table), say, AB with two one-to-many relationships A -> AB and B -> AB. In this case the logical primary key for AB is formed from the two foreign keys (i.e. copies of the primary keys of A and B)."

