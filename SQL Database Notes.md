# **SQL Notes**
Used mainly for relational databases. Data definition (DDL), manipulation (DML). <br/>
DDL data definition language - schema definitions and changes, DML data manipulation language - changing and querying data. 

Standards:
1. SQL-86
2. 2006 - SQL added XML featured unstructured data (ex: social media has no structure)
3. 2008 - SQL added object oriented features
4. Now: SQL 3 (newest version)

Other languages have compilers but SQL has interpreters not compilers. 

To **end statement** use ;  semicolon
**SQL is case insentive** select = SELECT
**DB is case sensitive** meaning attribute names are case sensitive

##DDL 
schema -  outline of database (relational schema has all info on DB), Authorization identifier, descriptions for elements
elements - Tables, constraints, views, domains, and other constructs

**CREATE SCHEMA statement**
**CREATE SCHEMA COMPANY AUTHORIZATION ‘Jsmith'**

**CREATE Database <nameOfDatabase>**
creates the database first

**CREATE TABLE COMPANY.EMPLOYEE** 
COMPANY - database name 
EMPLOYEE -table name 

OR 

**CREATE TABLE EMPOLOYEE**
creates table in the current database it is in

Table creates a file in the database. 

**CREATE VIEW**
Views are created to see how database is handled. 

CREATE TABLE EMPLOYEE
  (Fname      VARCHAR(15)      NOT NULL
  -
  -
  -
  PRIMARY KEY (Fname) );

Constants: If we write NOT NULL means value cannot be missing, if NOT written then it can be NULL




