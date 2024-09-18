# spring-petclinic-microservice-local
<br>
spring-petclinic-microservice-local deployment only
<br>
<br>
<h2>Default port details of each microservice</h2>
<br>
<br>
<ul>
  <li>OwnerService = 4000</li>
  <li>PetService = 3000</li>
  <li>Spring-petclinic = 8080</li>
  <li>VetService = 5000</li>
  <li>VisitService = 6000</li>
</ul>
<br>
<h2>To run this microservice required JRE 1.8 version</h2>
<br>

<h2>configuring database for spring petclinic microservice localy</h2>
<br>

Step 1 : Required MySql server running Locally.
<br>
Step 2 : Run the Mysql script file available in mysql folder named "petclinic_database_sql_data.sql" by following below steps.
<br>
Step 3 : Create a database with name 'petclinic'. 
<br>
Step 4 : run below command by navigating to 'MySQL_installed_directory\bin' for example 'C:\Program Files\MySQL\MySQL Server 8.0\bin'
<br>
Command : mysql --host=localhost --user=xxxx --port=3306 -p petclinic < D:\Sprng-petclinic\spring-petclinic-microservices-master\mysql\petclinic_database_sql_data.sql
<br>
Step 6 : provide the password to import the tables and data into database.
<br>

<h2>how to start the spring petclinic microservice localy</h2>
<br>
Run below command after preapring executable jar from source. 
<br>
<ul>
  <li>java -jar spring-petclinic.jar</li>
  <li>java -jar VisitService.jar</li>
  <li>java -jar VetService.jar</li>
  <li>java -jar PetService.jar</li>
  <li>java -jar -DDEMO_EXTERNAL_URL=https://www.google.co.in/ -DDEMO_CPU_MILLIS=500 -DDEMO_SLOW_SQL_QUERY=true -DDEMO_SLOW_SQL_QUERY_MILLIS=1300 -DDEMO=true OwnerService.jar</li>
</ul>

<h2>Accessing the spring petclinic microservice</h2>
<br>
<ul>
  <li>Home Page : http://localhost:8080/</li>
  <li>Error Page : http://localhost:8080/oups</li>
  <li>Slow SQL : http://localhost:8080/owners?lastName=</li>
  <li>External HTTP call : http://localhost:8080/owners/find</li>
</ul>






