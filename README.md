USAGE COMMANDS
--------------

> Please be aware that following tools should be installed in advance on your computer: **Java**, **Maven** and **Git**. 

> Please **clone/download** project, open **project's main folder** in your favorite **command line tool** and then **proceed with steps below**. 

Usage steps:
1. In a command line tool start application with `mvn clean package wildfly:run`
1. In a http browser (e.g. Chrome) visit `http://localhost:8080/rest/api/hello`
   * Expected JSON **{"message": "Hello World!"}**
1. Clean up environment 
     * In a command line tool stop application with `ctrl + C`


USAGE IMAGES
------------

![My Image](readme-images/image-01.png)


DESCRIPTION
-----------

##### Goal
The goal of this project is to present how to insert some **initial data** into **REST API Java** application with **H2 embedded database** using **Java EE 10** framework. This application returns JSON with the key "message" and the value **Hello World!** as the result of GET HTTP method. 

Application is deployed on **Wildfly** server.

##### Flow
The following flow takes place in this project:
1. User via any browser sends request to application for a content.
1. Application saves message "Hello World!" into H2 database.
1. Application reads message from H2 database.
1. Application returns response with JSON containing message "Hello World"!. This response is presented to User via browser.

##### Launch
To launch this application please make sure that the **Preconditions** are met and then follow instructions from **Usage** section.

##### Technologies
This project uses following technologies:
* **Java EE 10** framework
* **H2** embedded database


PRECONDITIONS
-------------

##### Preconditions - Tools
* Installed **Operating System** (tested on Windows 10)
* Installed **Java** (tested on version 21.0.2). Tool details: `https://docs.google.com/document/d/119VYxF8JIZIUSk7JjwEPNX1RVjHBGbXHBKuK_1ytJg4/edit?usp=sharing`
* Installed **Maven** (tested on version 3.9.6). Tool details: `https://docs.google.com/document/d/1cfIMcqkWlobUfVfTLQp7ixqEcOtoTR8X6OGo3cU4maw/edit?usp=sharing`
* Installed **Git** (tested on version 2.43.0.windows.2). Tool details: `https://docs.google.com/document/d/1Iyxy5DYfsrEZK5fxZJnYy5a1saARxd5LyMEscJKSHn0/edit?usp=sharing`


##### Preconditions - Actions
* **Download** source code using Git 
* Open any **Command Line** (for instance "Windonw PowerShell" on Windows OS) tool on **project's folder**.


ADDITIONAL INFO
---------------

Used starter page: `https://start.jakarta.ee/`