

# Node.js CI/CD Demo with GitHub Actions & Docker 🐳🚀

This is a simple Node.js application that demonstrates a full CI/CD pipeline using GitHub Actions and Docker.

- Node.js
- Express.js
- Docker
- GitHub Actions (CI/CD)

## 🛠️ Setup Instructions (Local)

### 1. Clone the repository

```bash
git clone https://github.com/khaleeluddin9912/-nodejs-demo-app.git
cd nodejs-cicd-demo
```

### 2. Install dependencies

```bash
npm install
```

### 3. Run the app

```bash
npm start
```

App will be running at:  
**[http://localhost:3000](http://localhost:3000)**

## 🐳 Docker Setup

### 1. Build the Docker image

```bash
docker build -t nodejs-cicd-demo .
```

### 2. Run the Docker container

```bash
docker run -p 3000:3000 nodejs-cicd-demo
```

App will be accessible at:  
**[http://localhost:3000](http://localhost:3000)**

## ⚙️ CI/CD with GitHub Actions

Every time you push code to GitHub:
- GitHub Actions will automatically build your Docker image
- Install dependencies
- Run the app inside a container

You can find the workflow file at:  
`.github/workflows/ci-cd.yml`

---

## 📷 Screenshots

| Localhost Output | GitHub Actions |
|------------------|----------------|
| ![Localhost](./screenshots/localhost.png) | ![GitHub Actions](./screenshots/github-actions.png) |

---

## 📤 Author

**Mohammed Khaleel Uddin**  
LinkedIn www.linkedin.com/in/mohammed-khaleel-uddin-9634012a0 | GitHub https://github.com/khaleeluddin9912

---

> 🚀 “Automate all the things!” – Great work finishing the CI/CD task!
=======
# jenkins-nodejs-task
>>>>>>> 847f81bc72dacc475769ed30b6b2d01164ca4eef
