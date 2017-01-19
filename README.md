## CS122B: Project 1 (Group 21)
### By Sihan Xu(60407382) & Yigan Zhang(18324490) & Yuting Xue(31323149)
  This file is mainly to guide you to create a MySQL database with provided movie information and shows the steps using a Java program to connect to the database with JDBC.
### Create MySQL Database
  login MySQL
  ```
  mysql -u root -p
  ```
  Create a table with createtable.sql
  ```
  source createtable.sql
  ```
  Populate the table with data.sql
  ```
  source data.sql
  ```
  
### Connect to database with JDBC
First, you need to compail and run the java program.
```
sudo javac JDBC1.java
sudo java JDBC1

```
#### Print out (to the screen) the movies featuring a given star.
input ID / First name /last name to get star information     
If none of them is valid, you will be asked to input again.    
If there is no information found according to your inputs, you will see: cannot find information in the table.    

#### Insert a new star into the database.
 You will be asked about the star's first name, last name, date of birth `YYYY-MM-DD` and url.    
 If you only insert one name, it will be treated as last name.     
 Once you successfully inserted a customer, you will see `Insert OK,1 row effected`.    
 
#### Insert a customer into the database.
 You will be asked about the customer's first name, last name, cc_id, address, email and password.   
 Like:   
 `please insert first name:`    
 If the cc_id is not in the table, you will see `cannot insert`.    
 If you only insert one name, it will be treated as last name.   
 To get a success insert, you need a name and a valid cc_id.    
 Once you successfully inserted a customer, you will see `Insert OK,1 row effected`.    

#### Delete a customer from the database.
  You will be asked to enter the id of the customer you want to delete.    
  If the id is valid, you will see `delete OK, 1 row effected`   
  If the id is invalid, you will see `delete OK, 0 row effected`   
  
#### Provide the metadata of the database
  Under the information of whether the customer is successly deleted, you will see metadata of database automatically.    

#### Enter a valid SELECT/UPDATE/INSERT/DELETE SQL command.
 In this part, you can enter any valid SELECT/UPDATE/INSERT/DELETE SQL command to get the right ressult.    
 If your enter is invalid, you will see`Your input is not valid`.   
 To use SELECT:     
 ```
 select id from stars    
 ```
 You will id of all stars.    
 If UPDATE/INSERT/DELETE is successed, you will see`Insert OK,1 row effected`.    
  
The program is over.    
  
  Thanks for reading :blush:    
  
    
