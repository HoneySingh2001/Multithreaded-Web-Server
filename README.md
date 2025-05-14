# 🌐 Multithreaded Web Server in Java

A lightweight, high-performance web server built from scratch in Java that efficiently handles concurrent client requests using thread pools.

## 🧩 Problem Statement

Traditional single-threaded servers struggle to handle multiple simultaneous client requests, leading to slow response times or dropped connections under heavy traffic.

## ✅ Solution

This project implements a multithreaded web server using a thread pool mechanism to handle client connections concurrently and efficiently, improving throughput and responsiveness.

## 🚀 Features

- ⚙️ Multithreaded request handling with thread pool executor
- 📄 Basic HTTP GET request support (serves static files like HTML, CSS, JS)
- 📦 Customizable server root directory
- ⏱️ Graceful shutdown and error handling
- 📈 Scalable design for concurrent clients

## 🔧 Technologies Used

- 💻 **Java (Core)**
- 📚 Java I/O, Sockets, Threads, Executors

## 📁 Project Structure

multithreaded-web-server/
├── src/
│ ├── MainServer.java # Starts the server, accepts connections
│ ├── ClientHandler.java # Handles client requests
│ ├── ThreadPoolManager.java # Manages the thread pool
├── public/ # Static files served by the server
├── README.md

## ⚙️ How It Works

1. Server socket listens on a configurable port.
2. Each incoming client request is handled by a `ClientHandler` task.
3. A fixed-size thread pool processes requests in parallel.
4. HTTP responses are returned for supported GET requests.

## 🧪 How to Run

### Prerequisites:
- Java 8 or above

