# 🚀 Node.js Demo App - CI/CD Pipeline Using GitHub Actions

This project demonstrates how to automate **build and deployment** of a Node.js web application using **GitHub Actions** and **Docker**.

---

## 🧩 Tech Stack
- **Node.js**
- **Docker**
- **GitHub Actions**
- **Docker Hub**

---

## ⚙️ Project Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/tejaswini2704/nodejs-demo-app.git
cd nodejs-demo-app
````

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Run the App Locally

```bash
node index.js
```

Then open your browser at 👉 **[http://localhost:3000](http://localhost:3000)**

---

## 🐳 Docker Commands

### Build Docker Image

```bash
docker build -t nodejs-demo-app .
```

### Run Docker Container

```bash
docker run -d -p 3000:3000 nodejs-demo-app
```

Then visit 👉 **[http://localhost:3000](http://localhost:3000)**

---

## ⚡ CI/CD Pipeline Using GitHub Actions

This repository includes an automated CI/CD workflow located at:

```
.github/workflows/main.yml
```

### The workflow performs:

1. Checkout code
2. Setup Node.js
3. Run test command
4. Build Docker image
5. Push image to Docker Hub

---

## 🔐 GitHub Secrets Required

Before running the pipeline, add the following secrets in your GitHub repo:

* `DOCKER_USERNAME`
* `DOCKER_PASSWORD`

---

## 🧪 Test Command

Add this in your **package.json** under `"scripts"`:

```json
"test": "echo 'Running tests...' && exit 0"
```

---

## 🧠 Trigger

The pipeline runs automatically on:

```yaml
on:
  push:
    branches: [ "main" ]
```

---

## 👩‍💻 Author

**Tejaswini Shirke**
GitHub: [@tejaswini2704](https://github.com/tejaswini2704)

```
