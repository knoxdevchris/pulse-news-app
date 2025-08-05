# Pulse API

This is the backend for **Pulse**, a mobile news app built with Flutter and Spring Boot. It's designed to give younger users quick, important news updates with context and upcoming events—all in a simple, swipeable format.

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
src/main/java/com/pulse/pulseapi/
├── controller/     # API routes
├── service/        # Handles logic
├── model/          # Database entities
├── repository/     # Database interfaces
└── PulseApiApplication.java
```

---

## How to Run

1. Clone the repo
2. Open in IntelliJ or your favorite IDE
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

- This is backend only. The frontend (Flutter) will pull from these endpoints.
- More features will be added over time (reactions, user prefs, AI summaries, etc.)
- This is a personal project for learning and experimenting with full-stack dev

---

## Author

Chris Miller  
[github.com/knoxdevchris](https://github.com/knoxdevchris)  
[linkedin.com/in/chris-millerx](https://linkedin.com/in/chris-millerx)
