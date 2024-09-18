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
<h4>Required MySql server running Locally</h4>
<ul>
  <li>java -jar spring-petclinic.jar</li>
  <li>java -jar VisitService.jar</li>
  <li>java -jar VetService.jar</li>
  <li>java -jar PetService.jar</li>
  <li>java -jar -DDEMO_EXTERNAL_URL=https://www.google.co.in/ -DDEMO_CPU_MILLIS=500 -DDEMO_SLOW_SQL_QUERY=true -DDEMO_SLOW_SQL_QUERY_MILLIS=1300 -DDEMO=true OwnerService.jar</li>
</ul>







