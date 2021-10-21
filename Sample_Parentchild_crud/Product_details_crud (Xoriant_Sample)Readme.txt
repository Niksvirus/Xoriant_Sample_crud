for Postman:


1)Post:

URL: http://localhost:9191/addProduct     ............to add single product
URL:http://localhost:9191/addProducts     ............to add multiple products
[{
"name":"xorlaptop",
"quantity":"5",
"price":"10000"
}
    ]

2)Get:

for all products

http://localhost:9191/products


get profuct by id: 


http://localhost:9191/productById/{id number}


get profuct by name:



http://localhost:9191/product/{name}



3)Update :

http://localhost:9191/update



4)Delete :

URL:http://localhost:9191/delete/{id}