# Database for provision of services

🌎 [Versão em português](/README.pt.md)

## 📌 Overview

The project presents two .txt files and one .mwb file, representing inserts, queries, and modeling for a relational database, such as MySQL, focused on a service provision application.

## 🎯 Objective
The objective of this project was to test my knowledge of databases, data relationships between entities and real-world application of technologies. Utilizing this project, it is possible to create a complete database system that aims to **facilitate the management** of services, employees, clients, and scheduling, fitting well for any type of company. 

## 🛠️ Tools used

* MySQL Workbench for Entity-Relationship Diagram (ERD)

## ☑️ Project scope

This system covers the following necessities:
* Client and employee registration, utilizing name, email and date of birth, besides a specific login and password for employees to create service scheduling;
* Address and phone number registered to an account, facilitating localization and communication between parties in the service provision.
* Each employee can schedule multiple services and register new clients;
* Managers can register new employees and control service status;
* Scheduling status control (concluded, ongoing, cancelled).

## 🏢 Structure 

### Entities

* Clients, Addresses, Users, Phone Numbers, Scheduling, Services.

### Relationships

* Clients <-> Addresses **(N:1)**
* Clients <-> Scheduling **(1:N)**
* Clients <-> Phone Numbers **(1:N)**
* Users <-> Addresses **(N:1)**
* Users <-> Scheduling **(1:N)**
* Users <-> Phone Numbers **(1:N)**
* Services <-> Scheduling **(1:N)**

## ▶️ How to use
1. To visualize the diagram:
    * Clone this repository 
    * Open MySQL Workbench -> File -> Open Model -> Select file "modelagem-bd.mwb"

   
2. To create the database through script:
    * Clone this repository 
    * Open MySQL Workbench -> File -> New Query Tab
    * Copy and paste file "implementacao-bd", executing first "CREATE DATABASE PROGRAMASERV;"
    * Test SELECT commands by pasting file "consultas-bd" 

Note: If you have any problems with mySQL Workbench, watch [this video](https://www.youtube.com/watch?v=u96rVINbAUI)

### Minimal requirements

* mySQL Workbench and Server, version 8.x.x

## 🧠 Concepts used

* Database normalization
* Entity-Relationship Diagram creation
* Basic SQL commands (CREATE TABLE, INSERT INTO, ...)
* Data selection logic using SELECT command

## 🚧 Limitations and possible improvements

* Create ID for Scheduling, allowing an employee to create another scheduling for the same service and client.

## 👥 Authors

This project was created in collaboration with GabrielHFPirolo as a final exam for the Database class at Universidade Tecnológica Federal do Paraná (UTFPR).
