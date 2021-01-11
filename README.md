# Bits & Bots Rubric
CSE 3241 - Introduction to Database Systems | AU20 Final Project

Sam Bossley, Michael Izzo, Josephine Ko, Henry Xiong

# Overview
You and your project team are employed by DB 4Ever., a consulting company with clients worldwide. You’ve been assigned to help Ms Yotta Bietz set up a database for her latest entrepreneurial enterprise, BITS & BOTS.
The application will be a kind of online marketplace for the maker community. It will permit makers to set up small virtual storefronts for securely distributing intellectual property, collecting payments and interacting with users.

Ms. Bietz needs a simple information management system and database to support virtual inventory, buyer/seller accounts, and sales operations. You have been given some sample data and test scenarios. You will need to supplement your solution with features that you consider important or interesting.

Your final document will include a relational database schema, entity relationship diagram, relational algebra and SQL statements, documentation on indexing, transactions, and normalization.

You and your team mates will work on this project independently all semester. You will receive feedback (but no points) for submitting four checkpoint documents.

In addition, to receive full credit for your project you will be required to make sure that your design:
1. Allows for proper handling of buyer /seller interactions such as orders, payments, feedback, and karma points
2. Offers additional features that expand on the initial requirements

a) Sample data:

Yotta Bietz has suggested that you look at sites like 3dcart, etsy, ebay, and shopzilla for examples of online spaces that cater to multiple sellers and buyer. Look at their order forms and reports to determine the necessary data items, their types, constraints and relationships.
Also look at www.makershed.com to get an idea of what the buyer/seller type of user is like, but remember that Bits & Bots will only sell non-physical items (for instant gratification).
You will need to create your own buyer and other data. (Look online for sites that generate random data for testing) You should put enough test data into your database in order to run the assigned queries and test the scenarios. It is important that you have enough test data to generate reasonable results for each of the assigned queries, your views and transactions.

b) Test Scenarios:

The database should be able to support the usual operations of an online store. That is, that buyers search for different items, make purchases and review their accounts. Sellers should be able to create new listings and see sales reports on what items have sold.
The intellectual property may be source code, executables, CAD files, PDFs, images and other file formats. All will all be stored as files in the system.

# Final Project Document Description
The final report must be a professionally presented, well-organized, typed document, with a complete SQL database, submitted electronically to the Carmen Dropbox in a single ZIP file. This ZIP file needs to be neatly and professionally organized, with all filenames appropriately chosen, and all files suitably organized into subdirectories. Include a Table of Contents file named README.txt that explains the layout of your files, including where to find each of the following files in your file structure.

# Outline
## Part I – The Final Report
### Section 1 - Database Description
a. ER – Model properly documented
b. Relational schema properly documented
c. Database fully normalized, with correct justifications
d. Relational schema and SQL for two views
e. Two indexes properly documented
f. Two sample transactions

### Section 2 - User Manual
a. Description with “Extra” entities included and discussed
b. Sample SQL Queries (from CP02 and CP03)
c. INSERT samples
d. DELETE samples

### Section 3 - Graded Checkpoint Documents
Marked Project Checkpoints and Worksheets.
Description of additional work-in-progress, any feedback and revisions Part II – The SQL Database
*.sqlite, or *.db binary:
correctly formatted, and ready to open with SQLiteOnline (https://sqliteonline.com/)
*.txt:
SQL statements for your DB, as simple text files

# Details
## Part I – The Final Report
Your final document will include a relational database schema, entity relationship diagram, SQL queries, and reports, as indicated below.

### Section 1 - Database Description
A database description document that contains the following information about your database (compiled from your completed and revised checkpoints);

a. A professionally presented, well-formatted ER-model that reflects the updates you have made during the semester. Do not submit a hand-drawn diagram.

b. A professionally presented, well-formatted relational schema for the database. This schema must be annotated with the primary key for each table, all foreign keys on all tables, and all functional dependencies on all tables. Make sure that connections between FKs and PKs are clear.

c. For each table, give a brief description of the level of normalization achieved for that table. If the table is not in BCNF, explain why.

d. A description of each of the two indexes that you have chosen to implement on your database, along with rationale for each.

e. A complete description of two sample views useful for your database. For each view that you have implemented, provide the following:
   - i. A brief description in English of what this view produces, and why it would be useful.
   - ii. Relational algebra expression to produce this view.
   - iii. SQL statements to produce the view.
   - iv. Sample output from the view, with 5-10 lines of data records shown.

f. A professionally presented description of two sample transactions useful for your database. This should
include the sample SQL code for each transaction as well as an English language description of what “unit of work” the transaction represents. The transaction should include read and/or write operations on at least two tables, with appropriate error and constraint checks and responses.

### Section 2 - User Manual
A user manual describing the usage of your database, for use by developers who are going to be writing code to use your database. Your manual should include:

a. For each table, explain what real world entity it represents. Provide a description of each attribute, including its data type and any constraints you have built.

b. The sample SQL queries that you provided in Checkpoints 02 and 03. These
queries should be organized and presented neatly and professionally. Each query
should include:
   - An English language description of what the query should be returning
   - The correct relational algebra syntax of the query
   - The equivalent SQL query

c. INSERT syntax for adding new items, orders, sellers and buyers to your system. If there are dependencies in your system that require multiple records to be added to tables in a specific order to add one of these items, make sure you clearly indicate what those restrictions are.

d. DELETE syntax for removing items, orders, sellers and buyers from your system. Again, indicate any dependencies that exist on the order that the steps in your DELETE must take. In addition, provide an example set of DELETE statements for each entity in your database.

### Section 3 - Graded Checkpoint Documents
You will start work on the project immediately and work on it incrementally all semester. Some work will be done during class time, but most of your effort will be with your team.

Four checkpoint (draft) documents will be submitted during the semester so that your instructor can give you feedback and any necessary corrections.

An appendix to the final report that MUST contain all of your original, graded checkpoint documents organized in a neat and professional manner. For each checkpoint that required a revision you MUST include a revision for that checkpoint. This revision may be a pointer to where in the final database document the “fixed” version of the checkpoint resides (“See Section X Page Y for the new relational model diagram” for example).

## Part II – The SQL Database
1. A binary version of your database, suitable for opening with the SQLiteOnline application (*sqlite, *.db).
2. Text formatted SQL. These files, when used with the table creation scripts above, should be able to recreate your database from scratch if your binary file is corrupted or lost. Make sure you provide instructions on how to use these scripts and files in a separate text file. (NOTE: there are free tools that will automatically generate the SQL to create your database from an appropriately formatted DB file)
   - SQL CREATE . A text file containing all of the scripts needed to create your database schema on an empty database. This file should be properly commented and should execute properly if pasted into an SQL interpreter. These scripts should include all indexes and views created on your database.
   - SQL INSERT. A plain-text file containing instructions to load the data into your database tables.
   - SQL QUERIES. A text file containing all of the SQL queries used in your final report from Part I/Section 2. All of these queries must should execute properly if pasted into an SQL interpreter. In addition, make sure that these queries are completely commented so that it is clear where the query comes from in your final report writeup.
   - SQL INSERT/ DELETE. A text file containing all of the sample INSERT and DELETE statements provided in your user manual (Part I/Section 2), suitable for pasting into a command prompt and testing the result on your database.
