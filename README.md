# service-prov-db
PT-BR

# Banco de dados para prestação de serviços

## 📌 Resumo

O projeto apresenta dois arquivos de extensão .txt e um .mwb, que representam as inserções, consultas e modelagem para um banco de dados relacional, como o mySQL, voltado à uma aplicação para prestação de serviços.

## 🎯 Objetivo
O Objetivo deste trabalho foi testar os conhecimentos sobre bancos de dados, relacionamento entre entidades e aplicações para sistemas reais do mercado de trabalho. 
Utilizando esse projeto, é possível criar um sistema de banco de dados completo que busca **facilitar o gerenciamento** de serviços, funcionários, clientes e agendamentos, encaixando-se para empresas de qualquer ramo.

## 🛠️ Ferramenta utilizada

* mySQL Workbench para Diagrama Entidade-Relacionamento (DER)

## ☑️ Escopo do projeto

Esse sistema cobre as seguintes necessidades:
* Cadastro de clientes e funcionários, utilizando nome, email e data de nascimento, além de um login e senha específico para que os funcionários agendem serviços;
* Cadastro de endereço e telefone atrelado à conta, facilitando a localização e comunicação entre as partes na prestação de serviços;
* Cada funcionário pode agendar vários serviços e cadastrar novos clientes;
* Gerentes podem cadastrar novos funcionários e clientes e monitorar o andamento de serviços;
* Controle de status do agendamento (concluído, em andamento, cancelado).

## 🏢 Estrutura 

### Entidades

* Clientes, Endereço, Usuários, Telefones, Agendamento, Serviços.

### Relacionamentos

* Clientes <-> Endereço **(N:1)**
* Clientes <-> Agendamento **(1:N)**
* Clientes <-> Telefones **(1:N)**
* Usuários <-> Endereço **(N:1)**
* Usuários <-> Agendamento **(1:N)**
* Usuários <-> Telefones **(1:N)**
* Serviços <-> Agendamento **(1:N)**

## ▶️ Como utilizar
1. Para visualizar o diagrama:
    * Clone este repositório 
    * Abra o mySQL Workbench -> File -> Open Model -> Selecione o arquivo "modelagem-bd.mwb"
   
2. Para criar o banco de dados por meio de código:
    * Clone este repositório
    * Abra o mySQL Workbench -> File -> New Query Tab
    * Copie e cole o arquivo "implementacao-bd", executando primeiramente "CREATE DATABASE PROGRAMASERV;" 
    * Teste os Selects colando o arquivo "consultas-bd"

Nota: Caso tenha problemas com mySQL Workbench, assista à [esse vídeo](https://www.youtube.com/watch?v=oi3UHWXLxLs)

### Requisitos Mínimos

* mySQL Workbench e Server, a partir da versão 8.x.x

## 🧠 Conceitos aplicados

* Normalização de banco de dados
* Construção de diagrama Entidade-Relacionamento
* Comandos básicos de SQL (CREATE TABLE, INSERT INTO, ...)
* Lógica de seleção de informações usando o comando SELECT

## 🚧 Limitações e possíveis melhorias

* Criar ID para Agendamento, de forma que um funcionário pudesse criar outro agendamento com o mesmo serviço para o mesmo cliente

## 👥 Autores

Este projeto foi criado em conjunto com GabrielHFPirolo como projeto final para a matéria de Banco de Dados na Universidade Tecnológica Federal do Paraná (UTFPR).

---
EN-US

# Database for provision of services

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
