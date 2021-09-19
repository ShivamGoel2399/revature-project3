
# Railway Reservation System
  <h3>Postgress Credentials</h3>
  <li>Database Name : postgres</li><br>
  <li>Username : postgres</li><br>
  <li>Password : root12345</li><br>
  <li>Schema Name : train_schema</li><br>
  
   <h3>Remote Desktop Server(MYSQL) Credentials</h3>
  <li>Database Name : Railway</li><br>
  <li>Username : root</li><br>
  <li>Password : root12345</li><br>
  <li>Schema Name : railway</li><br>
  <li>Local Host : railway.cgotxcdjntda.us-east-2.rds.amazonaws.com</li><br>
<hr>

## Spring Boot Configuration Details
``server.port=9848``
<h3>Maven Dependencies<h3>
1. spring-boot-starter-web<br>
2. spring-boot-starter-data-jpa<br>
3. spring-boot-starter-test<br>
4. jjwttoken<br>
5. Spring-Web-Secuity<br>
6. Jaxbi<br>
5. postgresql<br>
7. Java8
8. MySQL

<h3>Spring maven Plugins<h3>
1. spring-boot-maven-plugin


<hr>

## Angular Configuration Details
```server.port=4200```
```
$npm install -g @angular/cli //installing angular CLI
$ng new examfront //creating our app
cd examfront
ng serve --open //for running project on server
```
### Angular Libraries Used
1. Angular Material UI <br>
``` ng add @angular/material ```
### NPM Packages Used
``` npm install --save sweetalert2 ``` <br>
``` npm install -g @angular/cli  ``` <br>
``` npm install matsnackbar  ```

## Git commands
  - for creating a branch and shifting to it directly<br>
  $git checkout -b mybranchname<br>
  - command for shifting back to master<br>
  $git checkout main<br>
  -command for pushing the changes to branch<br>
   $git push origin branch name<br>
  -command for merging the changes made in branches to the main(assume main as master)<br>
  $git merge main<br>
  
  ## Swagger
  - link for accessing swagger<br>
  ``` http://localhost:9848/swagger-ui/ ```  
   
 # Railway Reservation System 
  The system should allow the users to reserve the train seats/sleeper for 2 routes (up/down otherwise source/destination) and in each route should allow 3 trains, in that the morning train will be a passenger train, the afternoon train will be express starts from source to destination - no stopping in the middle and the night train will be fast train with minimum stops About user/actors Admin Users End Users - reserve/cancel Detailed requirements-Functional About Trains - Capacity Trains will have 10 coaches Two types Seating- Chair Type and Sleeping type Two types coaches- Non-AC and AC Each coach will have 70 chair type and if sleeper type 50 is the capacity In each coach minimum 2 maximum 4 need to be allocated to physically challenged About Trains Morning trains will have only one AC and all seating capacity - meaning chair type Morning trains will stops in 10-15 stations in between source and destination Afternoon trains will have only one AC and all seating capacity - meaning chair type Afternoon trains will not stop in any stations in between source and destination Night trains will have only two AC and all sleeping type capacity and one Non-AC chair seating type Night trains will stop 4-6 stations in between source and destination About Travel Hours Each routes should have the start time at source and destination reach time Include the stopping points hours as well Include the travel hours from each source to each destination About Ticket Price One time ticket price will be fixed by the admin user for the route/seating type/AC/Non-AC Below Age of 5 price nil Age above 6 till 60 fixed a price Age above 60 fix a price which should have a concession of price of (6-60 age) 10% Age above 80 fix a price which should have a concession of price of (6-60 age) 20% Irrespective of age if physically challenged 30% discount from the price of (6-60) Pricing will be different for AC/Non-AC Pricing will be different from Chair Type/Sleeping Type About Admin users Users able to add a route or remove a route with train name and train number Users able to add stopping point or remove stopping point in each route, each stopping point should have a name Users able to fix the price - general price - of age 6-60 for that route About End Users - Who is used to reserve the seats for any date/route User Registration - includes name, email, phone, address with login user name & password Each login user to this application should have one identity proof like driving license/pan/aadhar Each login user can add their family or friends with name, age, gender, if physically challenged or not - maintain a list Each login user can reserve for 5-10 seats not more than that Reservation Rules 30 days ahead reservation is allowed and till 1 day prior to the start date reservation is allowed Reservation allowed to all stopping points in the middle as well Each stopping point will have 5% of total capacity of the reservations for the train For each reservation Confirmation Ticket will need to be made available in the screen with a Unique Ticket Number Tickets can be reserved for only 1 user or many users meaning the Unique Ticket Number may be for 1 user or multiple users Confirmed Ticket should be printable form kind of Date of travel, source, destination, time of start, reach time, number of stop overs - only count, name of the traverller(s), traver hours, reservation date/time Ticket user should have identity proof in our End User data Cancellation Rules From the train start date 7 days before if cancelled Refund 80% From the train start date 4 days before if cancelled Refund 40% From the train start date 2 day before if cancelled Refund 20% On the day of train starts if the cancellation is done only 5% refund Cancellation number will be generated - unique number - and should be allowed to print Cancellation status should immediately reflect with respect to date/train, so that it should allow for other users to reserve/book the ticket Cancellation Confirmation should be printable from with all the reservation information plus date of cancellation, reason for cancellation (need to capture this - it can be empty also) with the refund amount based on the cancellation rules Reports At any point of time Admin users should be able to generate for any date/time/route the following reports Travel Report Reservation Report Cancellation Report End users who reserve should able to view last 3 months confirmed tickets/cancelled tickets/reserved tickets Technical Design/Architecture need to be derived for the following - Before start of the Development Database Schema/Table Design Presentation Layer - meaning UI Screens - for all the requirements stated above - none should be modified in the backend Business/service Layer - based on the requirements create the functionality and have them in the middle layer Database Layer - to access the DB data Validations All front end validations need to be done All business validations need to be properly reflected to the users with proper messages to change the data if needed All database validations need to be properly reflected to the users with proper messages to change the data if needed Logs To be maintained like which user using which functionality App logs for each layer need to be differentiated Exclusions or Implicit Assumptions Payment gateway or payments are assumed that all goes well without invoking Implicit - Testing For all the development implicit usage of Unit testing code should be done Devops - Tools should be used Github, Maven, Jenkins must be used to build and deploy Notifications (optional) Sent through Emails and SMS

# Roles / Responsibilities
Used Agile methodalogy for the project.
Worked on Spring Tool Suite and Visual Studio Code.
Utilized GitHub to manage the source code.
Developed Web pages using Angular 10.
Worked on Spring Data JPA  for SQL operations.
Leveraged server side technologies such as Java, Rest, Spring Boot and Spring Data to handle requests and responses.
Utilized DevOps and Jenkins for publish the project in the server.
Used JUnit for testing the business layer as well as other functionalities.
Used Jasmine And Karma for testing the service layer for front-end technologies.
Deployed AWS S3 bucket  and AWS EC2 to have a fully functioning remote application.
Used Monolithic Service for implementing the code.
# Environment / Technologies
Angular 4, Spring Boot, Jenkins, AWS EC2, Docker, Log4J, JUnit4, Agile-Scrum
