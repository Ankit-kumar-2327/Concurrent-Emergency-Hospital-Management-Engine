# Concurrent Emergency & Hospital Management Engine

A multithreaded Java backend system that simulates emergency hospital resource allocation under concurrent requests. The project demonstrates **thread safety, synchronization, concurrent data structures, and modular object-oriented design**, making it a strong showcase of Java concurrency concepts used in backend systems.

---

## Features

* Thread-safe allocation of hospital beds and medicine inventory
* Concurrent request handling using Java multithreading
* Synchronization using `synchronized` methods and `ConcurrentHashMap`
* Modular service-layer architecture separating business logic from domain models
* Thread management with `ExecutorService` and thread pools
* Custom exception handling for resource allocation failures
* Object-oriented design using inheritance and polymorphism

---

## Project Structure

```text
Concurrent-Emergency-Hospital-Management-Engine/
├── src/
│   ├── model/
│   ├── service/
│   ├── exception/
│   ├── util/
│   └── Main.java
├── README.md
└── .gitignore
```

---

## Tech Stack

* **Java**
* **Multithreading**
* **ExecutorService**
* **ConcurrentHashMap**
* **Synchronization**
* **Object-Oriented Programming (OOP)**

---

## System Workflow

1. A patient request is generated.
2. The allocation service checks bed and medicine availability.
3. Shared resources are protected using synchronization.
4. `ConcurrentHashMap` provides thread-safe access to resource data.
5. `ExecutorService` executes multiple allocation tasks concurrently.
6. Custom exceptions handle allocation failures gracefully.

---

## Concurrency Design

The system prevents race conditions by combining **`synchronized` methods** with **`ConcurrentHashMap`** for shared resource management. Multiple hospital requests are processed in parallel using **`ExecutorService`**, ensuring safe and efficient concurrent execution.

---

## Getting Started

### Prerequisites

* Java 17 or later
* Git

### Clone the Repository

```bash
git clone https://github.com/Ankit-kumar-2327/Concurrent-Emergency-Hospital-Management-Engine.git
cd Concurrent-Emergency-Hospital-Management-Engine
```

### Compile the Project

```bash
javac src/**/*.java
```

### Run the Application

```bash
java src.Main
```

---

## Example Output

```text
[Thread-1] Bed allocated to Patient #101
[Thread-2] Medicine allocated: Paracetamol
[Thread-3] Bed allocation failed: No beds available
[Thread-4] Medicine allocated: Amoxicillin
```

---

## Key Learning Outcomes

* Java multithreading
* Thread synchronization
* Race condition prevention
* Concurrent collections
* ExecutorService and thread pools
* Service-layer architecture
* Exception handling
* OOP design principles

---

## Future Enhancements

* Spring Boot REST API integration
* MySQL/PostgreSQL database persistence
* Real-time monitoring dashboard
* Priority-based emergency scheduling
* JUnit and concurrency testing
* Docker containerization

---

## Author

**Ankit Kumar**

B.Tech, Electronics and Communication Engineering, IIIT Guwahati

* GitHub: https://github.com/Ankit-kumar-2327
* LinkedIn: https://www.linkedin.com/in/your-linkedin-profile

---

If you found this project useful, consider giving it a **star** on GitHub.
