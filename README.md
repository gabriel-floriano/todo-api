# Todo App

This is a simple Todo App built with Spring Boot and PostgreSQL. The application allows users to manage their tasks by creating, updating, viewing, and deleting tasks. Each task includes a description, due date, and completion status.

## Features

- **Create a Task:** Add a new task with a description, due date, and completion status.
- **View All Tasks:** List all tasks with their details.
- **Update a Task:** Edit an existing task's details.
- **Delete a Task:** Remove a task from the list.
- **RESTful API:** The app provides a REST API for interacting with tasks.

## Technology Stack

- **Backend:** Spring Boot
- **Database:** PostgreSQL
- **Build Tool:** Maven
- **Language:** Java
- **IDE:** IntelliJ IDEA Community

## Getting Started

### Prerequisites

- **Java 17:** Ensure Java 17 or higher is installed on your machine.
- **PostgreSQL:** A running instance of PostgreSQL.
- **Maven:** Used for managing dependencies and building the project.

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```


2. **Set up PostgreSQL:**
  - Create a PostgreSQL database for the project:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```
  - Update the application.properties file with your PostgreSQL credentials:
   ```bash
   spring.datasource.url=jdbc:postgresql://localhost:5432/todoapp
   spring.datasource.username=your-username
   spring.datasource.password=your-password
   spring.jpa.hibernate.ddl-auto=update
   ```


3. **Install dependencies:**

   ```bash
   mvn clean install
   ```


4. **Run the application:**

   ```bash
   mvn spring-boot:run
   ```

### API Endpoints
- **GET /api/tasks:** Retrieve all tasks.
- **GET /api/tasks/{id}:** Retrieve a specific task by ID.
- **POST /api/tasks:** Create a new task.
- **PUT /api/tasks/{id}:** Update an existing task by ID.
- **DELETE /api/tasks/{id}:** Delete a task by ID.

### Example cURL Requests
- Create a Task:

   ```bash
   curl -X POST http://localhost:8080/api/tasks -H "Content-Type: application/json" -d '{"description":"Learn Spring Boot","dueDate":"2024-09-01","completed":false}'
   ```
- List All Tasks:

   ```bash
   curl http://localhost:8080/api/tasks
   ```

