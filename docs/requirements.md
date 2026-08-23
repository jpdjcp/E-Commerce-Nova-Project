# Requirements Document

## 1. Introduction

### 1.1 Purpose

This document defines the initial requirements for the Nova E-Commerce system. It provides a common reference for the development team and establishes the functional and non-functional needs of the system.

The document is intended to evolve throughout the project as requirements are elicited, refined, classified, prioritized, and specified.

### 1.2 Scope

Nova E-Commerce is a web-based e-commerce application that allows customers to browse products, manage a shopping cart, place orders, and make payments.

The system also provides administrative capabilities for managing products and customer information.

This document focuses on the requirements of the system and does not prescribe a specific frontend implementation.

### 1.3 Goals

#### 1.3.1 Document Goals

The goals of this document are to:

- Establish a shared understanding of the system requirements.
- Provide a reference for the development team.
- Support requirements analysis, prioritization, and specification.
- Provide traceability between user requirements and system requirements.
- Evolve the requirements as the product is developed iteratively.

#### 1.3.2 System Goals

The system aims to provide:

- A simple and accessible e-commerce experience for customers.
- Product and customer management capabilities for authorized users.
- A reliable shopping cart and ordering process.
- Secure handling of sensitive information.
- An architecture that supports incremental development and future evolution.

### 1.4 Problem Description

Customers need a platform where they can browse products and purchase them through an online shopping process.

Store administrators need to manage the products offered by the platform and access the information required to operate the store.

The system must provide the functionality and security required to support these interactions.

### 1.5 System Description

Nova E-Commerce is a web-based application composed of a frontend, a backend API, and a database.

- **Frontend:** technology-agnostic web client.
- **Backend:** RESTful API developed with Python and FastAPI.
- **Database:** PostgreSQL.

The frontend communicates with the backend through the API. The backend implements the application's business logic and manages access to persistent data.

## 2. Requirements

### 2.1 Introduction

This section describes the initial requirements identified for the Nova E-Commerce system. The requirements are organized into user requirements, which describe the expected capabilities from the user perspective, and system requirements, which will provide more detailed specifications for implementation. These requirements will be reviewed, validated, and prioritized in association with the customer as the project evolves.

### 2.2 User Requirements

#### Product Management

- UR-001 - Create a product.
- UR-002 - View products.
- UR-003 - Update product information.
- UR-004 - Deactivate a product.

#### Customer Management

- UR-005 - Register a customer.
- UR-006 - View customer information.
- UR-007 - Update customer information.

#### Shopping Cart

- UR-008 - Add a product to the cart.
- UR-009 - Change product quantity.
- UR-010 - Remove a product from the cart.
- UR-011 - View the cart.

#### Ordering

- UR-012 - Place an order.
- UR-013 - View an order.
- UR-014 - Cancel an order if it is pending.

#### Payment

- UR-015 - Process a payment.
- UR-016 - Protect payment information.

### 2.3 System Requirements (Details)

#### 2.3.1 Product Management

- SR-001.1 - The system must allow administrators to create a new product.
- SR-002.1 - The system must allow users to view all active products.
- SR-003.1 - The system must allow administrators to update product information.
- SR-004.1 - The system must allow administrators to deactivate products.

#### 2.3.2 Customer Management

- SR-005.1 - The system must allow users to register a customer account.
- SR-006.1 - The system must allow authenticated customers to view their own account information.
- SR-006.2 - The system must allow administrators to view customer information, excluding sensitive data.
- SR-007.1 - The system must allow authenticated customers to update their own account information.

#### 2.3.3 Shopping Cart

- SR-008.1 - The system must allow the authenticated customer to add products to the cart.
- SR-009.1 - The system must allow the authenticated customer to increase quantity of a product currently in the cart.
- SR-009.2 - The system must allow the authenticated customer to decrease quantity of a product currently in the cart.
- SR-010.1 - The system must allow the authenticated customer to remove a product currently in the cart.
- SR-011.1 - The system must allow the authenticated customer to view all products currently in the cart and their quantities.
- SR-011.2 - The system must allow the authenticated customer to view the total price.

#### 2.3.4 Ordering

- SR-012.1 - The system must allow the authenticated customer to place an order using the products currently in the cart.
- SR-012.2 - The system must create an order with a unique identifier.
- SR-012.3 - The system must record the products and quantities included in the order.
- SR-012.4 - The system must record the total price of the order.
- SR-013.1 - The system must allow the authenticated customer to view an order.
- SR-013.2 - The system must allow the authenticated customer to view the products and quantities included in an order.
- SR-013.3 - The system must allow the authenticated customer to view the total price of an order.
- SR-013.4 - The system must allow the authenticated customer to view the current status of an order.
- SR-014.1 - The system must allow the authenticated customer to cancel an order while its status is pending.
- SR-014.2 - The system must change the status of a cancelled order to cancelled.

#### 2.3.5 Payment

- SR-015.1 - The system must allow the authenticated customer to initiate a payment for an order.
- SR-015.2 - The system must validate the payment information provided by the customer.
- SR-015.3 - The system must process the payment for the total price of the order.
- SR-015.4 - The system must record the result of the payment.
- SR-015.5 - The system must associate the payment with the corresponding order.
- SR-016.1 - The system must protect the customer's payment information from unauthorized access.
- SR-016.2 - The system must not store sensitive payment information unless required by the payment processing requirements.

## 3. Classification of Requirements

This section classifies the requirements according to their nature and purpose. Functional requirements describe the behaviors, operations, and capabilities that the system must provide to its users. Non-functional requirements describe quality attributes and constraints, such as security, reliability, usability, performance, and maintainability. This classification helps organize the requirements for analysis, implementation planning, and validation.

### 3.1 Functional Requirements

Manage Products

(place holders)
- FR-000.

### 3.2 Non-functional Requirements (Quality)

(place holders)
- NFR-000.

## 4. Prioritization of Requirements

### 4.1 Essentials

### 4.2 Importants

### 4.3 Wishables
