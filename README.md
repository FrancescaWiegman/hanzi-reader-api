# Hanzi Reader - Backend API

Backend API server for Hanzi Reader. Handles segmentation, annotation, and user management.

## Features

- 🔤 Chinese text segmentation
- 📝 Automatic annotation (pinyin, tones, HSK levels)
- 📊 Text statistics and analysis
- 👤 User vocabulary management
- 🎯 Spaced repetition tracking
- 🔍 Dictionary lookups

## Tech Stack

- **Java 17** - Language
- **Spring Boot 3.x** - Framework
- **Spring Data JPA** - ORM
- **PostgreSQL** - Database
- **HanLP** - Chinese NLP
- **Maven** - Build tool

## Project Structure

```
src/
├── main/java/com/hanzi/
│   ├── controller/       # REST endpoints
│   ├── service/          # Business logic
│   ├── model/            # Entity classes
│   ├── repository/       # Data access
│   ├── pipeline/         # Segmentation pipeline
│   ├── annotation/       # Annotation engine
│   └── HanziReaderApplication.java
└── test/
```

## Database Setup

```bash
# Create PostgreSQL database
createdo db hanzi_reader
```

## Building & Running

### Prerequisites
- Java 17+
- Maven 3.8+
- PostgreSQL 12+

### Development

```bash
mvn clean install
mvn spring-boot:run
```

The API will be available at `http://localhost:8080/api`

### Production

```bash
mvn clean package
java -jar target/hanzi-reader-api-0.1.0.jar
```

## API Endpoints

See `docs/API.md` for detailed API specification.

## Related Repositories

- [Web Frontend](https://github.com/FrancescaWiegman/hanzi-reader-web)
- [Data Pipeline](https://github.com/FrancescaWiegman/hanzi-reader-data-pipeline)
- [Android](https://github.com/FrancescaWiegman/hanzi-reader-android)
- [iOS](https://github.com/FrancescaWiegman/hanzi-reader-ios)
