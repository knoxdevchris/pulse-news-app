# 📰 Pulse API

**Pulse** is a modern backend API built with Java Spring Boot designed to power a mobile news application built in Flutter. The app delivers daily bite-sized news summaries and important upcoming events, focused on a younger, fast-paced audience.

---

## 🚀 Features (MVP)

- Serve curated articles with:
  - Title
  - Summary
  - Category (e.g., Tech, World, Politics)
  - “Why it matters” field
- Serve upcoming events:
  - Title, Description, Date
- Clean REST API structure
- Future: reactions, user customization, AI summaries, push notifications

---

## 🧱 Tech Stack

- **Java 17**
- **Spring Boot**
- **Spring Web**
- **Spring Data JPA**
- **MySQL (or H2 for dev testing)**
- **Lombok (optional)**
- **Spring Boot DevTools**

---

## 🗂 Folder Structure

```
src/main/java/com/pulse/pulseapi/
├── controller/     # REST endpoints
├── service/        # Business logic
├── model/          # Entity classes
├── repository/     # JPA interfaces for DB
├── dto/            # (Optional) DTOs for clean API
└── PulseApiApplication.java  # Main app entry point
```

---

## 🔧 Setup Instructions

### 1. Clone & Open
Clone the repo and open in your IDE (IntelliJ recommended).

### 2. Configure DB (Dev: H2, Prod: MySQL)

For **H2**:
```properties
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.hibernate.ddl-auto=update
```

For **MySQL**:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/pulse
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.username=YOUR_USERNAME
spring.datasource.password=YOUR_PASSWORD
spring.jpa.hibernate.ddl-auto=update
```

### 3. Run It

In your IDE or terminal:

```bash
./mvnw spring-boot:run
```

API should be live at:  
`http://localhost:8080/api`

---

## 📬 API Endpoints (Planned)

| Method | Endpoint             | Description                  |
|--------|----------------------|------------------------------|
| GET    | /api/articles        | Get all articles             |
| GET    | /api/articles/{id}   | Get article by ID            |
| POST   | /api/articles        | Create new article           |
| GET    | /api/events          | Get all upcoming events      |
| POST   | /api/events          | Create a new event           |

---

## 📌 Notes

- Frontend (Flutter) consumes these endpoints using `http` package
- Future features: categories, saved articles, user reactions, push alerts, AI summarizer

---

## 🧠 Author

Chris Miller  
- [GitHub](https://github.com/knoxdevchris)  
- [LinkedIn](https://linkedin.com/in/chris-millerx)

---

## 📄 License

This project is open-source for learning and personal use.
