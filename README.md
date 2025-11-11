# portfolio
sample-sql
Last login: Tue Nov 11 20:37:45 on ttys000
amane.t@WAVE ~ % mysql -u root -p
Enter password: 
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 13
Server version: 9.5.0 MySQL Community Server - GPL

Copyright (c) 2000, 2025, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> CREATE DATABASE ZooDB;
Query OK, 1 row affected (0.004 sec)

mysql> USE ZooDB;CREATE TABLE AnimalTable (
Database changed
    ->     animal_id INT PRIMARY KEY AUTO_INCREMENT,
    ->     Name VARCHAR(50),
    ->     Species VARCHAR(50),
    ->     DateOfBirth DATE,
    ->     Gender VARCHAR(10),
    ->     Enclosure VARCHAR(50)
    -> );
Query OK, 0 rows affected (0.015 sec)

mysql> INSERT INTO AnimalTable (Name, Species, DateOfBirth, Gender, Enclosure)
    -> VALUES ('LELE', 'Panda', '2025-11-11', 'Female', 'Cute Zone');
Query OK, 1 row affected (0.005 sec)

mysql> SELECT * FROM AnimalTable;
+-----------+------+---------+-------------+--------+-----------+
| animal_id | Name | Species | DateOfBirth | Gender | Enclosure |
+-----------+------+---------+-------------+--------+-----------+
|         1 | LELE | Panda   | 2025-11-11  | Female | Cute Zone |
+-----------+------+---------+-------------+--------+-----------+
1 row in set (0.001 sec)

