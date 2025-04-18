# 🗺️ eureka

Microserviço responsável pela **descoberta e registro de microsserviços**. Atua como um **Service Registry** usando Spring Cloud Eureka.

---

## 📌 Objetivo

Centralizar o **registro e descoberta de microsserviços** em ambiente distribuído, permitindo balanceamento de carga e comunicação entre serviços sem configuração estática de endereços.

---

## ⚙️ Stack Tecnológica

- **Linguagem:** Java
- **Framework:** Spring Boot
- **Service Registry:** Spring Cloud Eureka

---

## 📁 Estrutura

Serviço simples com única responsabilidade: atuar como servidor de registro. Todos os micros da plataforma registram-se automaticamente no Eureka.

---

## ⚙️ Configuração Básica

### `application.yml`

```yaml
server:
  port: 8761

spring:
  application:
    name: eureka

eureka:
  client:
    register-with-eureka: false
    fetch-registry: false
