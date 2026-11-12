# RouteRed — Online Bus Reservation System (Full Stack)

A complete full-stack bus reservation platform featuring route discovery, dynamic seat layout selection, concurrent seat locking, booking management with PNR generation, and role-based portals for passengers, operators, and administrators.

## Project Structure

```
├── obrs-backend/        # Spring Boot 3.3 REST API (Java 17+, Spring Security, JPA, Flyway, PostgreSQL/MySQL)
├── obrs-frontend/       # React 18 SPA (Vite, Tailwind CSS, Lucide React, Context API)
└── README.md
```

---

## 🚀 Quick Start

### 1. Frontend Setup (`obrs-frontend`)

**Prerequisites:** Node.js 18+ and npm

```bash
cd obrs-frontend
npm install
npm run dev
```

The frontend will start at: `http://localhost:5173`

To create a production build:
```bash
npm run build
```

---

### 2. Backend Setup (`obrs-backend`)

**Prerequisites:** JDK 17+ (or 21+) and Maven 3.9+ (or Docker)

#### Option A: Run via Docker Compose (Recommended for Local DB + API)
```bash
cd obrs-backend
docker compose up --build
```
- API will be accessible at: `http://localhost:8080`
- Swagger UI will be at: `http://localhost:8080/swagger-ui.html`

#### Option B: Run via Maven (with local PostgreSQL)
```bash
cd obrs-backend
mvn spring-boot:run -Dspring-boot.run.profiles=dev
```

#### Demo Credentials (dev profile)
| Role | Email / Login | Password |
|---|---|---|
| Admin | `admin@obrs.local` | `Admin@12345` |
| Operator | `operator@obrs.local` | `Operator@123` |
| Passenger | `demo@obrs.local` | `Demo@1234` |

---

## 🛠 Tech Stack

- **Backend:** Java 17+, Spring Boot 3.3.5, Spring Security, Spring Data JPA, Hibernate, Flyway, JJWT, PostgreSQL / MySQL, Springdoc OpenAPI
- **Frontend:** React 18, Vite 5, Tailwind CSS, React Router v6, Lucide Icons, Context API
