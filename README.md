# Deshi Gadgets
This is an E-Commerce website built for the online sale of electronic products.
## Course Details:
- **Course Name**: Software Engineering Lab
- **Course Code**: 328
- **Course Instructor**: Labiba Farah, Lecturer, BUBT
## Our Top Contributors 
<p align="center">
  <a href="https://github.com/0mehedihasan/Software-Development-3/graphs/contributors">
    <img src="https://contrib.rocks/image?repo=0mehedihasan/Software-Development-3" max-width="1000" columns="5" anon="1" />
  </a>
</p>

## Our Team
<div style="display: flex; align-items: center; margin: 10px;">
  <!-- Contributor 1 Image -->
  <a href="https://github.com/0mehedihasan">
    <img src="https://avatars.githubusercontent.com/0mehedihasan" width="100" height="100" alt="Md Mehedi Hasan" />
    <div style="margin-left: 10px;">
    <a href="https://github.com/0mehedihasan">Md Mehedi Hasan</a><br />
    ID: 21225103334
    </div></a>
</div>

---
## About

This project allows users to visit the website, register, and log in. Once logged in, users can browse the available products, search and filter items by category, and add them to their shopping cart. Users can add multiple items to the cart and adjust the quantity of each item. After updating the cart, users can proceed to checkout and enter their payment details. Once the payment is successful, the order is placed, and users can view their order details along with the shipping status.

The admin has an important role in this system. The admin can add new products to the store, update existing items, remove products, and manage the inventory. The admin can also view all orders and update their status (e.g., mark orders as shipped or delivered).

A **key feature** of this project is the email notifications for users. When a user registers, they will receive a confirmation email. Additionally, whenever a user places an order or when the order is shipped, they will receive an email with the details. If a product goes out of stock and a user tries to purchase it, they will be notified by email once the product is available again.

- **Note:** The payment page is for demonstration purposes only and is not connected to a real payment gateway. For now, any credit card details can be used to place a demo order.
---
## Project Overview
### Key Features
### Notification Emails
Users will receive notification emails in the following scenarios:
- Upon registration on the website.
- After successfully placing an order.
- When a previously out-of-stock item becomes available again.
- When an order is shipped or delivered.
## Technologies Utilized
### Front-End:
- HTML
- CSS
- JavaScript
- Bootstrap
### Back-End:
- Java (JDK 21) [JDK8+ MUST]
- JDBC
- Servlets
- JSP
### Database:
- MySQL
### ER Diagram
<img width="589" alt="image" src="https://github.com/0mehedihasan/Software-Development-3/blob/main/Documentations/ER.jpg">

### UML DIAGRAM
<img width="589" alt="image" src="https://github.com/0mehedihasan/Software-Development-3/blob/main/Documentations/ER.jpg">

### ================ Software And Tools Required ================
- : Git [https://git-scm.com/downloads]
- : Java JDK 8+ [https://www.oracle.com/bd/java/technologies/downloads/#jdk23-windows]
- : Eclipse EE (Enterprise Edition) [https://www.eclipse.org/downloads/]
- : Apache Maven [https://maven.apache.org/download.cgi]
- : Tomcat v8.0+ [https://tomcat.apache.org/download-90.cgi]
- : MySQL Server [https://dev.mysql.com/downloads/workbench/]
- : MySQL Workbench [https://dev.mysql.com/downloads/workbench/]
## ================ Project Setup Instructions ================
### Dummy Database Initialization
**Step 1:** Open MySQL Command Prompt or MySQL Workbench.
**Step 2:** Log in to the MySQL administrator user:
```mysql
mysql -u <username> -p
```
(Enter the password if prompted)
**Step 3:** Execute the MySQL query from the following file:
- Run the SQL query from this file: [databases/mysql_query.sql](./databases/mysql_query.sql)
### Generating Gmail App Password for Mailing Functionalities
- **Step 1:** Create a Gmail account or log in to an existing account in any browser.
- **Step 2:** Navigate to [Google Account Security](https://myaccount.google.com/security) and ensure that 2-step verification is enabled. Enable it if it is not already enabled.
- **Step 3:** Proceed to [Google App Passwords](https://myaccount.google.com/apppasswords) and enter your password if prompted.
- **Step 4:** In the "Select an App" section, select "Other (custom name)" and enter "Ellison Electronics" then generate the password.
- **Step 5:** A 16-digit app password will be generated. Copy and save this password for future configurations.
- **Step 6:** Completed. Continue with importing the project. [Do not share the generated password with anyone.]
### Importing and Running the Project Through Eclipse EE
- **Step 1:** Open Eclipse Enterprise Edition. [Install it if it is not already installed.]
- **Step 2:** Navigate to File > Import > Git > Projects from Git > Clone URI > Paste the repository URL: 
```https://github.com/0mehedihasan/Software-Development-3.git```
Select the master branch > Next > Next > Finish.
- **Step 3:** Navigate to `Java Resources > src > application.properties` and update the values as follows:
    - a) Update the values for `db.username` and `db.password` according to your MySQL credentials.
    - b) Update the values for `mailer.email` and `mailer.password` with the email and app password generated earlier. [Note: The actual Gmail password will not work.]
- **Step 4:** Right-click on the project > Run As > Maven Build > In the goals field, enter "clean install" > Apply > Run.
- **Step 5:** Right-click on the project > Build Path > Configure Build Path > Libraries > Remove and update any libraries if a red mark exists > Finish.
- **Step 6:** Right-click on the project > Maven > Update Project > Select "Force Update" > Apply > Close.
- **Step 7:** Tomcat Configurations:
    - If Tomcat Server is not configured in Eclipse:
      - Right-click on the project > Run As > Run on Server > Manually define a new server > Select server type > Select Tomcat v8.0+ > (Select Tomcat v8.0+ installation location if prompted) > Next > Add the current project > Finish.
    - If Tomcat Server is already configured in Eclipse:
      - Right-click on the project > Run As > Run on Server > Select Tomcat version > Next > Add the project > Finish.
      - Alternatively, go to the server tab, select the Tomcat server, and use the debug or run button to start the previously run project.
- **Step 8:** Verify the site is running at [http://localhost:8080/Deshi-Gadgets/](http://localhost:8080/Deshi-Gadgets/).
- **Step 9:** To change the port if encountering an error like 'port already in use', open the server tab > Double-click on Tomcat Server > Ports > Change the port number for HTTP/1.1 to 8083 > Close and save.     - Start the server and access the project at [http://localhost:8083/Deshi-Gadgets/](http://localhost:8083/Deshi-Gadgets/).
- **Step 10:** The default username and password for the admin is "admin@gmail.com" and "admin".
- **Step 11:** The default username and password for the user is "guest@gmail.com" and "guest".
#### "Suggestions and project improvement ideas are welcomed!"
<bold>Thanks a lot,</bold><br/>
Project Leader<br/>
<b>Md Mehedi Hasan</b>


