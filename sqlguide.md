# WHAT IS DATABASE:

database is collection of data in a format tat is easily accesible

# WHAT IS DBMS:

dbms is a software use to manage the database.
dbmas is used to interact a user with the data base.

# TYPES OF DATABASES:

- 1. RELATIONAL DATA BASES : In which data is stored in the form of tables.(also called sql (because they understand the sql language)) some examples of relational databases are: mysql,oracle
- **CRUD OPERATIONS:**

* **create:**used to create the datavbase

- **Read:**used to read data from the tables

* **update:**update the data

- **DELETE:**to delete the data

**HOW TO INSTALL MYSQL:**

-3. Go to mysql.com
*4. go to downloads option (now scroll to bottom and select (mysql community download option)).
-5. then go to my sql community server option.
*6. and then select the operating system for which you want to download and then download .

- We also need to download my sql workbench for this follow the following steps:
  *7. Go to mysql.com
  -8. go to downloads option (now scroll to bottom and select (mysql community download option)).
  *9. then go to my sql workbench option.
  -10. and then select the operating system for which you want to download and then download .
  To create connection. go to + icon on workbench add username password hostname to create connection.

### WHAT IS A TABLE:

table is a combination of rows and coloumns coloumns determine the structure and rows determine the data .

#### HOW TO CREATE AND DELETE DATABASE:

- To create data base use create database databasename
  there is another version of create database command that is: create data base if notexist (it creates if there is not such data base created already)

* To delete use the command drop database databasename
  there is another version of create database command that is: create data base
  if exists (it creates if there is not such data base created already)

- **show database** is used to show the databases that exist in your server.
  show table shows all the tables of the database that you are currently using.

* **CRETAE TABLE COMMAND**: it is used to crate the table i.e. create table tablename(colname datatype CONSTRAINT)

- **INSERT COMMAND** : insert command is used to insert the data in the rows of the table. syntax: insert into tablename (col1name,col2name) values(col1val1,col2val1),(col1val2,col2val2)

* **UPDATE COMMAND:** it update data of the existing table
  syntax: update tablename colname =value where condition.

- **ALTER COMMAND:** it is used to change the schema of the tabele using the following cmmands:

* (1) ADD coloumn:it will add a coloumn (ex: alter table tablename add coloumn coloumnname datatype CONSTRAINT)

- (2) DROP:to delete a coloumn (ex: alter table tablename drop coloumn columnname)

* (3) CHANGE: to change the column name or data type (ex: alter table tablename change columnoldname column newname datatype new constraint)

- (4) MODIFY:used to modify datatype and constraint(ex:alter table tablename modify columnname newdatatype new constraint)

- **TRUNCATE COMMAND:** used to delete tables data the main difference between drop and truncate is drop deletes the table whereas truncate only deletes the data. i.e. truncate table tablename.

### TYPES OF KEYS:

-1.**primary key:**it is a colounms or set of colounms in a tablethat uniquly identifies a row(there could be only one primary key it will not be null)
\*2.**Foreign key:** it is a colounms or set of colounms in a table that refers to the primary key in other table.( there could be multiple foreign keys)

### CONSTRAINTS:

sql are used to specfy rules for data ina table

#### TYPES OF CONSTRAINT:

*1. **NOT NULL:** coloumn can not have a null value .
-2. **Unique:** all value sin colounmn must be unique.
*3. **primary key:** makes a coloumn unique and not null.
-4. **foreign key:** prevent actions that destroy link between tables.
\*5. **default:** used to set default value for a coloumn.
-6. **check:** used to limit the values allowed in a coloumn. -**SELECT QUERY:**Used to select the specified data from the table: - select colname1,colname2 from tablename(to select the specified coloumns) + select\* from tablenamae(to select all coloumns from table ) +** WHERE CLAUSE:**where clause is used with select to specify condition on which data is selected.i.e: - select colname from tablename where condition.

### OPERATORS:

operators are used in where clause to specify conditions.

#### TYPES OF OPERATORS:

-1.**AIRTHEMETIC OPERATORS:**used to to airthmetic operations (such operators are +,-,\*,/,%) + 2.**COMPARISON OPERATORS:** used to compare the values(such operators are = !=,>,>=,<=) 3.**LOGICAL OPERATORS:** some logical are between,AND OR ,NOT,IN
-(i) AND : chcks both condition are true:i.e. select \_from table name where condition1 and condition2

- (ii) OR :chcks for only one condition to be true:i.e. select _ from table name where condition1 or condition2
  _ (iii) BETWEEN: Select data for a given range(i.e. select \_ from students where marks between 80 and 90)

* (iv) IN: matches any value for the data(i.e. slect \_from cities where city in ("karachi","lahore"))

- (V) NOT:used to negate the condition(i.e. slect _from cities where city not in ("karachi","lahore"))
  **limit clause:** use to set upper limit on the number of rows to be selected.
  i.e select _ from students limit 3.
  **\*ORDERBY CLAUSE:** it sorts the data in ascending or descending ORDER. - i.e select \_ from students ORDER BY marks ASC.(if you want in descending order use DESC in place of ASC).

#### AGREGATE FUNCTIONS:

AGREGATE FUNCTIONS are fuctions that are used to perform calculation on given set of data. SOME AGREGATE functions are given below.

- **COUNT():**returns the count of elements + **AVG()**:return the average +**SUM():**returns the sum of the values
- **MIN():**return min value

* **MAX():** returns max value

- **GROUP BY CLAUSE:** it groups rows that have the same value
  i.e. select city from students group by city.

* **HAVING CLAUSE:** same as where but where can not be used on groups it is only used on rows.
  i.e. select city from students group by city HAVING marks>90.

### JOINS:

joins are used to combine rows of different table based on related coloumns.

#### TYPES OF JOINS:

- 1. **INNER JOIN:**return data that is matched in both tables . syntax: select coloumnname fom tablea innerjoin tableb on tablea.coloumnname=tableb.coloumnname

* 2. **LEFT JOIN:**return all data from left table and matched data from right table
     syntax: select coloumnname fom tablea left join tableb on tablea.coloumnname=tableb.coloumnname.
     \*3. **RIGHT JOIN:**return all data from right table and matched data from left table
     syntax: select coloumnname fom tablea right join tableb on tablea.coloumnname=tableb.coloumnname.
     -4. **FULL JOIN :** returns all the data from both tables.
     syntax: select coloumnname fom tablea FULL join tableb on tablea.coloumnname=tableb.coloumnname.
     +5. **UNION:** union is used to combine the the results of two select statements(it give unique values)
     syntax: select coloumnname from table1 union select coloumnname from table2

- **SUB QUERIES:** sub query is a query within another query
  example:select names from student where marks >(Select avg(marks) from students )
