Employee Management System built for client: TracFone Wireless Inc. <br>
Backend for a CRUD application which exposes a REST API for managing the organizational structure of a company. <br>
The system was built with Spring Boot using the Controller-Service-Repository architecture. <br>
<br>
# Technologies <br>
Spring Boot <br>
Spring Security <br>
Spring Data JPA <br>
JUnit <br>
mockito <br>
MySQL <br>
Postman was used to perform HTTP requests. <br>
<br>
# Architecture <br>
Each service is a separate microservice. <br>
Gateway: entry point for other services. Protects other routes and validates tokens. <br>
Auth: authentication server, used for signing up and issuing tokens. <br>
Employee: employee service. <br>

# Install Instruction<br>
1.Clone the source code.<br>
2.Update the /src/main/resources/application.properties with your own DB URL/Password.<br>
3.Update the port number if necesarry(by default it is 7070). <br>
4.If you have MySQL installed, run the script hr.sql to create the tables.<br>
5.Run Application class.<br>
<br>
# Auth API
POST http://localhost:7070/auth/signup <br>

# Employee API
GET http://localhost:7070/employee/ <br>
GET http://localhost:7070/employee/1 <br>

# Recruitment API
GET http://localhost:7070/job <br>
POST http://localhost:7070/job <br>
PUT http://localhost:7070/job/1 <br>
GET http://localhost:7070/job/1 <br>
DELETE http://localhost:7070/job/1 <br>

# Job Applicants
GET http://localhost:7070/job/applicant <br>
POST http://localhost:7070/job/applicant <br>
GET http://localhost:7070/job/applicant/1 <br>
PUT http://localhost:7070/job/applicant/1 <br>
DELETE http://localhost:7070/job/applicant/1 <br>

# Job Applicants Postings
GET http://localhost:7070/job/application <br>
POST http://localhost:7070/job/application <br>
GET http://localhost:7070/job/application/applicant/1 <br>
GET http://localhost:7070/job/application/job/1 <br>
DELETE http://localhost:7070/job/application <br>

# Position API
GET http://localhost:7070/position/ <br>
GET http://localhost:7070/position/1 <br>
DELETE http://localhost:7070/position/1 <br>
POST http://localhost:7070/position/ <br>
PUT http://localhost:7070/position/1 <br>




