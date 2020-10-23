Employee Management System built for client: TracFone Wireless Inc. <br>
Backend for a CRUD application which exposes a REST API for managing the organizational structure of a company. <br>
The system was built with Spring Boot using the Controller-Service-Repository architecture. <br>
<br>
#Technologies <br>
Spring Boot <br>
Spring Security <br>
Spring Data JPA <br>
JUnit <br>
mockito <br>
MySQL <br>
Postman was used to perform HTTP requests. <br>
<br>
#Architecture <br>
Each service is a separate microservice. <br>

Gateway: entry point for other services. Protects other routes and validates tokens. <br>

Auth: authentication server, used for signing up and issuing tokens. <br>

Employee: employee service. <br>

#Install Instruction<br>
1.Clone the source code.<br>
2.Update the /src/main/resources/application.properties with your own DB URL/Password.<br>
3.Update the port number if necesarry(by default it is 7070). <br>
4.If you have MySQL installed, run the script /script/HR20170803.sql to create the tables.<br>
5.Run Application class.<br>
<br>




