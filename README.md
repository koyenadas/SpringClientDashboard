# SpringClientDashboard
Spring MVC web application for managing clients inventory.


## Description
The application allows users to list and manage client inventory (add new ones, update existing and delete, etc.).

In the Client Dashboard there are three types of users:

1. Employee - they can register themselves and view and search exisiting client list.
2. Manager - limited number of users who can add new clients and search for existing clients. 
3. Admin - person, who can add, edit and delete clients.

## Tools & Frameworks
The application is built using Spring MVC, Spring Security, Hibernate and Maven build tool.

#### Database & configuration

- MySQL
- Tomcat
- Git
- Maven

#### Backend technologies

- Java
- Spring MVC, Spring AOP, Spring Security
- Hibernate ORM
- Hibernate Validator

#### Frontend technologies

- HTML, CSS, JavaScript
- JSP, JSTL
- Bootstrap 4

## How to run it?
Prerequisites: Eclipse IDE, Tomcat, MySQL Community Edition

1. Clone this git repository
`$ git clone https://github.com/koyenadas/SpringClientDashboard`

2. Open MySQL Workbench and type following SQL scripts:
	```mysql CREATE DATABASE  IF NOT EXISTS `web_customer_tracker`;
USE `web_customer_tracker`;

DROP TABLE IF EXISTS `customer`;

CREATE TABLE `customer` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `first_name` varchar(45) DEFAULT NULL,
  `last_name` varchar(45) DEFAULT NULL,
  `email` varchar(45) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=6 DEFAULT CHARSET=latin1;

LOCK TABLES `customer` WRITE;

INSERT INTO `customer` VALUES 
	(1,'Arya','Stark','arya@winterfell.com'),
	(2,'Cersei','Lannister','cersei@casterlyrock.com'),
	(3,'Jim','Moriarty','moriarty@rememberme.com');

UNLOCK TABLES;

```

3. Right click project name -> Run on server

4. The application will avaialble under URL http://localhost:8080/dashboard

