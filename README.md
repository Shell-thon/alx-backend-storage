## 0x00. MySQL advanced

### Concepts
For this project, we expect you to look at this concept:

- Advanced SQL

### Resources
Read or watch:

- [MySQL cheatsheet](link_to_cheatsheet)
- [MySQL Performance: How To Leverage MySQL Database Indexing](link_to_performance_guide)
- [Stored Procedure](link_to_stored_procedure)
- [Triggers](link_to_triggers)
- [Views](link_to_views)
- [Functions and Operators](link_to_functions_operators)
- [Trigger Syntax and Examples](link_to_trigger_examples)
- [CREATE TABLE Statement](link_to_create_table)
- [CREATE PROCEDURE and CREATE FUNCTION Statements](link_to_create_proc_func)
- [CREATE INDEX Statement](link_to_create_index)
- [CREATE VIEW Statement](link_to_create_view)

### Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

#### General
- How to create tables with constraints
- How to optimize queries by adding indexes
- What is and how to implement stored procedures and functions in MySQL
- What is and how to implement views in MySQL
- What is and how to implement triggers in MySQL

### Requirements
#### General
- All your files will be executed on Ubuntu 18.04 LTS using MySQL 5.7 (version 5.7.30)
- All your files should end with a new line
- All your SQL queries should have a comment just before (i.e. syntax above)
- All your files should start by a comment describing the task
- All SQL keywords should be in uppercase (SELECT, WHERE…)
- A README.md file, at the root of the folder of the project, is mandatory
- The length of your files will be tested using wc

### More Info
Comments for your SQL file:
```sql
-- 3 first students in the Batch ID=3
-- because Batch 3 is the best!
SELECT id, name FROM students WHERE batch_id = 3 ORDER BY created_at DESC LIMIT 3;Use “container-on-demand” to run MySQL Ask for container Ubuntu 18.04 - Python 3.7 Connect via SSH Or via the WebTerminal In the container, you should start MySQL before playing with it:$ service mysql start
 * MySQL Community Server 5.7.30 is started$ cat 0-list_databases.sql | mysql -uroot -p my_database
Enter password:
Database
information_schema
mysql
performance_schema
sysIn the container, credentials are root/rootHow to import a SQL dump:$ echo "CREATE DATABASE hbtn_0d_tvshows;" | mysql -uroot -p
Enter password:
$ curl "https://s3.amazonaws.com/intranet-projects-files/holbertonschool-higher-level_programming+/274/hbtn_0d_tvshows.sql" -s | mysql -uroot -p hbtn_0d_tvshows
Enter password:
$ echo "SELECT * FROM tv_genres" | mysql -uroot -p hbtn_0d_tvshows
Enter password:
id  name
1   Drama
2   Mystery
3   Adventure
4   Fantasy
5   Comedy
6   Crime
7   Suspense
8   ThrillerPlease replace the placeholder links (`link_to_cheatsheet`, `link_to_performance_guide`, etc.) with actual URLs to the respective resources.