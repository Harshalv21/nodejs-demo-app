# 🚀 Node.js CI/CD Demo with GitHub Actions & Docker

This is a simple Node.js web app integrated with a CI/CD pipeline using **GitHub Actions** and **Docker**. On every push to the `main` branch, the workflow will:

- Build the Node.js app
- Run basic tests
- Build a Docker image
- Push the image to DockerHub

---

## 📁 Project Structure

.
├── app.js
├── Dockerfile
├── package.json
└── .github/
└── workflows/
└── main.yml

---

## 🔧 Technologies Used

- Node.js
- GitHub Actions (CI/CD)
- Docker
- DockerHub

---

## ⚙️ CI/CD Workflow Overview

The pipeline is defined in `.github/workflows/main.yml` and is triggered on push to the `main` branch.

### Workflow Steps:

1. **Checkout code**
2. **Set up Node.js**
3. **Install dependencies**
4. **Run tests**
5. **Log in to DockerHub**
6. **Build Docker image**
7. **Push image to DockerHub**

---

## 🔐 GitHub Secrets Required

Before running the workflow, add the following secrets in your GitHub repository:

| Secret Name         | Description                            |
|---------------------|----------------------------------------|
| `DOCKER_USERNAME`   | ------ Use Your DockerHub username -------- |
| `DOCKER_PASSWORD`   | Use Your DockerHub password or access token |

---

## 🐳 DockerHub Image

After a successful push to `main`, the Docker image is published to:

> Dockerhub

---

## 📦 Running the App Locally (Optional)

```bash
# Install dependencies
npm install

# Run the app
npm start
✅ Example Output
When run, the app listens on port 3000:

Server running on port 3000

🙋‍♂️ Author
Harshal Vernekar

