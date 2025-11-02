# Event-Driven Microservices Project

This project demonstrates the **Event-Driven Architecture** in a **Microservices** setup.

## Overview

The system consists of multiple microservices communicating asynchronously through **Kafka**:

- **Order Service (Producer)**:  
  Creates and publishes events/messages to a Kafka broker whenever an order is placed.

- **Stock Service (Consumer)**:  
  Listens to order events from Kafka and updates stock levels accordingly.

- **Email Service (Consumer)**:  
  Listens to order events from Kafka and sends email notifications to customers.


- **Base Domains Service**:

The **Base Domains Service** is responsible for holding the **entity classes** used across the microservices.  

It provides a centralized place for defining:

- Common domain models and entities  
- Shared data structures used by multiple services  
- Consistent validation and relationships for entities  

This helps in maintaining **reusability** and **consistency** across the microservices in the project.


This architecture helps in building **loosely coupled, scalable, and reactive systems**.
