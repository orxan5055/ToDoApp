To-Do List Application
A simple To-Do List application built using Spring Boot, Thymeleaf, and H2 Database.

Features

- Add Tasks: Create new tasks to be added to the list.

- Delete Tasks: Remove tasks from the list.

- Toggle Task Status: Mark tasks as completed or uncompleted.

Technologies Used

- Spring Boot: Framework for building Java-based backend applications.

- Spring MVC: Model-View-Controller pattern to separate the application’s concerns.

- Thymeleaf: A modern server-side Java template engine for web and standalone environments.

- H2 Database: In-memory database for quick and lightweight storage.

Setup
Clone the repository:
```
git clone https://github.com/your-username/to-do-app.git
cd to-do-app
```
Build the project using Maven:

```
mvn clean install
```
Run the application:

```
mvn spring-boot:run
```
Access the application:
Open your browser and visit http://localhost:8080.

Endpoints

GET /: Displays the list of tasks.

POST /add: Adds a new task.

GET /delete/{id}: Deletes a task by its ID.

GET /toggle/{id}: Toggles the task status (completed/uncompleted).

Database

H2 Database is used for this application. It is an in-memory database, so it will be reset every time the application restarts.

You can access the H2 console at http://localhost:8080/h2-console (ensure that H2 console is enabled).

Folder Structure

```
src

 ├── main
 │    ├── java
 │    │    ├── com
 │    │    │    └── example
 │    │    │         └── todoapp
 │    │    │             ├── controller
 │    │    │             │    └── TaskController.java
 │    │    │             ├── model
 │    │    │             │    └── Task.java
 │    │    │             ├── repository
 │    │    │             │    └── TaskRepository.java
 │    │    │             └── service
 │    │    │                  └── TaskService.java
 │    ├── resources
 │    │    ├── templates
 │    │    │    └── index.html
 │    │    ├── application.properties
 │    │    └── static
 │    └── test
 │         ├── java
 │         └── resources
 └── pom.xml
```
Contribution

Feel free to fork this repository and create pull requests. If you find any bugs or want to suggest new features, please open an issue.
