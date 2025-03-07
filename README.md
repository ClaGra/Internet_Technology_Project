# Internet_Technology_Project

[![License](https://img.shields.io/:license-apache-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0.html)

#### Contents:
- [Analysis](#analysis)
  - [Scenario](#scenario)
  - [User Stories](#user-stories)
  - [Use Case](#use-case)
- [Design](#design)
  - [Prototype Design](#prototype-design)
  - [Domain Design](#domain-design)
  - [Business Logic](#business-logic)
- [Implementation](#implementation)
  - [Backend Technology](#backend-technology)
  - [Frontend Technology](#frontend-technology)
- [Project Management](#project-management)
  - [Roles](#roles)
  - [Milestones](#milestones)

## Analysis
> 🚧: You can reuse the analysis (you made) from other projects (e.g., requirement engineering), but it must be submitted according to the following template. 



### Scenario

The Brauverein Full is a brewing association based in Full. It was founded in June 2018 by five people who aimed to produce beer for themselves, friends, and families. The reason for the foundation of an association was that the beer of a private individual is legally not allowed to leave the property where it is brewed, which complicated the sharing with other people. Through the small size of the village, which has less than 1000 inhabitants, the word of a local brewery spread, and the association gained in popularity and customers.
The Brauverein Full has been managing its stock and sales using a self-made Excel sheet that has become increasingly time-consuming, error-prone, and difficult to manage as the association has grown in size and complexity. The association has decided to switch to a webbased application to streamline and automate its inventory management, sales tracking, and reporting processes. The new application will enable the association to track its inventory levels in real-time, automatically generate sales reports, and provide better visibility into its sales trends and stock turnover rates.
This project aims to improve the efficiency and accuracy of the Brauverein Full’s inventory management and sales tracking, reducing administrative overhead and enabling the association to make data-driven decisions to optimize their operations and meet the needs of their members and customers more effectively. 

The Excel sheet used for the stock and sales management was created by the head of administration of the Brauverein Full. Its purpose is to give the association members a better overview of the inventory levels and decrease the effort at the end of the year to create the report for the customs administration overseeing the taxation of sold beer.
Since the Excel sheet includes many complex formulas, the remainder of the association will not use the tool out of fear of deleting or breaking something. As a solution to this problem, the head of administration currently manages to fill the Excel sheet herself. The association members transmit the information about withdrawals from the inventory via a specific WhatsApp chat. They are then transferred into the Excel sheet by the head of administration, which leads to a double track and a high administrative effort for multiple members. Furthermore, since only one out of five people opened the Excel sheet, it lost its purpose.
The Excel sheet does not give any insights about specific customers or their orders since the administrative workload is tried to be held as small as possible for the head of administration. With the implementation of a web-based application, this information could be easily added and would provide better visibility into the sales trends.

### User Stories

#### User Stories General
1. As an Admin, I want to have a Web app to use on different mobile devices and desktop computers.
2. As an Admin, I want to see a consistent visual appearance to navigate easily, and it should look consistent.
3. As an Admin, I want to use list views to explore and read my business data.
4. As an Admin, I want to use edit and create views to maintain my business data.
5. As an Admin, I want to log-in so that I can authenticate myself.
6. As a User, I want to use list views so that I can access public pages.
7. (Optional) As a User, I want to authenticate myself so that I can read my personal and confidential data.

#### User Stories Administration
1. As a Head of Administration, I want to add user accounts so that I can grant access to new users.
2. As a User, I want to edit my user account so that I can update user information when necessary.
3. As a Head of Administration, I want to delete user accounts so that I can remove access when needed.
4. As a User, I want to log in so that I can access the system securely.
5. As a User, I want to log out so that I can securely end my session.

#### User Stories Inventory
1. As a User, I want to add inventory so that I can keep track of new stock.
2. As a User, I want to edit inventory so that I can update inventory details.
3. As a Head of Administration, I want to delete inventory so that I can remove outdated or incorrect stock entries.

#### User Stories Brewing & Bottling
1. As a User, I want to add a brewing protocol so that I can document new brewing processes.
2. As a User, I want to edit brewing protocols so that I can update brewing process details.
3. As a Head of Administration, I want to delete brewing protocols so that I can remove outdated or incorrect processes.
4. As a User, I want to add bottling information so that I can record packaging details.
5. As a User, I want to edit bottling records so that I can update packaging information.
6. As a Head of Administration, I want to delete bottling records so that I can remove incorrect or outdated packaging data.
7. As a User, I want to view brewing protocols so that I can understand the brewing processes.
8. As a User, I want to query brewing and bottling information so that I can get insights into production data.

### Use Case

#### Use Case 100 Administration
![image](https://github.com/user-attachments/assets/b96bf3f3-9f86-48a2-ae54-d099608180a2)
 
- UC-101 [Add User Account]: The system shall allow the head of administration to create a new user account
- UC-102 [Edit User Account]: The system shall allow the user to edit their account
- UC-103 [Delete User Account]: The system shall allow the head of administration to delete a user account
- UC-104 [User Login]: The system shall allow the user to log in
- UC-105 [User Logout]: The system shall allow the user to log out

#### Use Case 200 Inventory
![image](https://github.com/user-attachments/assets/6575f187-2fba-4dbe-9645-527392fbd26a)

- UC-201 [Add Inventory]: The system shall allow the user to add inventory
- UC-202 [Edit Inventory]: The system shall allow the user to edit previously entered
inventory
- UC-203 [Delete Inventory]: The system shall allow the head of administration to delete previously recorded inventory

#### Use Case 300 Brewing & Bottling
![image](https://github.com/user-attachments/assets/7db469ff-2f65-480d-a896-c7aaa941a372)

- UC-301 [Add Brewing Protocol]: The system shall allow the user to create a brewing protocol  
- UC-302 [Edit Brewing Protocol]: The system shall allow the user to edit an existing brewing protocol 
- UC-303 [Delete Brewing Protocol]: The system shall allow the head of administration to delete an existing brewing protocol  
- UC-304 [Add Bottling]: The system shall allow the user to register a new bottling process
- UC-305 [ Edit Bottling]: The system shall allow the user to edit an existing bottling process
- UC-306 [Delete Bottling]: The system shall allow the user to delete an existing bottling process
- UC-307 [Viewing Brewing Bottling]: The system shall allow the user to view the brewing protocol in its current state 
- UC-308 [Query Brewing & Bottling]: The system shall allow the user to query a report of the brewing and bottling for taxes


## Design
> 🚧: Keep in mind the Corporate Identity (CI); you shall decide appropriately the color schema, graphics, typography, layout, User Experience (UX), and so on.

### Wireframe
> 🚧: It is suggested to start with a wireframe. The wireframe focuses on the website structure (Sitemap planning), sketching the pages using Wireframe components (e.g., header, menu, footer) and UX. You can create a wireframe already with draw.io or similar tools. 

Starting from the home page, we can visit different pages. Available public pages are visible in the menu...

![image](https://github.com/user-attachments/assets/5f947bef-3f63-4c60-864f-1b3c91eb2eb6)
![image](https://github.com/user-attachments/assets/86b6520a-1ff1-4cf2-bea6-f1fda049e8a2)
![image](https://github.com/user-attachments/assets/c988754d-f137-40d6-a047-8f7996d2cb4a)
![image](https://github.com/user-attachments/assets/cbbfc199-577b-41fc-8995-ce6b6cebb6f4)
![image](https://github.com/user-attachments/assets/249d8812-b5ad-49dc-a767-ef0296f94265)
![image](https://github.com/user-attachments/assets/86aeff53-199b-4ce0-b069-0a6a6e3bf01d)
![image](https://github.com/user-attachments/assets/83cd7590-0cd3-42e4-977f-8b152d59c93e)



### Prototype
> 🚧: A prototype can be designed using placeholder text/figures in Budibase. You don't need to connect the front-end to back-end in the early stages of the project development.

### Domain Design
> 🚧: Provide a picture and describe your domain model; you may use Entity-Relationship Model or UML class diagram. Both can be created in Visual Paradigm - we have an academic license for it.

The `ch.fhnw.pizza.data.domain` package contains the following domain objects / entities including getters and setters:

![](images/domain-model.png)

### Business Logic 
> 🚧: Describe the business logic for **at least one business service** in detail. If available, show the expected path and HTPP method. The remaining documentation of APIs shall be made available in the swagger endpoint. The default Swagger UI page is available at /swagger-ui.html.

Based on the UC-4, there will be two offers and a standard offer. Given a location, a message is shown accordingly:

- If the location is "Basel", the message is "10% off on all large pizzas!!!"
- If the location is "Brugg", the message is "two for the price of One on all small pizzas!!!"
- Otherwise, the message is "No special offer".

**Path**: [`/api/menu/?location="Basel"`] 

**Param**: `value="location"` Admitted value: "Basel","Brugg".

**Method:** `GET`

## Implementation
> 🚧: Briefly describe your technology stack, which apps were used and for what.

### Backend Technology
> 🚧: It is suggested to clone this repository, but you are free to start from fresh with a Spring Initializr. If so, describe if there are any changes to the PizzaRP e.g., different dependencies, versions & etc... Please, also describe how your database is set up. If you want a persistent or in-memory H2 database check [link](https://github.com/FHNW-INT/Pizzeria_Reference_Project/blob/main/pizza/src/main/resources/application.properties). If you have placeholder data to initialize at the app, you may use a variation of the method **initPlaceholderData()** available at [link](https://github.com/FHNW-INT/Pizzeria_Reference_Project/blob/main/pizza/src/main/java/ch/fhnw/pizza/PizzaApplication.java).

This Web application is relying on [Spring Boot](https://projects.spring.io/spring-boot) and the following dependencies:

- [Spring Boot](https://projects.spring.io/spring-boot)
- [Spring Data](https://projects.spring.io/spring-data)
- [Java Persistence API (JPA)](http://www.oracle.com/technetwork/java/javaee/tech/persistence-jsp-140049.html)
- [H2 Database Engine](https://www.h2database.com)

To bootstrap the application, the [Spring Initializr](https://start.spring.io/) has been used.

Then, the following further dependencies have been added to the project `pom.xml`:

- DB:
```XML
<dependency>
			<groupId>com.h2database</groupId>
			<artifactId>h2</artifactId>
			<scope>runtime</scope>
</dependency>
```

- SWAGGER:
```XML
   <dependency>
      <groupId>org.springdoc</groupId>
      <artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
      <version>2.3.0</version>
   </dependency>
```

### Frontend Technology
> 🚧: Describe your views and what APIs is used on which view. If you don't have access to the Internet Technology class Budibase environment(https://inttech.budibase.app/), please write to Devid on MS teams.

This Web application was developed using Budibase and it is available for preview at https://inttech.budibase.app/app/pizzeria. 

## Execution
> 🚧: Please describe how to execute your app and what configurations must be changed to run it. 

**The codespace URL of this Repo is subject to change.** Therefore, the Budibase PizzaRP webapp is not going to show any data in the view, when the URL is not updated or the codespace is offline. Follow these steps to start the webservice and reconnect the webapp to the new webservice url. 

> 🚧: This is a shortened description for example purposes. A complete tutorial will be provided in a dedicated lecture.

1. Clone PizzaRP in a new repository.
2. Start your codespace (see video guide at: [link](https://www.youtube.com/watch?v=_W9B7qc9lVc&ab_channel=GitHub))
3. Run the PizzaRP main available at PizzaApplication.java on your own codespace.
4. Set your app with a public port, see the guide at [link](https://docs.github.com/en/codespaces/developing-in-a-codespace/forwarding-ports-in-your-codespace).
5. Create an own Budibase app, you can export/import the existing Pizzeria app. Guide available at [link](https://docs.budibase.com/docs/export-and-import-apps).
6. Update the pizzeria URL in the datasource and publish your app.

### Deployment to a PaaS
> 🚧: Deployment to PaaS is optional but recommended as it will make your application (backend) accessible without server restart and through a unique, constantly available link.  

Alternatively, you can deploy your application to a free PaaS like [Render](https://dashboard.render.com/register).
1. Refer to the Dockerfile inside the application root (FHNW-INT/Pizzeria_Reference_Project/pizza).
2. Adapt line 13 to the name of your jar file. The jar name should be derived from the details in the pom.xml as follows:<br>
`{artifactId}-{version}.jar` 
2. Login to Render using your GitHub credentials.
3. Create a new Web Service and choose Build and deploy from a Git repository.
4. Enter the link to your (public) GitHub repository and click Continue.
5. Enter the Root Directory (name of the folder where pom.xml resides).
6. Choose the Instance Type as Free/Hobby. All other details are default.
7. Click on Create Web Service. Your app will undergo automatic build and deployment. Monitor the logs to view the progress or error messages. The entire process of Build+Deploy might take several minutes.
8. After successful deployment, you can access your backend using the generated unique URL (visible on top left under the name of your web service).
9. This unique URL will remain unchanged as long as your web service is deployed on Render. You can now integrate it in Budibase to make API calls to your custom endpoints.

## Project Management
> 🚧: Include all the participants and briefly describe each of their **individual** contribution and/or roles. Screenshots/descriptions of your Kanban board or similar project management tools are welcome.

### Roles
- Back-end developer: 
- Front-end developer: 

### Milestones
1. **Analysis**: Scenario ideation, use case analysis and user story writing.
2. **Prototype Design**: Creation of wireframe and prototype.
3. **Domain Design**: Definition of domain model.
4. **Business Logic and API Design**: Definition of business logic and API.
5. **Data and API Implementation**: Implementation of data access and business logic layers, and API.
6. **Security and Frontend Implementation**: Integration of security framework and frontend realisation.
7. (optional) **Deployment**: Deployment of Web application on cloud infrastructure.


#### Maintainer
- Claudia Graf
- Tuangporn Siwaboon
- Yannik Stöckli
- Soheyla Tofighi 

#### License
- [Apache License, Version 2.0](blob/master/LICENSE)
