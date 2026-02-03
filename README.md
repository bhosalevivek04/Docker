# RestDemo - Spring Boot Docker Application

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Maven](https://img.shields.io/badge/Apache_Maven-C71A36?style=for-the-badge&logo=apache-maven&logoColor=white)

A lightweight, production-ready RESTful web service built with **Spring Boot 3.3.3** and fully containerized using **Docker**. This project serves as a reference implementation for building and deploying Java microservices.

---

## 🚀 Features

- **RESTful API**: Simple and efficient endpoints using Spring Web.
- **Dockerized**: Includes a `Dockerfile` for easy containerization and deployment.
- **Spring Boot 3.3.3**: Leverages the latest features of the Spring ecosystem.
- **Maven Wrapper**: Build the project without needing a pre-installed Maven version.
- **Unit Testing**: Integrated testing suite using JUnit and Spring Boot Test.

---

## 🛠️ Technologies Used

- **Language:** Java 17+
- **Framework:** Spring Boot 3.3.3
- **Build Tool:** Maven
- **Containerization:** Docker
- **Web Layer:** Spring Web (MVC)

---

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- [JDK 17 or higher](https://adoptium.net/)
- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- [Git](https://git-scm.com/)

---

## 🔧 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/bhosalevivek04/Docker.git
cd Docker/RestDemo
```

### 2. Build the Project
Use the Maven wrapper to compile the application and run tests:
```bash
# On Linux/macOS
./mvnw clean package

# On Windows
mvnw.cmd clean package
```
The executable JAR file will be generated in the `target/` directory.

---

## 🐳 Docker Integration

### Build Docker Image
To create a Docker image for the application, run the following command from the `RestDemo/` directory:
```bash
docker build -t rest-demo:latest .
```

### Run Docker Container
Start the application in a container, mapping port 8080:
```bash
docker run -p 8080:8080 rest-demo:latest
```

The application will now be accessible at `http://localhost:8080`.

---

## 📖 API Documentation

The application exposes a simple REST controller (`HelloController`).

### Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET`  | `/`      | Returns a welcome message or "Hello World". |

#### Example Request
```bash
curl http://localhost:8080/
```

#### Example Response
```text
Hello from Spring Boot!
```

---

## 📂 Project Structure

```text
RestDemo/
├── src/
│   ├── main/
│   │   ├── java/com/vivek/RestDemo/     # Source code
│   │   └── resources/                   # Application properties
│   └── test/                            # Unit & Integration tests
├── Dockerfile                           # Docker configuration
├── pom.xml                              # Maven dependencies
└── mvnw                                 # Maven wrapper script
```

> **Note:** The `bin/` directory in the repository contains build artifacts and compiled classes. For development, please focus on the `src/` directory.

---

## 🧪 Running Tests

To execute the test suite, run:
```bash
./mvnw test
```
Test reports are generated in `target/surefire-reports/`.

---

## 🤝 Contributing

Contributions are welcome! To contribute:
1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

---

## 📄 License

This project is currently unlicensed. Please contact the repository owner for usage permissions.

---

## ✉️ Contact

**Vivek** - [GitHub Profile](https://github.com/bhosalevivek04)

Project Link: [https://github.com/bhosalevivek04/Docker](https://github.com/bhosalevivek04/Docker)