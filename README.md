# 🌿 Automated Greenhouse Management System (AGMS)

Spring Boot Microservices

AGMS is a cloud-based system built to support smart agriculture using a microservices architecture. It collects real-time environmental data from an external IoT API and automatically triggers actions to maintain ideal greenhouse conditions.

---

## 🏗️ System Architecture

The system is designed using **Spring Cloud Microservices** to ensure scalability and flexibility.

### 🔹 Infrastructure Layer

* **Eureka Server** – Handles service discovery
* **API Gateway** – Central entry point with request routing and security
* **Config Server** – Manages centralized configuration

### 🔹 Business Services

* **Zone Service** – Manages greenhouse zones and temperature limits
* **Sensor Service** – Fetches real-time temperature and humidity data
* **Automation Service** – Applies rules and triggers actions (fan/heater/sprinkler)
* **Crop Service** – Tracks crop growth stages

---

## 🚀 Key Features

* **Live Data Monitoring** – Fetches IoT data at regular intervals
* **Automated Decision Making** – Applies rules based on temperature and humidity
* **Crop Lifecycle Tracking** – Manages stages from seedling to harvest
* **JWT Security** – Secured APIs via API Gateway
* **Service Communication** – Uses OpenFeign for inter-service calls

---

## 🛠️ Tech Stack

| Category      | Technology                             |
| ------------- | -------------------------------------- |
| Framework     | Spring Boot                            |
| Microservices | Spring Cloud (Eureka, Gateway, Config) |
| Security      | JWT                                    |
| Communication | OpenFeign, REST                        |
| Database      | MySQL / H2                             |
| Testing       | Postman                                |

---

## 🚦 Getting Started

### Prerequisites

* Java 17+
* Maven
* MySQL
* Git

---

### ▶️ Run the System

Start services in this order:

1. Config Server
2. Eureka Server
3. API Gateway
4. Zone Service
5. Automation Service
6. Sensor Service
7. Crop Service

---

### ✅ Verify

Open:
http://localhost:8761

Check all services are **UP**

---

## 🧪 API Testing

* Import Postman collection
* Login and get JWT token
* Use token to access APIs via Gateway (port 8080)

---

## 📂 Project Structure

```id="p2q7yf"
agms/
├── infrastructure/
├── services/
├── config-repo/
├── docs/
└── README.md
```

---

## 📌 Features Summary

* Real-time IoT integration
* Automated rule engine
* Distributed microservice design
* Secure API access

---

## 👨‍💻 Author

Developed for **GDSE – Software Architectures & Design Patterns II**
