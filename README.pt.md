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
