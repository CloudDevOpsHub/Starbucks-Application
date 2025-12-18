# Starbucks Application – Jenkins CI/CD Pipeline Project

This project demonstrates a **production-style CI/CD implementation using Jenkins** for a containerized web application (Starbucks Clone).  
The primary focus of this project is **CI/CD automation**, not frontend development.

---

## 📌 Project Objective

To design and implement an **end-to-end Jenkins CI/CD pipeline** that:
- Automatically builds the application on every code change
- Creates and pushes Docker images
- Deploys the application using a Continuous Deployment pipeline
- Follows **pipeline-as-code** best practices

---

## 🏗️ Architecture Overview

Developer → GitHub → Jenkins CI Pipeline → Docker Image → DockerHub → Jenkins CD Pipeline → Running Container

---

## 🔁 CI/CD Workflow

### 🔹 Continuous Integration (CI) – Jenkins
Triggered on source code changes.

Steps:
1. Checkout source code from GitHub
2. Tool installation & environment setup
3. Workspace cleanup
4. Install application dependencies (NPM)
5. Build application
6. Build Docker image
7. Tag Docker image
8. Push image to DockerHub

---

### 🔹 Continuous Deployment (CD) – Jenkins
Triggered after successful CI pipeline.

Steps:
1. Pull Docker image from DockerHub
2. Deploy application as a Docker container
3. Application available via browser

---

## ⚙️ Tech Stack

- Jenkins (Declarative Pipelines)
- Docker & DockerHub
- GitHub
- Linux
- Node.js
- React

---

> Note: Shell scripts were used during initial experimentation and learning stages.  
> The main CI/CD logic is implemented using Jenkins Declarative Pipelines.
---


---

## 📸 Jenkins Pipeline Screenshots

> Add the following screenshots here:
- Jenkins CI Stage View
 <img width="1440" height="900" alt="Screenshot 2025-12-14 at 6 08 48 PM" src="https://github.com/user-attachments/assets/af28f5de-e98f-4be1-8aad-e3f505cf3d23" />

- Jenkins CD Stage View
  <img width="1440" height="900" alt="Screenshot 2025-12-14 at 6 08 35 PM" src="https://github.com/user-attachments/assets/16b3ad0c-8b5a-4cdb-8323-203f4989b976" />

  <img width="1440" height="900" alt="Screenshot 2025-12-14 at 6 08 57 PM" src="https://github.com/user-attachments/assets/e888da5b-e456-4cde-8ab3-5fc10cd1ccf0" />

- Live deployed application

<img width="1440" height="900" alt="Screenshot 2025-12-14 at 6 07 43 PM" src="https://github.com/user-attachments/assets/d92f827b-47d5-415f-b3bf-5846489c9a86" />

---

## 🧠 Key Learnings

- Jenkins Declarative Pipeline design
- CI vs CD separation (best practices)
- Docker image lifecycle management
- Jenkins and Docker integration
- Debugging pipeline failures
- Production-style CI/CD automation

---

## 🔗 GitHub Repository

https://github.com/Rishi2911/Starbucks-Application

---

## 🎯 Career Focus

This project was built to demonstrate **real DevOps CI/CD skills** for:
- DevOps Intern roles
- Cloud Engineering roles
- Junior DevOps Engineer positions

---

## 📬 Feedback

Feedback and suggestions from DevOps professionals are welcome.
