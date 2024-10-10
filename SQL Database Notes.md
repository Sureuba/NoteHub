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

###Authorizations
**CREATE SCHEMA statement**
**CREATE SCHEMA COMPANY AUTHORIZATION ‘Jsmith'**

###Creating Database
**CREATE Database <nameOfDatabase>**
creates the database first

###Creating a Table

**CREATE TABLE COMPANY.EMPLOYEE** 
COMPANY - database name 
EMPLOYEE -table name 

OR 

**CREATE TABLE EMPOLOYEE**
creates table in the current database it is in

Table creates a file in the database. 

**CREATE VIEW**
Views are created to see how database is handled. 


**CREATE TABLE EMPLOYEE** <br />
**(Fname      VARCHAR(15)      NOT NULL**  
  
  -
  -
**PRIMARY KEY (Fname) );** <br />

###How to change a table:
**ALTER TABLE EMPLOYEE**

###Creating a table with foreign key <br />
**(Fname      VARCHAR(15)      NOT NULL**  
  
  -
  -
**PRIMARY KEY (Dnumber)** <br />
**UNIQUE(Dname)** <br />
**FOREIGN KEY (Mgr_ssn) REFERENCES EMPLOYEE(Ssn) );** <br />

Foreign keys: may have circular reference
Unique means it is also unique but not a Primary Key

###TABLE notes:

you can skip constants
can skip primary key specification

**Constants**: If we write NOT NULL means value cannot be missing, if NOT written then it can be NULL

###**Datatypes**:
Integer (int)
Smallint
Float 
Real

char - digits or alpha numeric
char(n) means length MUST be n
char means length is 1

varchar(n) - means its max length can be n but it can be any # of characters below n
Character varying (n)

Boolean
Bit(n) - fixed bit-string datatype
Bit varying(n) - not fixed

DATE YY-MM-DD
TIMESTAMP - todays date and what time now
TIMESTAMP with timezone 
INTERVAL

###Domains
CREATE DOMAIN SSN_TYPE as CHAR(9)

Used in:
CREATE TABLE EMP (SSN     SSN_TYPE     NOT NULL, ...);

###Other constrains on Attributed Domains
DEFAULT <value>

Can also CHECK:
Dnumber    INT     NOT NULL CHECK (Dnumber > 0 AND Dnumber < 21

###Key Constraints

PK- chooses a PK
Unique - Candidate key
FK - has options : 
  1. SET NULL
  2. CASCADE
  3. SET DEFAULT
  4. 

