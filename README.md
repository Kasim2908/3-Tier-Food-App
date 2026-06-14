# 🍔 QuickBite - 3-Tier Food Ordering Application

A full-stack food ordering application deployed on **AWS EC2** using **Docker** and **Docker Compose**, following a **3-tier architecture** consisting of:

* **Frontend Tier (Nginx + HTML/CSS/JavaScript)**
* **Application Tier (Node.js + Express.js)**
* **Database Tier (MongoDB)**

---

## 🚀 Project Overview

QuickBite is a containerized food ordering application that allows users to:

* 🔐 Register and Login
* 🍕 Browse food items
* 🛒 Add items to cart
* 📦 Place orders
* 💾 Store user and order data in MongoDB

The entire application is deployed on an **AWS EC2 instance** using Docker containers managed with Docker Compose.

---

## 🏗️ Architecture

```text
                Internet
                    │
                    ▼
          ┌────────────────────┐
          │  Frontend Container │
          │       (Nginx)       │
          │      Port 80        │
          └────────────────────┘
                    │
                    ▼
          ┌────────────────────┐
          │ Backend Container  │
          │ Node.js + Express  │
          │     Port 5001      │
          └────────────────────┘
                    │
                    ▼
          ┌────────────────────┐
          │ MongoDB Container  │
          │     Port 27017     │
          └────────────────────┘
```

---

# ⚙️ Tech Stack

### Frontend

* HTML
* CSS
* JavaScript
* Nginx

### Backend

* Node.js
* Express.js

### Database

* MongoDB

### DevOps Tools

* Docker
* Docker Compose
* AWS EC2
* Git & GitHub
* Linux

---

# 📂 Project Structure

```text
.
├── backend/
├── frontend/
├── Dockerfile.backend
├── Dockerfile.frontend
├── docker-compose.yml
├── nginx.conf
├── README.md
└── architecture.html
```

---

# 🐳 Docker Containers

| Container          | Technology | Port  |
| ------------------ | ---------- | ----- |
| quickbite_frontend | Nginx      | 80    |
| quickbite_backend  | Node.js    | 5001  |
| quickbite_db       | MongoDB    | 27017 |

---

# 🚀 Deployment on AWS EC2

### Clone Repository

```bash
git clone https://github.com/Kasim2908/3-Tier-Food-App.git
cd 3-Tier-Food-App
```

---

### Start Application

```bash
docker compose up -d
```

---

### Verify Running Containers

```bash
docker ps
```

---

### Stop Containers

```bash
docker compose down
```

---

# 🌐 Access Application

Frontend:

```text
http://<EC2-PUBLIC-IP>
```

Backend API:

```text
http://<EC2-PUBLIC-IP>:5001
```

---

# 🛠️ Challenges Faced

During deployment several real-world issues were encountered and resolved:

* SSH private key permission errors
* Docker installation issues
* Port mapping and AWS Security Groups
* MongoDB container crashes
* Docker networking issues
* MongoDB hostname resolution (`EAI_AGAIN mongodb`)
* Signup/Login failures
* Container communication problems
* MongoDB data verification

---

# 📚 Key Learnings

* Linux Administration
* Docker & Docker Compose
* AWS EC2 Deployment
* Container Networking
* MongoDB Integration
* Nginx Configuration
* Application Debugging
* Real-world Troubleshooting

---

# 🔮 Future Improvements

* ✅ HTTPS using Let's Encrypt
* ✅ Custom Domain with Route53
* ✅ GitHub Actions CI/CD
* ✅ Docker Hub Integration
* ✅ Terraform Infrastructure as Code
* ✅ Kubernetes Deployment
* ✅ Monitoring with Prometheus & Grafana

---

# 🛠 Built With

* Node.js
* Express.js
* MongoDB
* Docker
* Docker Compose
* Nginx
* AWS EC2

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

---

## 👨‍💻 Author

**Kasim2908**

Connect with me on LinkedIn and GitHub!

Happy Learning 🚀
