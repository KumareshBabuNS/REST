## REST API for CRUD operation,using the jersey,spring,hibernate,MySQL and maven.

Motivation for this project is to provide the head start to beginners for building the REST api,using the popular java open source frameworks and necessary configs.They should be able to build first webservice within 10 minutes.


### Prerequisities
JDK :- 1.7  
Mysql:- 5.6  
Maven  
Tomcat  

### Installing
1.Clone the project.<br>
2.If maven is setup properly in your system. then you can download all the required dependency and build war using the maven by using below command.<br>
 **mvn clean package**<br>
3.Open db.sql and run the sql commands in your mysql terminal.<br>
4.Change the username and password to your mysql username in context.xml.<br>
5.Go to the target folder and copy the rest.war file and put it in tomcat webapps folder and start the server.<br>

### API Documentation.
To test the REST API , use any rest client like postman etc.<br>
1.Create product api (sample)<br>
URL :- localhost:8080/rest/api/products/<br>
header :- content-type :- application/json<br>
method :- post<br>
body :- {<br>
    "name" : "first product",<br>
    "description" : "sample"<br>
}<br>
After hitting this api , new product must be created inside the rest database's product table. 
you can check this by firing the sql query on mysql terminal.<br>
2.Get product api (sample)<br>
URL :- localhost:8080/rest/api/products/{id}<br>
provide the id , which you get as a response from create product api , in the url , you will get its all the information.

## Automated test cases will be added later.
