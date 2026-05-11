# Fraud Detection Based System

A real-time fraud detection system developed using Spring Boot, Apache Kafka, and Machine Learning.

The project processes transaction events through Kafka and uses an AI-based fraud detection model to classify transactions as fraudulent or safe.

---

## Features

- Real-time transaction processing
- Kafka-based event streaming
- Fraud prediction using Machine Learning
- Producer-Consumer architecture
- Spring Boot REST APIs
- TensorFlow model integration

---

## Technologies Used

- Java
- Spring Boot
- Apache Kafka
- Python
- TensorFlow
- Maven

---

## System Architecture

The system contains:

1. Producer Application  
   Sends transaction events to Kafka topics.

2. Kafka Broker  
   Handles event streaming between applications.

3. Consumer Application  
   Consumes transactions and performs fraud detection using the ML model.

---

## How to Run

### Start Zookeeper

```bash
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
```

### Start Kafka

```bash
.\bin\windows\kafka-server-start.bat .\config\server.properties
```

### Run Producer Application

```bash
mvn spring-boot:run
```

### Run Consumer Application

```bash
mvn spring-boot:run
```

---

## Test API

```bash
curl -X POST "http://localhost:8087/send-transaction?amount=5000"
```

---

## Project Modules

- fraud-detection-producer
- fraud-detection-consumer
- TensorFlow ML Model



## Developed By

Sruthi Shakhamuri
