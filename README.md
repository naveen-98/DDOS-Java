# DDOS-Java

## Overview

**DDOS-Java** is a Java-based simulation of a Distributed Denial of Service (DDoS) attack. The code demonstrates how such an attack can be implemented in a simple way. This project is designed for educational purposes to help understand the mechanics of DDoS attacks and should not be used for malicious purposes.

## Features

- Simulates a basic DDoS attack using multithreading.
- Sends multiple HTTP GET requests to a specified target URL.
- Demonstrates the principles of overloading a target server with excessive requests.

## Educational Purpose

This project serves to illustrate how a DDoS attack works and how malicious actors might exploit such techniques. By studying this simulation, developers and security professionals can better understand how to defend against such attacks.

## How It Works

1. The code creates multiple threads (2,000 by default).
2. Each thread sends continuous HTTP GET requests to the specified target URL.
3. The target server may become overwhelmed due to the high volume of requests.

### Code Structure

- **`DdosAttack`**: The main class that initializes and starts multiple threads for the attack.
- **`DdosThread`**: A thread class responsible for sending requests to the target URL in a loop.
- **HTTP Requests**: Each thread uses `HttpURLConnection` to send requests with headers resembling a browser.

## Prerequisites

- Java Development Kit (JDK) installed.
- Basic knowledge of Java programming and multithreading.
- A test environment (never use this code on unauthorized targets).

## Usage

1. Clone this repository:
   ```bash
   git clone <repository-url>
   ```
2. Open the project in your preferred Java IDE or editor.
3. Modify the target URL in the `DdosThread` class (default: `https://www.hackthissite.org`).
4. Compile and run the program:
   ```bash
   javac DdosAttack.java
   java DdosAttack
   ```

## Important Notes

- Use this project only for educational purposes and in a controlled environment.
- Testing DDoS attacks without permission is illegal and unethical.
- The author does not take responsibility for any misuse of this code.

## Author

- **N4VIYA98 (Naveen Wijesinghe)**

## License

This project is licensed for educational use only. Unauthorized or malicious use is strictly prohibited.
