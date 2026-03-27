# ☁️ Cloud Task Management System (Backend)

A scalable **Task Management System Backend** built using **Microservices Architecture** with Spring Boot and Spring Cloud. This system enables efficient task handling, user management, and secure authentication through independent services.

---

## 🚀 Project Overview

This project follows a **Microservices Architecture**, where the backend is divided into multiple independent services that communicate through APIs.

Each service is responsible for a specific functionality such as user management, task handling, and authentication.

✔️ Scalable
✔️ Maintainable
✔️ Cloud-ready

Microservices architecture allows applications to be built as **loosely coupled services** that communicate via APIs, making them easier to scale and manage.

---

## 🧩 Microservices Included

### 1️⃣ Eureka Server (Service Discovery)

* Registers all microservices
* Enables communication between services
* Dashboard: `http://localhost:8761`

---

### 2️⃣ API Gateway

* Single entry point for all client requests
* Routes requests to appropriate services
* Handles load balancing and routing

👉 API Gateway acts as the **central access point** for microservices.

---

### 3️⃣ User Service

* Manage users
* CRUD operations (Create, Read, Update, Delete)
* Connects with MySQL database

---

### 4️⃣ Task Service

* Manage tasks
* Create, update, delete tasks
* Assign tasks to users

---

### 5️⃣ Auth Service

* Handles authentication (Login/Register)
* Can be extended with JWT security

---

## 🛠️ Tech Stack

* ☕ Java 17
* 🌱 Spring Boot
* ☁️ Spring Cloud
* 🔍 Eureka Server
* 🌐 API Gateway
* 🗄️ MySQL
* 📦 Maven

---

## 📁 Project Structure

```bash
task-management-microservices/
│
├── eureka-server/
├── api-gateway/
├── user-service/
├── task-service/
├── auth-service/
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/chamodhihansanaa/CloudTaskManagementSystem-BackEnd-.git
cd CloudTaskManagementSystem-BackEnd-
```

---

### 2️⃣ Build Project

```bash
mvn clean install
```

---

### 3️⃣ Run Services (Order Important)

1. Eureka Server
2. User Service
3. Task Service
4. Auth Service
5. API Gateway

---

## 🌐 API Access

All APIs are accessed through **API Gateway**

### Example:

```bash
http://localhost:8080/users
http://localhost:8080/tasks
http://localhost:8080/auth
```

---

## 🗄️ Database Setup

```sql
CREATE DATABASE taskdb;
```

Update `application.yml`:

```yaml
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/taskdb
    username: root
    password: 
```

---

## 🧪 Testing

Use tools like:

* Postman
* Swagger (optional)

---

## 🌍 Deployment

This project can be deployed using:

* Google Cloud Platform (GCP)
* Docker Containers


---

## 🔐 Future Improvements

* JWT Authentication
* Role-based access control (Admin/User)
* Docker  deployment
* Cloud deployment (GCP / AWS)

---

## 👩‍💻 Author

Chamodi Hansana
Software Engineering Student

---

## 📄 License

This project is for educational purposes.


## Images
### Eureka DashBoard
![EurekaDashboard](https://github.com/user-attachments/assets/1d6ed16d-8afc-495a-95ec-055faa570728)

### Postman Collection
![Postman ](https://github.com/user-attachments/assets/41a9b9aa-e74c-4f75-96b1-c75de5d640bd)




