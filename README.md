# Pulse API

This is the backend for **Pulse**, a mobile news app built with React Native and Spring Boot. It's designed to give younger users quick, important news updates with context and upcoming events — all in a simple, swipeable format.

---

## What this project does

- Serves a daily feed of short news summaries
- Includes a “why it matters” explanation for each story
- Tracks upcoming important events (elections, tech drops, etc.)
- Designed to be fast, clean, and easy to use

---

## Tech Stack

- Java 17
- Spring Boot (Web, JPA, DevTools)
- H2 (for now) or MySQL (later)
- Lombok (optional)

---

## Project Structure

```
backend/
└── src/main/java/com/pulse/pulseapi/
    ├── controller/     # API routes
    ├── service/        # Handles logic
    ├── model/          # Database entities
    ├── repository/     # Database interfaces
    └── PulseApiApplication.java
```

---

## How to Run (Backend)

1. Clone the repo
2. Open `/backend` in IntelliJ or your favorite IDE
3. Make sure `application.properties` is set up (H2 for now)
4. Run the project

The API will be available at:
```
http://localhost:8080/api
```

---

## Planned Endpoints

- `GET /api/articles` – get all articles
- `POST /api/articles` – create a new article
- `GET /api/events` – get upcoming events
- `POST /api/events` – add a new event

---

## Notes

- The frontend (React Native app) will pull data from these endpoints using Axios or fetch.
- More features will be added over time (reactions, user preferences, AI summaries, etc.)
- This is a personal project for learning and building a real-world full stack app

---

## Author

Chris Miller  
[github.com/knoxdevchris](https://github.com/knoxdevchris)  
[linkedin.com/in/chris-millerx](https://linkedin.com/in/chris-millerx)
