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

<h2>how to start the spring petclinic microservice localy</h2>
<br>

Step 1 : Required MySql server running Locally.
<br>
Step 2 : Run the Mysql script file available in mysql folder named "petclinic_database_sql_data.sql" before starting servers.
<br>
Step 3 : Run below command after preapring executable jar from source. 
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






