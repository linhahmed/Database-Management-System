# DBMS
Implement a simple DBMS that handles data stored in XML files.
The following SQL Statements is supported:
* Create database       * Create table
o Insert into table
o Delete from table

o Drop database
o Drop table
o Select from table
o Update table

3. The DBMS you will develop should control the management and retrieval of data
from data files. The DBMS accepts requests for data from application programs
(in the form of the SQL queries) and retrieves and transfers the appropriate data
from files that are stored physically on disk.
4. SQL is case insensitive in the statement and in the data base name (folder and
files).
5. You can find detailed statements descriptions at: http://www.w3schools.com/sql
6. You should support the “SELECT * FROM table;” statement.
7. For statements which contain conditions (i.e. the Where clause), support only the
simple conditions: =, >, and <. You are NOT required to support multiple
conditions: AND, OR, or NOT. (If you did, it will be bonus).
8. The table should support only two types: varchar and int. “varchar” used to store
string, and “int” to store numeric values (no floating point will be supported). Do
not support custom type lengths (e.g. varchar(255), or int(11) ), just assume all
types of the same default length. However, you should make your design
extensible.
9. The DBMS interface does NOT handle SQL queries directly. SQL queries should be
sent first to another class, say Parser class. The Parser parses them, and then calls
the appropriate DBMS function. The Parser should use only the functions
supported by the DBMS interface to access the database. The files should be
updated, whenever any DBMS function (that requires updating) is called.
10.The Parser should validate the SQL statements and reject bad ones.

11.The DBMS should validate the sent parameters and should throw appropriate
exceptions whenever needed.
12.Each table in the database should be stored in a separate XML file. Files should be
placed in the database directory.
13.You should maintain “Schema files” that contain data about the tables and
columns. Tables should be validated across their schema files (“DTD or XSD Files”
can be used for this purpose).
14.This means each table will have at least two files: one for data (XML file), and one
for its structure (DTD or XSD file)
15.You should use SAX or DOM, or StAX parsers to parse and validate the XML
database files.
16.You should provide a command line interface that accepts SQL queries.
17.You are required to create a UML class diagram.
