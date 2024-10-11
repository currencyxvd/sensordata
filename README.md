# Sensor Data Processing System

This project demonstrates a multithreaded Java application for processing data from various sensors using an event queue and thread pool. The system efficiently handles sensor data by utilizing multiple worker threads that process the incoming data in parallel.

## Features

- **Multithreading**: Utilizes Java's `ExecutorService` to handle multiple threads for concurrent processing.
- **Event Queue**: Uses a `BlockingQueue` to synchronize and manage sensor data events.
- **Scalable**: The number of threads can be configured based on the system's capability.
- **Real-time Processing**: Processes sensor data in real-time with minimal delay.

## Project Structure

- **`SensorData`**: Represents the data from a sensor, including the sensor ID, value, and timestamp.
- **`SensorProcessor`**: A worker thread that processes data taken from the event queue.
- **`SensorSystem`**: The main class that manages the event queue, creates sensor events, and assigns them to worker threads for processing.

## Getting Started

### Prerequisites

You need the following to build and run this project:

- Java 11 or later
- Maven (for dependency management and building)

### Build and Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/sensor-data-processing.git
   cd sensor-data-processing
