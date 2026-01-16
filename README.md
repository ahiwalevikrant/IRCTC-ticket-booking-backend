# IRCTC Train Booking System

A console-based train ticket booking application built with Java and Gradle, simulating the functionality of the Indian Railway Catering and Tourism Corporation (IRCTC) system.

## Description

This project is a practice implementation of a train booking system using Spring Boot and Angular concepts, but implemented as a pure Java console application. It allows users to sign up, log in, search for trains, book seats, view bookings, and cancel reservations. The system uses local JSON files for data persistence.

## Features

- **User Management**: Sign up and login functionality with password hashing
- **Train Search**: Search trains by source and destination stations
- **Seat Booking**: Interactive seat selection and booking
- **Booking Management**: View and cancel existing bookings
- **Data Persistence**: Uses JSON files for storing user and train data
- **Console Interface**: Simple command-line interface for all operations

## Prerequisites

- Java 8 or higher
- Gradle 7.0 or higher

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd IRCTC
   ```

2. Build the project:
   ```bash
   ./gradlew build
   ```

## Usage

Run the application:
```bash
./gradlew run
```

Follow the on-screen menu to:
1. Sign up for a new account
2. Login with existing credentials
3. Search for trains between stations
4. Book seats on selected trains
5. View your bookings
6. Cancel bookings
7. Exit the application

## Project Structure

```
IRCTC/
├── app/
│   ├── build.gradle          # Gradle build configuration
│   └── src/
│       ├── main/
│       │   ├── java/
│       │   │   └── ticket/
│       │   │       └── booking/
│       │   │           ├── App.java                    # Main application class
│       │   │           ├── entities/                   # Data model classes
│       │   │           │   ├── Ticket.java
│       │   │           │   ├── Train.java
│       │   │           │   └── User.java
│       │   │           ├── LocalDb/                   # Local database files
│       │   │           │   ├── trains.json
│       │   │           │   └── users.json
│       │   │           ├── service/                   # Business logic services
│       │   │           │   ├── TrainService.java
│       │   │           │   └── UserBookingService.java
│       │   │           └── Util/                      # Utility classes
│       │   │               └── UserServiceUtil.java
│       │   └── resources/
│       │       └── localdb/                          # Resource database files
│       │           ├── trains.json
│       │           └── users.json
│       └── test/
│           └── java/
│               └── ticket/
│                   └── booking/
│                       └── AppTest.java               # Unit tests
├── gradle/
│   └── wrapper/                                       # Gradle wrapper files
├── gradlew                                            # Gradle wrapper script (Unix)
├── gradlew.bat                                        # Gradle wrapper script (Windows)
├── settings.gradle                                    # Gradle settings
└── README.md                                          # This file
```

## Dependencies

- **Jackson Databind**: For JSON serialization/deserialization
- **Lombok**: For reducing boilerplate code
- **jBCrypt**: For password hashing
- **Guava**: General-purpose utilities

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is for pratice purposes only.
