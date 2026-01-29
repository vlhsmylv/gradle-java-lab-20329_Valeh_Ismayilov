# Gradle Java Lab

A simple Java application built with Gradle.

## Prerequisites

- **Java 25** (or let Gradle auto-download it via Foojay toolchain resolver)
- **Gradle 8.14.3** (included via wrapper)

## Running the Project

### Build

```bash
./gradlew build
```

### Run the Application

```bash
./gradlew run
```

### Run Tests

```bash
./gradlew test
```

### Clean Build

```bash
./gradlew clean build
```

## Project Structure

```
├── app/
│   ├── build.gradle.kts    # App module build config
│   └── src/main/java/org/example/App.java
├── gradle/
│   ├── libs.versions.toml  # Dependency versions catalog
│   └── wrapper/            # Gradle wrapper files
├── settings.gradle.kts     # Project settings
└── gradlew / gradlew.bat   # Gradle wrapper scripts
```

## Dependencies

- [Guava](https://github.com/google/guava) 33.4.5-jre
- [JUnit Jupiter](https://junit.org/junit5/) 5.12.1 (testing)

## Notes

- Uses Gradle configuration cache for faster builds
- JDK toolchain auto-provisioning enabled (no manual Java installation required if Gradle can download it)

## Windows Users

Use `gradlew.bat` instead of `./gradlew`:

```cmd
gradlew.bat run
```
