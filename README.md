##Ecart

A simple nodejs web application made using express framework, having functionalities as those simple Ecommerce website.


### Contents of public folder

The views folder contains all the pages to be rendered, there are 3 pages made in total

 1. A page showing all the inventory list
 2. A page showing the users cart having functionality of **Adding** and **substracting** from cart
 3. A admin page that allows a person to add the items in the inventory with fields **Title, Description , Image Link , Price**

### server.js
 
  This is the file which should be run as **node server.js** to start the application at your local host


### Changes to be done while running on your local host 

 In mysql_scripts , make changes to all the database connection instruction 
   1. make a database you want to use , and replace the database name you are using in the mysql_scripts.
   2. make a connection to your database by your mysql user name and password.

 There's no need to create the tables inside your database. As soon as you run this app , 
 and try to add in add something to product list or to cart, the following query will be 
 executed to form the tables inside the database -

 Query for cart table --- 

         CREATE TABLE IF NOT EXISTS cart (
        id INTEGER AUTO_INCREMENT PRIMARY KEY,
        title VARCHAR(50) NOT NULL,
        description VARCHAR(1000) NOT NULL,
        price INTEGER NOT NULL,
        img VARCHAR(10000) NOT NULL,
        quantity INTEGER NOT NULL
        ) 

 Query for product list table ---

        CREATE TABLE IF NOT EXISTS item (
        id INTEGER AUTO_INCREMENT PRIMARY KEY,
        title VARCHAR(50) NOT NULL,
        description VARCHAR(1000) NOT NULL,
        price INTEGER NOT NULL,
        img VARCHAR(10000) NOT NULL
        )



### Please follow below points to enjoy site view at best
  
  While adding the items in inventory through admin page , in the Image link section , pleae add any relevant image adress from 
  google . Go to googl images and search for product you want to add in inventory . Right click on it and click on **copy image adress**
  and paste in the link field.


  


