# RestDemo: Spring Boot Docker Application

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Maven](https://img.shields.io/badge/Apache_Maven-C71A36?style=for-the-badge&logo=apache-maven&logoColor=white)

A lightweight, production-ready RESTful web service built with **Spring Boot 3.3.3** and fully containerized using **Docker**. This project serves as a reference implementation for building, testing, and deploying Java-based microservices within isolated environments.

---

## 🚀 Features

- **RESTful API**: Simple and efficient endpoints implemented via Spring Web.
- **Dockerized**: Includes a multi-stage `Dockerfile` for optimized containerization.
- **Spring Boot 3.3.3**: Utilizes the latest stable features of the Spring ecosystem.
- **Maven Wrapper**: Includes `mvnw` scripts to ensure consistent builds across different environments without requiring a local Maven installation.
- **Automated Testing**: Integrated unit testing suite using JUnit 5 and Spring Boot Test.

---

## 🛠️ Technologies Used

- **Language:** Java 17 (OpenJDK)
- **Framework:** Spring Boot 3.3.3
- **Build Tool:** Apache Maven
- **Containerization:** Docker
- **Web Layer:** Spring Web (MVC)
- **Testing:** JUnit 5, MockMvc

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
Use the Maven wrapper to compile the application and run tests. This will generate an executable JAR file in the `target/` directory.

**On Linux/macOS:**
```bash
./mvnw clean package
```

**On Windows:**
```bash
mvnw.cmd clean package
```

---

## 🐳 Docker Integration

This project is designed to run seamlessly in a containerized environment.

### Build the Docker Image
From the `RestDemo` directory, run:
```bash
docker build -t rest-demo:latest .
```

### Run the Container
Once the image is built, start the container and map the internal port (8080) to your host machine:
```bash
docker run -p 8080:8080 rest-demo:latest
```
The application will now be accessible at `http://localhost:8080`.

---

## 📡 API Documentation

The application exposes a simple REST controller. Once the application is running, you can interact with the following endpoint:

### Hello Endpoint
- **URL:** `/` or `/hello` (depending on implementation)
- **Method:** `GET`
- **Response:** `200 OK`
- **Body:** Returns a "Hello World" or greeting message.

**Example Request:**
```bash
curl http://localhost:8080/
```

---

## 📂 Project Structure

```text
RestDemo/
├── src/
│   ├── main/
│   │   ├── java/com/vivek/RestDemo/
│   │   │   ├── RestDemoApplication.java  # Main entry point
│   │   │   └── HelloController.java      # REST Endpoints
│   │   └── resources/
│   │       └── application.properties     # App configuration
│   └── test/                             # Unit & Integration tests
├── Dockerfile                            # Docker configuration
├── pom.xml                               # Maven dependencies
└── mvnw                                  # Maven wrapper script
```

---

## 🧪 Running Tests

To execute the test suite and ensure everything is working correctly:

```bash
./mvnw test
```

The test results, including coverage reports, will be available in the `target/surefire-reports/` directory.

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

This project is currently unlicensed. Please check the repository for updates regarding licensing.

---

## ✉️ Contact

**Vivek Bhosale** - [GitHub Profile](https://github.com/bhosalevivek04)

Project Link: [https://github.com/bhosalevivek04/Docker](https://github.com/bhosalevivek04/Docker)