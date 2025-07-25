# 📝 Node.js To-Do App with Docker, GitHub Actions CI/CD, and Azure

This is a simple Node.js To-Do API application built with:

- ✅ Node.js + Express
- 🐳 Dockerized
- 🚀 Deployed to Azure Web App
- 🤖 GitHub Actions for CI/CD

---

## 🌐 Live Demo

🔗 [https://todo-app-<your-app-name>.azurewebsites.net](https://todo-app-<your-app-name>.azurewebsites.net)

---

## 📦 Features

- Add, delete, update To-Do tasks
- RESTful API
- MongoDB backend (or in-memory)
- Docker support
- CI/CD using GitHub Actions
- Automatic deploy to Azure on push

---

## 🚀 Deployment Workflow

### GitHub Actions Workflow

Every time you push to `main`:
1. Docker image is built.
2. Image is pushed to Azure Container Registry (ACR).
3. Azure Web App pulls the latest image and restarts the app.

**CI/CD made simple!**

---

## ⚙️ Tech Stack

- Node.js
- Express.js
- Docker
- Azure Container Registry (ACR)
- Azure Web App
- GitHub Actions

---

## 🐳 How to Run Locally

```bash
# Clone the repo
git clone https://github.com/SakshWathare77/Node-todo-cicd.git
cd Node-todo-cicd

# Build Docker image
docker build -t node-todo-app .

# Run the container
docker run -p 3000:3000 node-todo-app
