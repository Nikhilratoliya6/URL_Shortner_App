# 🔗 URL Shortener Application

A full-stack URL Shortener web application that allows users to:

- 🔹 Shorten long URLs into compact, shareable links  
- 📊 Track click analytics using interactive charts  
- 🔐 Register/login securely with JWT authentication  
- 🧑‍💼 Use an admin panel to monitor all URLs  

---

### 🧱 Tech Stack

- Backend: Spring Boot + Spring Security (JWT)
- Frontend: React + Vite + TailwindCSS
- Database: MySQL (or H2 for dev)
- Charts: Chart.js
- Docker: Containerized support for easy deployment

---

## 📁 Project Structure

URL-SHORTENER-PROJ/  
├── url-shortener-react/   # Frontend (React + Vite + Tailwind)  
└── url-shortener-sb/      # Backend (Spring Boot + JWT + MySQL)

---

## 🚀 Features

- ✅ Convert long URLs into short ones  
- 🔐 User authentication with JWT  
- 📊 Track number of clicks for each short URL  
- 📈 View analytics using charts  
- 🧾 Clean and RESTful API  
- 🗃 Admin dashboard to manage URLs  
- ☁️ Environment variable support  
- 🐳 Docker support for deployment

---

## 🛠️ Getting Started

### 📦 Prerequisites

- Java 17+  
- Node.js 16+  
- Maven  
- Git  
- MySQL (or use H2)

---

### 🖥️ Backend Setup (Spring Boot)

1. Navigate to the backend folder:

cd url-shortener-sb

2. Update the application.properties file:

spring.datasource.url=jdbc:mysql://localhost:3306/url_shortener  
spring.datasource.username=root  
spring.datasource.password=yourpassword  
spring.jpa.hibernate.ddl-auto=update  
jwt.secret=your_jwt_secret_key

3. Run the backend:

./mvnw install  
./mvnw spring-boot:run

The server will start at: http://localhost:8080

---

### 🌐 Frontend Setup (React + Vite)

1. Navigate to the frontend folder:

cd ../url-shortener-react

2. Create a .env file with the following content:

VITE_API_BASE_URL=http://localhost:8080/api

3. Install dependencies and run the frontend:

npm install  
npm run dev

The frontend will start at: http://localhost:5173

---

## 🔌 API Endpoints

POST   /api/auth/register   — Register a new user  
POST   /api/auth/login      — Login and receive JWT  
POST   /api/shorten         — Shorten a new URL (auth required)  
GET    /api/shorten/all     — Get all URLs for the user  
GET    /{shortCode}         — Redirect to original URL  

---

## 🐳 Docker Support (Optional)

1. Navigate to the backend:

cd url-shortener-sb

2. Build and run the Docker container:

docker build -t url-shortener-backend .  
docker run -p 8080:8080 url-shortener-backend

---

## 👨‍💻 Author

Nikhil Ratoliya  
GitHub: https://github.com/your-github  
LinkedIn: https://linkedin.com/in/your-linkedin

---

## 📃 License

This project is licensed under the MIT License.
