
# 🔗 URL Shortener Web Application

A production-ready full-stack URL shortener application that allows users to shorten long URLs, track usage analytics, and view interactive charts. It includes secure authentication and role-based access, built using modern technologies:

- ⚙️ **Backend:** Spring Boot  
- 💻 **Frontend:** React + Vite  
- 🛢 **Database:** MySQL or H2  
- 🔐 **Authentication:** Spring Security with JWT  
- 📊 **Analytics:** Chart.js  
- 🐳 **Deployment Ready:** Docker Support  

---

## 📁 Project Structure

URL-SHORTENER-PROJ/
├── url-shortener-react/   # Frontend (React, Vite, Tailwind)
└── url-shortener-sb/      # Backend (Spring Boot, JWT, MySQL)

---

## 🚀 Key Features

- 🔗 Shorten long URLs into compact, shareable links  
- 🔐 User authentication and role-based access (JWT)  
- 📈 Click tracking and real-time usage analytics  
- 📊 Visual dashboards using Chart.js  
- 🗂 Admin panel to manage all shortened links  
- 📤 RESTful API architecture  
- ☁️ Environment variable support via `.env`  
- 🐳 Dockerized backend setup for containerized deployment  

---

## 🛠️ Getting Started

### ✅ Prerequisites

Ensure the following are installed on your machine:

- Java 17+  
- Node.js 16+  
- Maven  
- MySQL (or use H2 for in-memory DB)  
- Git  

---

### 🔧 Backend Setup (Spring Boot)

```bash
# 1. Navigate to the backend directory
cd url-shortener-sb

2. Configure the application:

Edit src/main/resources/application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/url_shortener
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
jwt.secret=your_jwt_secret_key

# 3. Build and run the app
./mvnw install
./mvnw spring-boot:run

Server will be running at: http://localhost:8080

⸻

🌐 Frontend Setup (React + Vite)

# 1. Navigate to the frontend directory
cd ../url-shortener-react

2. Create a .env file in the root directory:

VITE_API_BASE_URL=http://localhost:8080/api

# 3. Install dependencies and start dev server
npm install
npm run dev

Frontend will be available at: http://localhost:5173

⸻

📡 Sample API Endpoints
	•	POST /api/auth/register — Register a new user
	•	POST /api/auth/login — User login and JWT issuance
	•	POST /api/shorten — Shorten a URL (authenticated)
	•	GET /api/shorten/all — Retrieve all URLs for the user
	•	GET /{shortCode} — Redirect to original URL

⸻

🐳 Docker Setup (Optional)

If you prefer Docker-based deployment:

# Backend Docker
cd url-shortener-sb
docker build -t url-shortener-backend .
docker run -p 8080:8080 url-shortener-backend

You can similarly containerize the frontend if needed.

⸻

👤 Author

Nikhil Ratoliya
GitHub • LinkedIn

⸻

📄 License

This project is licensed under the MIT License.

Let me know if you want to include screenshots, deployment instructions (like Netlify or Render), or badges (e.g., build status, license, tech stack) too!
