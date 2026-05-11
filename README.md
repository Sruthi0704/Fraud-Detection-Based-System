# Fraud Detection Based System

A real-time fraud detection system developed using Spring Boot, Apache Kafka, and Machine Learning.

This project processes transaction events through Kafka and uses an AI-based fraud detection model to classify transactions as fraudulent or safe.

---

# Features

- Real-time transaction processing
- Kafka-based event streaming
- Fraud prediction using Machine Learning
- Producer-Consumer architecture
- REST API integration using Spring Boot
- TensorFlow model integration
- Scalable distributed system design

---

# Technologies Used

- Java
- Spring Boot
- Apache Kafka
- Python
- TensorFlow
- Maven
- REST APIs

---

# Project Architecture

The system consists of three major components:

## 1. Producer Application
- Sends transaction events to Kafka topics.
- Built using Spring Boot REST APIs.

## 2. Kafka Broker
- Handles real-time event streaming between applications.

## 3. Consumer Application
- Consumes transaction events from Kafka.
- Uses the trained Machine Learning model to classify fraud transactions.

---

# Project Structure

```text
Fraud-Detection-Based-System/
│
├── fraud-detection-producer/
├── fraud-detection-consumer/
├── serving/
├── images/
├── fraud_detection_model.ipynb
└── README.md
```

---

# Prerequisites

Before running the project, install:

- Java 17+
- Python 3.7+
- Apache Kafka
- Maven
- TensorFlow

---

# How to Run the Project

## Step 1: Start Zookeeper

```bash
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
```

## Step 2: Start Kafka Server

```bash
.\bin\windows\kafka-server-start.bat .\config\server.properties
```

## Step 3: Run Producer Application

```bash
cd fraud-detection-producer
mvn spring-boot:run
```

## Step 4: Run Consumer Application

```bash
cd fraud-detection-consumer
mvn spring-boot:run
```

---

# Machine Learning Model

The fraud detection model was trained using Python and TensorFlow.

The model:
- preprocesses transaction data
- predicts fraudulent transactions
- integrates with the Spring Boot consumer service

---



Example Output:
- Transaction sent to Kafka
- Fraud prediction generated successfully

---



# Future Improvements

- Real-time dashboard visualization
- Advanced fraud analytics
- Cloud deployment support
- Enhanced ML model accuracy
- Docker and Kubernetes integration

---

# Learning Outcomes

Through this project, I gained experience in:
- Event-driven architecture
- Apache Kafka integration
- Spring Boot microservices
- Machine Learning deployment
- Real-time transaction processing

---

# Developed By

Sruthi Shakhamuri
