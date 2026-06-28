# Smart Calendar Assistant

Smart Calendar Assistant is a Java Spring Boot backend for managing personal calendars, events, reminders and schedule conflicts.

The idea is to build a personal planning assistant where a user can keep different calendars for work, study, hobbies, training and daily tasks. Calendars can be viewed separately or combined into one schedule. The application will also help detect time conflicts and remind users about important events.

## Current Scope

- Calendar management
- REST API for calendars
- PostgreSQL persistence
- Liquibase database migrations
- Validation and centralized error handling

## Planned Features

- Event management
- Schedule conflict detection
- Reminders
- Telegram bot integration
- Voice commands for creating events
- External calendar integrations

## Tech Stack

- Java 17
- Spring Boot
- Maven
- Spring Web MVC
- Spring Data JPA
- PostgreSQL
- Liquibase
- Validation
- Lombok
- JUnit

## Run Locally

Create a PostgreSQL database:

```sql
CREATE DATABASE smart_calendar_assistant;
```

Run the application with default local settings:

```bash
./mvnw spring-boot:run
```

Default database settings can be overridden with environment variables:

```bash
DB_URL=jdbc:postgresql://localhost:5432/smart_calendar_assistant
DB_USERNAME=postgres
DB_PASSWORD=postgres
```

## API

Base URL:

```text
/api/v1
```

Calendars:

```text
POST   /api/v1/calendars
GET    /api/v1/calendars
GET    /api/v1/calendars/{id}
PUT    /api/v1/calendars/{id}
DELETE /api/v1/calendars/{id}
```
