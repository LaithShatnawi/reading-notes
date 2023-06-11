# Data Modeling

## nosql vs sql

### 1.What type of database is the best fit for the complex query intensive environment?

SQL database

### 2.What type of database is the best fit for hierarchical data storage?

NOSQL database

### 3.Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.

sql can be used for larger scale projects where it uses relations between tables (meaning that you can access data that is dependent upon each other easly).

### 4.How do we treat keywords and parameters differently in SQL syntax?

for the keywords we would use ubbercase syntax as its the best practice, as for the parameters specific syntax varies depending on the database system you are using, it includes (?) and (:).

### 5.Define normalization within the context of schemas and data.

normalization is a way of organizing the data between tables so that we dont have unnecessary and redundant data.

### 6.Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.

one-to-one: we can imagine its a relationship between two persons where you can only have one item(row of data) from the other person.

one-to-many: its a relationship where you can have more than one item(row of data) from the other person.

many-to-many: its a relationship where you can have more than one item(row of data) from the other person and vise-versa.

## sql modeling techniques

### 1.Among data tables, what is a one-to-many relationship and how do we “relate” them?

its a relationship between to two tables in which you can have more than one row of data in that other table but not the other way around.
we can relate them using a foreign key and joining the data from both tables.

### 2.Prior to designing your relational database, it might be useful to ___ a ___ of the database tables and their relationships.

create a conceptual model.

### 3.Explain the difference between a primary and foreign key.

the primary key is the main key for the data in the table which is unique to that item. the foreign key on the other hand is actually a primary key for another table hence the name foreign, which is used to connect the two tables based on a condition.