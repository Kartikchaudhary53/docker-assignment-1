# Docker Assignment 1

This project demonstrates a **multi-container application** using **Docker** and **Docker Compose**. It includes a **frontend, backend, and database** working together in a containerized environment.

 **Live Demo:**  
https://kartikchaudhary53.github.io/docker-assignment-1/

---

##  Overview

This project is designed to showcase how modern applications can be broken into smaller services and run using containers.

- Each component runs in its own container  
- Services communicate through Docker networking  
- Docker Compose manages all services in one place  

---

##  Architecture
User (Browser)
↓
Frontend (index.html)
↓
Backend (API Server)
↓
Database


---

## 📁 Project Structure


docker-assignment-1/
│── backend/ # Backend application
│── database/ # Database setup/configuration
│── docker-compose.yml # Docker multi-container config
│── index.html # Frontend UI
│── README.md


---

## ⚙️ Technologies Used

- Docker  
- Docker Compose  
- HTML (Frontend)  
- Backend (API Service)  
- Database  

---

## 🐳 Key Concepts

### 🔹 Containers
Containers package code and dependencies so the application runs consistently across environments.

### 🔹 Docker Images
Images are templates used to create containers.

### 🔹 Docker Compose
Used to define and run multi-container applications using a single YAML file.

### 🔹 Networking
Containers communicate internally using Docker networks.

### 🔹 Port Mapping
Ports are exposed to access services from the browser:


host_port : container_port


---

## 🚀 Getting Started

### ✅ Prerequisites

Make sure you have installed:

- Docker  
- Docker Compose  

---

### 🔧 Installation Steps

#### 1. Clone the repository


git clone https://github.com/kartikchaudhary53/docker-assignment-1.git
cd docker-assignment-1
2. Run the application
docker-compose up --build

This will:

Build Docker images
Create containers
Start all services
🌐 Access the Application

After running:

Frontend → http://localhost:3000
Backend → http://localhost:5000

(Ports may vary depending on your docker-compose configuration)

🔄 Stop the Application
docker-compose down
📊 Services Description
🔹 Frontend
Static HTML page
Displays UI to users
🔹 Backend
Handles server logic
Processes API requests
🔹 Database
Stores application data
Connected to backend
📦 Docker Compose Workflow
Reads docker-compose.yml
Builds images
Creates containers
Sets up networking
Starts services
