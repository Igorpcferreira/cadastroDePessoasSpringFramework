# Guia de Deploy para Projeto Spring Boot

Este guia descreve os passos necessários para realizar o deploy de um projeto que utiliza Angular no front-end e Spring
Boot com Java 17 no back-end.

## Pré-requisitos

Antes de começar, certifique-se de ter o seguinte instalado em sua máquina de desenvolvimento:

- Node.js (https://nodejs.org/)
- Java 17 JDK (https://adoptopenjdk.net/)
- Apache Maven (https://maven.apache.org/)
- PostgreSQL 15 ou superior

## Configuração do Banco de Dados

1. **Banco de Dados PostgreSQL:**
   Certifique-se de ter o PostgreSQL 15 ou superior instalado. Crie um banco de dados chamado `cadastro` com o usuário e
   senha `postgres`.

   ```sql
   CREATE DATABASE cadastro;
   CREATE USER postgres WITH ENCRYPTED PASSWORD 'postgres';
   GRANT ALL PRIVILEGES ON DATABASE cadastro TO postgres;
   ```
