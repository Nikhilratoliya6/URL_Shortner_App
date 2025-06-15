# 🔗 URL Shortener Application

This is a full-stack URL Shortener web application where users can shorten long URLs, track how many times they've been clicked, and view analytics through dynamic charts. It includes authentication and role-based access, and is built using:

- 🔧 Spring Boot (Backend)
- ⚛️ React + Vite (Frontend)
- 🛢 MySQL or H2 (Database)
- 🔐 Spring Security with JWT
- 📊 Chart.js for analytics
- 🐳 Docker-ready (optional)

---

## 📂 Project Structure
URL-SHORTENER-PROJ/
├── url-shortener-react/   # Frontend: React + Tailwind + Vite
└── url-shortener-sb/      # Backend: Spring Boot + Spring Security + MySQL


---

## 🚀 Features

- ✅ Shorten long URLs into compact links
- 🔒 User authentication and authorization using JWT
- 📈 Track number of clicks per shortened URL
- 📊 Visualize analytics with interactive charts
- 🗃 Admin panel to monitor all shortened links
- 🧾 RESTful API structure
- ☁️ Environment variable support with `.env`
- 🐳 Docker support for containerized deployment

---

## 🛠️ Getting Started

### 📦 Prerequisites

- Java 17+
- Node.js 16+
- Maven
- MySQL (optional if using H2)
- Git

---

### 🖥️ Backend Setup (Spring Boot)

1. Navigate to the backend folder:

```bash
cd url-shortener-sb
