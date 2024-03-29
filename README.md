<strong> **DO NOT DISTRIBUTE OR PUBLICLY POST SOLUTIONS TO THESE LABS. MAKE ALL FORKS OF THIS REPOSITORY WITH SOLUTION CODE PRIVATE. PLEASE REFER TO THE STUDENT CODE OF CONDUCT AND ETHICAL EXPECTATIONS FOR COLLEGE OF INFORMATION TECHNOLOGY STUDENTS FOR SPECIFICS. ** </strong>
# WESTERN GOVERNOR UNIVERSITY 
## D288 – BACK-END PROGRAMMING
Welcome to Back-End Programming! This is an opportunity for students to develop object-oriented applications that can be integrated with relational databases, write code for object-oriented applications using Spring framework, and implements design patterns for object-oriented applications. 
FOR SPECIFIC TASK INSTRUCTIONS AND REQUIREMENTS FOR THIS ASSESSMENT, PLEASE REFER TO THE COURSE PAGE.
## BASIC INSTRUCTIONS
For this project, you will be building your project using IntelliJ IDEA (Ultimate Edition) in a WGU-provided lab environment. You will be working with an existing MySQL database and Angular front-end, which are supplied for you in the lab environment. You will share this project to a private external GitLab repository and backup regularly. If you wish to work on it on your local machine, you will also need to download the Angular front-end application and create your own MySQL database. Use the links on your course page to install the integrated development environments (IDE), MySQL WorkBench, and IntelliJ IDEA, and pull the project from the lab environment.  


Part C:
Created six new packages to create new files in
Copied RestDataConfig into config package
Copied application.properties into the file

Part D:
Cart.java: lines 15-52 used UML diagram to map columns to database
CartItem.java: lines 15-52 used UML diagram to map columns to database and used Enum annotation
Country.java: lines 12-34 used UML diagram to map columns to database
Customer.java: lines 13-51 used UML diagram to map columns to database
Division.java: lines 12-38 used UML diagram to map columns to database
Excursion.java: lines 13-42 used UML diagram to map columns to database
StatusType.java: lines 2-3 stores entity from annotation in cart.java
Vacation.java: lines 13-44 used UML diagram to map columns to database
RestDataConfiguration.java: line 3 changed import to entity file location

Part E:
CartItemRepository: lines 7-8, created interface that extends the respective jpa repo
CartRepository: lines 7-8, created interface that extends the respective jpa repo
CountryRepository: lines 7-8, created interface that extends the respective jpa repo
CustomerRepository: lines 7-8, created interface that extends the respective jpa repo
DivisionRepository: lines 7-8, created interface that extends the respective jpa repo
ExcursionRepository: lines 7-8, created interface that extends the respective jpa repo
VacationRepository: lines 7-8, created interface that extends the respective jpa repo

Part F:
Created four new java classes under the services package
Purchase.java: lines 10-14, created Purchase class that will handle purchasing 
PurchaseResponse.java: lines 5-7, created a PurchaseResponse class for tracking number that cannot be changed once it is made
CheckoutService.java: lines 3-4, created a checkout service class that will return purchase response class when purchased
CheckoutImpl: lines 19-46 implemented code to retrieve order, generate a tracking number, populate items and create a unique UUID
Customer.java: lines 53-59, created conditions to add items to order
Cart.java: lines 54-60, created conditions to add items to order

Part G:
Customer.java: lines 23-35, added validation to fields that require inputs from customer

Part H:
Created a new java class under controller package
CheckoutController.java: lines 8-20, created code using post mapping to for placing orders

Part I:
BootStrapData.java: lines 9-59, created 5 new customers to the database and saving them
Customer.java: lines 62-70, created customer constructor and initialized variables needing inputs

Additional fixes:
Cart.java: line 43, added cascading due to cart item not populating in sql
Fix to populate excursion_cartitem in sql
Excursion.java: lines 43-44, mapped many-many relationship differently which was taken from CartItem.java and changing variables as needed
Cartitem.java: lines 26-30, originally in excursion.java, added to this file and changed accordingly to fit in
