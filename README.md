E-commerce Microservices REST API

This is a e-commerce REST API developed using Java and Spring Boot. It offers features for managing products, orders, customers and more. The API uses JSON Web Tokens (JWT) for authentication and authorization. The structure follows a microservice architecture, making it scalable and easier to manage.
Table of Contents

    Microservices
        API Gateway
        Catalog Service
        Config Service
        Order Service
        Auth Service
        Image Service
        Customer Service
        Cart Service
    Technologies Used
    Setup
    Authentication and Authorization
  

Microservices

The API is built using microservices, each service handles a specific business function.
API Gateway

Acts as the single entry point for clients, directing traffic to the right service.
Catalog Service

Manages products catalog, including details, pricing, and availability.
Config Service

Centralizes configuration for all services.
Order Service

Handles customer orders, tracking and managing them.
Auth Service

Manages authentication and authorization using JWTs.
Image Service

Deals with product images.
Customer Service

Manages customer information.
Cart Service

Handles shopping cart functionality.
Technologies Used

The API is built with:

    Spring Cloud (Config, OpenFeign, Eureka)
    JPA / Hibernate
    Springdocv2
    Java 19
    Spring Boot 3.0.2
    PostgreSQL

Setup

    Clone the repo.
    Install PostgreSQL and setup the database.
    Update application-{service}.yml in config-server with your database details.
    Start services in this order:
        Eureka Server
        Config Server
        API Gateway
        All other microservices

Authentication and Authorization

JWTs are used for secure authentication and authorization. A JWT is issued upon login and must be included in request headers.