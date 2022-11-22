# Celestial-Bodies-Database
## Introduction
This project is made while taking the relational-database course of [freeCodeCamp](https://www.freecodecamp.org). This is one of the required projects to earn certification.
he course link is 👉[Relational Database Course by FreeCodeCamp](https://www.freecodecamp.org/learn/relational-database/).

## Description
This database is made using `PostgreSql`. It has following main components:
### Tables
* Galaxy
* Star
* Planet
* Planet_Type
* Moon
### Data-Types and Constraints
👉Each of the tables has a `primary key`, at least two `not nullable` column, a column with `unique` contraint.<br>
👉`Star` table has one `foreign key` referencing a column in `Galaxy` table.<br>
👉`Planet` table has one `foreign key` referencing a column in `Star` table.<br>
👉`Moon` table has one `foreign key` referencing a column in `Planet` table.<br>
👉Data Types such as `INT`, `VARCHAR`, `TEXT`, `NUMERIC`, `BOOLEAN` are used wherever necessary.

## Getting Started
1. Pull repository or download ***universe.sql*** file.
2. Log in to ***PostgreSQL*** with psql. Do that by entering ```psql --username=freecodecamp --dbname=postgres``` in the terminal.  
3. Rebuild the database by entering ```psql -U postgres < universe.sql``` in a terminal where the .sql file is.
4.  You can make a dump of your database by entering  ```pg_dump -cC --inserts -U freecodecamp universe > universe.sql``` in a bash terminal (not the psql one). 
   


