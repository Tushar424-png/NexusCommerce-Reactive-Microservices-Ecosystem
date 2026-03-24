# 🚀 NexusCommerce – Reactive Microservices E-Commerce Platform

🔥 A scalable, production-style **Microservices E-Commerce Backend** built using **Spring Boot + WebFlux** with distributed architecture.

---

## 🧠 Project Overview

NexusCommerce is a fully decoupled microservices system where each service runs independently with its own database.

It ensures:

* ⚡ High performance with Reactive Programming (WebFlux)
* 🔐 Secure authentication with JWT
* 🧩 Loose coupling using API Gateway & Service Registry
* 🛡 Fault tolerance using Circuit Breaker
* 📦 Smart inventory handling with auto stock updates

---

## 🏗️ Architecture

* API Gateway (Entry point)
* Service Registry (Eureka)
* Auth Service (JWT Authentication)
* User Service (Cart, Wishlist, User Details)
* Product Service
* Inventory Service
* Order Service

Each service:
✔ Runs independently
✔ Has its own database
✔ Communicates via WebFlux

---

## 🔥 Key Features

### 🔐 Authentication & Security

* JWT-based authentication
* Role-based access (User / Admin)
* API Gateway authorization

---

### 🛒 User Features

* Register & Login
* View Products
* Add/Remove Cart
* Wishlist Management

---

### 📦 Inventory Management

* Auto stock update after order
* Product becomes inactive if out of stock
* Restock → auto active

---

### 📊 Order Processing

* Inventory checked before order
* If stock not available → error returned
* If available → order success + stock reduced

---

### 🛡 Fault Tolerance

* Circuit Breaker used
* Prevents system failure
* Improves user experience

---

## 🔄 Order Flow

1. User logs in → gets JWT token
2. Request goes through API Gateway
3. Order service checks inventory
4. If stock available → success
5. Else → failure message

---

## 🧩 Tech Stack

* Java
* Spring Boot
* Spring WebFlux
* Spring Security
* JWT Authentication
* Eureka Server
* API Gateway
* Circuit Breaker (Resilience4j)
* MySQL

---

## 📌 Microservices List

| Service           | Description          |
| ----------------- | -------------------- |
| Auth Service      | Handles login & JWT  |
| User Service      | User, Cart, Wishlist |
| Product Service   | Product management   |
| Inventory Service | Stock management     |
| Order Service     | Order processing     |
| API Gateway       | Routing & security   |
| Service Registry  | Service discovery    |

---

## 🗄️ Database Design

* Each service has its own DB
* Loose coupling maintained
* User → Cart → Wishlist relations handled separately

---

## ⚙️ How to Run

```bash
# Clone project
git clone https://github.com/your-username/NexusCommerce.git

# Run services one by one
# Start Eureka Server
# Start API Gateway
# Start all microservices
```

---

## 📊 Diagrams

### 🏗 Architecture

(Add architecture diagram image here)

### 🔄 Order Flow

(Add sequence diagram image here)

### 🧩 DB Relations

(Add ER diagram image here)

---

## 💡 Future Improvements

* Docker & Kubernetes Deployment
* CI/CD Pipeline
* Distributed Logging (ELK)
* Monitoring (Prometheus + Grafana)

---

## 👨‍💻 Author

**Tushar Handa**
Java Backend / Full Stack Developer

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!
