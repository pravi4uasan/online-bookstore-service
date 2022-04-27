# online-bookstore-service
This is a backend Rest API application, used to perform CRUD and checkout operations in Book Store
# Technologies Used :
Java 8 ,Spring Boot,H2 DB ,Maven

# Use Case :

Create a REST API for an online bookstore, where the user can perform the following operations:
CRUD operations on Books 

Checkout operation for single or multiple books which will return the total payable amount.
# Considerations :
Book object should have the following attributes:

Name ,Description ,Author ,Type/Classification ,Price ,ISBN

Checkout method will take list of books as parameters plus optional promotion code and return total price after discount (if applicable).

Promotion/Discounts is variant according to book type/classification, ex: fiction books may have 10% discount while comic books have 0% discount.

# Source Code :

Clone the below repository 

git clone https://github.com/pravi4uasan/online-bookstore-service.git

# Build :
Open the Terminal then Navigate to online-bookstore-service and execute below command

mvn clean install

# Deployment in Local :

mvn spring-boot:run

   OR 
   
Goto project and select OnlineBookStoreApplication.java and run as Java Application in Eclipse

# Docker Build :

Use Dockerfile from project root directory to build docker images

docker build -f Dockerfile -t onlinebookstoreapp .

# Docker Run :
 docker run -p 9900:8080 onlinebookstoreapp

# Database Access

Hit this Datasource URL in a browser: http://localhost:8080/h2-console

To connect data source use below credentials

JDBC URL : jdbc:h2:mem:bookdb

User Name : sa

Password :

# Discount Catalogue :
FICTION(10)

COMIC(0)

ACTION(10)

THRILLER(10)

TECHNOLOGY(0)

SCIENCE(5)

POETRY(20)

OTHERS(30)

# Application Testing in Postman

Use below given postman collection from project root folder and import in Postman

Online Book Store.postman_collection.json




