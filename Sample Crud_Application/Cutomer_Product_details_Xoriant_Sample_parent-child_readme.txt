Application to store customer and product details associated with each customer


need to create schema "xoriant_Assign" before running the jar


find the port details and properties which you need to change before running this project

spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.url = jdbc:mysql://localhost:3306/xoriant_Assign
spring.datasource.username = root
spring.datasource.password = root
spring.jpa.show-sql = true
spring.jpa.hibernate.ddl-auto = update
spring.jpa.properties.hibernate.dialect = org.hibernate.dialect.MySQL5Dialect
server.port=9191



Note:instead of using enity classes we have created dto classes



1)Post: 
 
URL: http://localhost:9191/placeOrder
To insert customer 
and products purchased by him

whereas under one customer you can place multiple products which are purchased by him.

{
 "customer": 
  {
   "name":"Nikhil",
   "email":"gsgsasc@gmail.com",
   "gender":"Male",
   "products":
      [
     {
       "pid":101,
       "productName": "Xoriant_laptop",
       "price": 10000,
       "qty" : 2
     },
        {
          "pid":102,
          "productName": "Xoriant_Web",
          "price": 20000,
          "qty" : 3      
        }
      ]
   }
}




2)Get 

To display all customer order details 

URL: http://localhost:9191/findAllOrders








