# spring-open-api-code-generation


This project generates Spring Boot API interfaces and models using OpenAPI Generator.

## 📌 Features
- Generates API interfaces (`com.example.api`)
- Generates model classes (`com.example.model`)
- Uses **Jakarta EE** and **Java 8 Date/Time API**
- Supports OpenAPI YAML-based code generation

## 🚀 How to Generate Code
Run the following Maven command:

```sh
mvn clean openapi-generator:generate
```

This will generate the API interfaces and models inside:

```
target/generated-sources/openapi/
```

## 📂 Project Structure
```
src/
│── main/
│   ├── java/com/example/api/      # API interfaces
│   ├── java/com/example/model/    # Model classes
│   └── resources/openapi.yaml      # OpenAPI specification
```

## 🛠️ Build and Run
1. Generate code:
   ```sh
   mvn clean openapi-generator:generate
   ```
2. Build the project:
   ```sh
   mvn clean package
   ```
3. Run the Spring Boot application:
   ```sh
   mvn spring-boot:run
   ```
