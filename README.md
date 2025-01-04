# Simple demo blog - Spring Boot - Thymeleaf - Gradle project
![JDK](https://img.shields.io/badge/JDK-17-orange)
![springBoot](https://img.shields.io/badge/Spring%20Boot-2.6.7-brightgreen)
![Thymleaf](https://img.shields.io/badge/Thymeleaf-3.0.15-darkgreen)
![H2](https://img.shields.io/badge/H2-1.4.2-darkblue)
|![screanshot](img.png)|
|-----|

### Description
Thymeleaf Spring Boot Gradle project for demonstration and educational purposes. Simple demo blog with user authentication and blog post management. Features include basic authentication, user creation and full CRUD (Create, Retrieve, Update, Delete) operations on posts and comments. Blog is pre-populated with demo data on application start. Create new user or login with any author full name, password is `password`, administrator username: `admin` password: `admin`.


### Design

#### Implementation Policy
- Built using Spring Boot framework with a layered architecture
- Follows MVC (Model-View-Controller) pattern
- Uses Spring Security for authentication and authorization
- Implements JPA/Hibernate for database operations
- Thymeleaf templating engine for server-side rendering
- Gradle build system for dependency management and building
- H2 database for data persistence

#### Directory Structure
```
src/main/
├── java/lt/codeacademy/blog/
│   ├── advice/          # Global exception handlers
│   ├── config/          # Application configuration classes
│   ├── controller/      # MVC controllers handling HTTP requests
│   ├── dto/             # Data Transfer Objects
│   ├── entity/          # JPA entities
│   ├── exception/       # Custom exceptions
│   ├── repository/      # Data access layer interfaces
│   ├── service/         # Business logic layer
│   └── utils/           # Utility classes
└── resources/           # Application properties and templates
```

#### Package Roles
- `advice`: Contains global exception handlers for consistent error handling across the application
- `config`: Spring configuration classes, including security and web configurations
- `controller`: REST and web controllers that handle HTTP requests and manage view navigation
- `dto`: Data Transfer Objects for carrying data between processes and layers
- `entity`: JPA entity classes that map to database tables
- `exception`: Custom exception classes for specific application error scenarios
- `repository`: JPA repositories for database operations
- `service`: Business logic implementation and transaction management
- `utils`: Helper classes and utility functions used across the application

### Installation

Download source code as zip, unzip archive or
```
git clone https://github.com/hmurij/thymeleaf-spring-mvc-blog.git
```
Navigate to project folder and run
```
gradlew bootRun
```

### Access the application

Access application on http://localhost:8080.

### Reference
* [Sister project using React and Spring Boot REST API](https://github.com/hmurij/react-spring-boot-blog)
