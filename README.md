# Spring Boot Todo App

## Overview
This project is a simple Todo application built with **Spring Boot**, allowing users to manage their tasks effectively through a web interface. The application includes features for adding, updating, deleting, and viewing tasks. It integrates with a **MySQL database** for data persistence and uses **Thymeleaf** for server-side rendering.

## Features
- Add new tasks through the web interface.
- Update existing tasks.
- Delete tasks.
- View all tasks in a list format.
- Mark tasks as completed.

## Technologies Used
- **Java**: Version 21
- **Spring Boot**: Web, Data JPA, and Thymeleaf starters.
- **MySQL**: Database for task storage.
- **Lombok**: Simplifies the development of Java classes.
- **Maven**: Dependency and build management.

## Requirements
- **Java Development Kit (JDK)**: Version 21 or higher.
- **MySQL Database**: For persistence.
- **Maven**: Version 3.6 or higher.

## Installation

### Clone the Repository
```bash
git clone https://github.com/your-username/spring_boot_todo_app.git
cd spring_boot_todo_app
```

### Configure the Database
1. Create a MySQL database named `todo_db`.
2. Update the `application.properties` file in `src/main/resources/` with your MySQL credentials:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/todo_db
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   spring.jpa.hibernate.ddl-auto=update
   spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
   ```

### Build and Run the Application
1. Build the project using Maven:
   ```bash
   mvn clean install
   ```
2. Run the application:
   ```bash
   mvn spring-boot:run
   ```

### Access the Application
- **Web Interface**: `http://localhost:8080`

## Development Notes
### Lombok Configuration
Lombok is used to reduce boilerplate code. Ensure your IDE supports annotation processing:
- **IntelliJ IDEA**: Enable annotation processing in `Settings > Build, Execution, Deployment > Compiler > Annotation Processors`.
- **Eclipse**: Install the Lombok plugin.

### Testing
Run unit tests using:
```bash
mvn test
```

## Contribution
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push the branch (`git push origin feature-name`).
5. Create a pull request.

## License
This project is licensed under the [MIT License](LICENSE).

## Contact
For questions or feedback, feel free to reach out at [https://x.com/al_azwari](https://x.com/al_azwari).
