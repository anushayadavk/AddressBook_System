#UC2 Ability to create a Address Book Table with first and last names, address, city, state, zip, phone number and email as its attributes
mysql> create table Adressbook (
    -> id int NOT NULL AUTO_INCREMENT PRIMARY KEY,
    -> first_name varchar(150) NOT NULL,
    -> last_name varchar(150) NOT NULL,
    -> adress varchar(150) NOT NULL,
    -> state varchar(150) NOT NULL,
    -> city varchar(150) NOT NULL,
    -> zip varchar(100),
    -> email_adress varchar(150) NOT NULL,
    -> phone_number varchar(15)
    -> );

mysql> insert into Adressbook (first_name,last_name,adress,state,city,zip,email_adress,phone_number) values
    -> ('Anusha','Yadav','Rajajinagar','Karnataka','Bangalore','560010','anu@gmail.com','8105561103');

mysql> select * from Adressbook;
+----+------------+-----------+-------------+-----------+-----------+--------+---------------+--------------+
| id | first_name | last_name | adress      | state     | city      | zip    | email_adress  | phone_number |
+----+------------+-----------+-------------+-----------+-----------+--------+---------------+--------------+
|  1 | Anusha     | Yadav     | Rajajinagar | Karnataka | Bangalore | 560010 | anu@gmail.com | 8105561103   |
+----+------------+-----------+-------------+-----------+-----------+--------+---------------+--------------+
1 row in set (0.12 sec)
