# 🐳 Go HTTP Server in Docker

This is a simple Go web server that runs inside a Docker container. It exposes two endpoints and returns basic text responses.

---

## 📁 Project Structure

```
.
├── Dockerfile
├── go.mod
└── main.go
```

---

## 🚀 Features

* Written in Go
* Dockerized for easy deployment
* Two basic endpoints:

  * `/` → Returns `Hello, "/"`
  * `/hi` → Returns `hi`

---

## 📦 Prerequisites

* Docker installed (latest recommended)
* Go installed (for local testing, optional)

---

## 🛠 Build Docker Image

```bash
docker build -t go-http-server .
```

---

## ▶️ Run the Docker Container

```bash
docker run -p 8080:8080 go-http-server
```

---

## 🌐 Test the Endpoints

Open in your browser or use curl:

* `http://localhost:8080/` → "Hello, "/""
* `http://localhost:8080/hi` → "hi"

---

## 🧹 Clean Docker Build Cache (if needed)

```bash
docker system prune -a
```

---

## 💬 Author

Made by Vishal Sharma aka Ego 🙌

Feel free to contribute or fork this project.

---

## 🔐 Security Tip

If you’re going to deploy this, consider using environment variables or a reverse proxy in front of this app.
