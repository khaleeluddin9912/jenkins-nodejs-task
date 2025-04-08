# Task 2 - Jenkins CI/CD Pipeline with Docker and Node.js

## ✅ Objective
The goal of this task was to set up a basic **CI/CD pipeline using Jenkins** and **Docker** to automate the build and deployment process of a **Node.js** application.

---

## ⚙️ What I Did

1. **Created a simple Node.js application** that displays a message `Hello from CI/CD Pipeline!` on port `3000`.
2. **Dockerized the application** by writing a Dockerfile to containerize the app.
3. **Pulled Jenkins using Docker** and accessed it on `http://localhost:8080`.
4. Installed required Jenkins plugins: Git, Docker, Pipeline, and Blue Ocean.
5. Created a **Jenkins Pipeline** project in Jenkins.
6. Wrote a `Jenkinsfile` that:
   - Pulls the Node.js app from GitHub
   - Builds the Docker image
   - Runs a container from the image
7. Verified the deployed app runs on `http://localhost:3000`.

---

## 📁 Files Included

- `app.js` – Main Node.js app
- `Dockerfile` – For containerizing the app
- `Jenkinsfile` – Jenkins pipeline script
- `package.json` – Node.js dependencies
- `screenshots/` – Task proof screenshots
- `README.md` – This file

---

## 🔗 Output
The app was successfully deployed and visible at:  
`http://localhost:3000` → `Hello from CI/CD Pipeline!`

---

## 👤 Author  
**Mohammed Khaleel Uddin**

📅 **Date:** April 8, 2025
