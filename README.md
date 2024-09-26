# Computer Networking Projects

This repository contains various computer networking projects demonstrating core concepts in network communication, socket programming, and protocols.

## Table of Contents

- [Project 1: Socket Programming](#project-1-socket-programming)
- [Project 2: Socket Programming Applications](#project-2-socket-programming-applications)
- [Project 3: Routing Protocols and Network Simulations](#project-3-routing-protocols-and-network-simulations)
- [Project 4: Implementation of Load Balancer and Airport Security Screening Simulation](#project-4-implementation-of-load-balancer-and-airport-security-screening-simulation)
- [Getting Started](#getting-started)
- [Technologies Used](#technologies-used)

## Project 1: [Socket Programming](https://github.com/TanmayB2003/computer-networking/tree/main/socket-programming)
This project implements various networking applications using C/C++ socket programming. The project comprises three major tasks:
1. [Concurrent Base64 Encoding with TCP Sockets](https://github.com/TanmayB2003/computer-networking/tree/main/socket-programming/q1_concurrent-communication)
2. [Simple Chat Server](https://github.com/TanmayB2003/computer-networking/tree/main/socket-programming/q2_chat-server)
3. Network Calculator using [TCP](https://github.com/TanmayB2003/computer-networking/tree/main/socket-programming/q3_tcp) and [UDP](https://github.com/TanmayB2003/computer-networking/tree/main/socket-programming/q3_udp)

### Features:
1. **Concurrent Base64 Encoding Communication (TCP)**:
   - Implement a server that handles multiple clients concurrently using TCP sockets.
   - Clients send Base64-encoded messages to the server.
   - Server decodes the messages, prints them, and sends an acknowledgment back to the clients.
   - Clients can send multiple messages and gracefully close the connection.

2. **Simple Chat Server (TCP)**:
   - Server binds to an IP address and port, accepting multiple client connections.
   - Handles communication between clients and the server in a simple chat mechanism.
   - Clients send messages to the server, which broadcasts them to other clients.
   - Implements graceful exit for both client and server applications.

3. **Network Calculator (TCP/UDP)**:
   - Implements both TCP and UDP client-server applications for a network calculator.
   - Clients send arithmetic expressions to the server.
   - The server evaluates and returns the result to the client.
   - Supports basic operations (+, -, *, /, ^) and handles negative/decimal numbers.
   - Provides error handling and debugging features.
   
4. **Error Handling and Robustness**:
   - Ensures error handling for invalid inputs, missing arguments, and unexpected disconnections.
   - Each task includes handling different network issues and ensuring the stability of communication.

## Project 2: [Socket Programming Applications](https://github.com/TanmayB2003/computer-networking/tree/main/app-using-socket)
This project implements four networking applications using socket programming in C/C++:
1. [DNS Lookup Tool](https://github.com/TanmayB2003/computer-networking/tree/main/app-using-socket/Question_1_dns-lookup)
2. [HTTP Web Cache](https://github.com/TanmayB2003/computer-networking/tree/main/app-using-socket/Question_2_http-lru-cache)
3. [Client-Client Chat Server (TCP Protocol)](https://github.com/TanmayB2003/computer-networking/tree/main/app-using-socket/Question_3_chat-server-tcp)
4. [Wireshark Analysis](https://github.com/TanmayB2003/computer-networking/tree/main/app-using-socket/Question_4_wireshark-analysis)

### Features:
1. **DNS Lookup Tool (UDP)**:
   - Takes a domain name as input.
   - Sends a DNS query to Google's DNS server (8.8.8.8).
   - Parses the response and displays the IP address.
   - Implements caching for frequent domain lookups.

2. **HTTP Web Cache (LRU)**:
   - Stores up to 5 web pages fetched via HTTP GET requests.
   - Uses a Least Recently Used (LRU) eviction policy.
   - Implemented using sockets and a linked list to track page accesses.

3. **Client-Client Chat Application (TCP)**:
   - Supports multiple clients (minimum 10) connected to a chat server.
   - Allows client-to-client message exchange (broadcast or private messages).
   - Implements graceful exit for both clients and the server.

5. **Wireshark Traffic Analysis**:
   - Captures and analyzes network traffic (DNS, HTTP, TCP/UDP) using Wireshark.
   - Documents protocol details, handshaking sequences, and caching mechanisms.
   - Provides statistics such as throughput, RTT, and packet loss under different conditions.

## Project 3: [Routing Protocols and Network Simulations](https://github.com/TanmayB2003/computer-networking/tree/main/routing-protocols)
This project involves implementing key network communication concepts using C/C++. It consists of three tasks:
1. [Simplified OSPF Routing Protocol](https://github.com/TanmayB2003/computer-networking/tree/main/routing-protocols/q1_ospf)
2. [Simplified MAC Layer Simulation (CSMA/CA Protocol)](https://github.com/TanmayB2003/computer-networking/tree/main/routing-protocols/q2_mac-layer)
3. [Stop-and-Wait Flow Control Protocol](https://github.com/TanmayB2003/computer-networking/tree/main/routing-protocols/q3_stop-and-wait-flow)

### Features:
**1. OSPF Routing Protocol Implementation:**
   - **Router Class**: 
     - Unique router identification.
     - Neighboring routers represented as pointers.
     - Routing table for storing routing information.
   - **Routing Methods**: 
     - Add neighboring routers dynamically.
     - Compute and update routing tables using Dijkstra’s algorithm.
     - Display routing tables for each router.
   - **Network Simulation**: 
     - Create and connect a network of routers.
     - Simulate packet routing based on the routing table.

**2. MAC Layer Simulation**
   - **CSMA/CA Protocol**: 
     - Simulates behavior of nodes in a wireless network.
     - Configurable number of nodes and shared communication channel.
   - **Backoff Mechanism**: 
     - Nodes select random backoff intervals before attempting transmission.
   - **Collision Detection**: 
     - Mechanism for detecting simultaneous transmissions and handling collisions.
   - **Statistics Tracking**: 
     - Records successful transmissions, collisions, and backoff attempts.

**3. Stop-and-Wait Flow Control Protocol**
   - **Flow Control Implementation**: 
     - Implements the Stop-and-Wait protocol for data transmission control in a network. 

## Project 4: [Implementation of Load Balancer and Airport Security Screening Simulation](https://github.com/TanmayB2003/computer-networking/tree/main/queueing_algo)
This project involves implementing two main applications using socket programming in C/C++:
1. [Weighted Fair Queuing (WFQ) Implementation](https://github.com/TanmayB2003/computer-networking/tree/main/queueing_algo/q1_wfq)
2. [Airport Security Screening Simulation](https://github.com/TanmayB2003/computer-networking/tree/main/queueing_algo/q2_airport-security)

### Features
1. **WFQ Load Balancer Implementation**:
   - **Website Class**: Represents websites with unique IDs, owners, and request queues.
   - **HttpRequest Class**: Models incoming HTTP requests with unique IDs, website IDs, and processing times.
   - **LoadBalancer Class**: Manages requests and implements the WFQ algorithm with methods to add websites, enqueue requests, and dequeue requests based on WFQ scheduling.
   - **Test Cases**: Multiple scenarios to validate functionality, including:
     - Equal and differential resource allocation.
     - Stress testing with large request volumes.
     - Handling empty queues and edge cases.

2. **Airport Security Screening Simulation**:
   - **Simulation Setup**: Models a security screening process as a queuing system with an initial single security line.
   - **User-Defined Parameters**: Allows specification of arrival rate (λ) and service rate (μ) for passenger processing.
   - **Data Collection**: Collects statistics on average waiting time, queue length, and system utilization.
   - **Queue Length Optimization**: Incorporates a finite buffer for waiting passengers and assesses its impact.
   - **Multi-Server Expansion**: Simulates scenarios with multiple security lines and scanners.
   - **Buffered Multi-Server Model**: Adds a buffer for multiple scanners, allowing authorities to set buffer sizes.
   - **Analysis and Reporting**: Evaluates the efficiency of security screening processes and documents findings and optimization strategies.

## Getting Started

### Prerequisites
- **C/C++ Compiler**:
  - GCC (GNU Compiler Collection) for Linux and macOS.
  - MinGW (Minimalist GNU for Windows) for Windows.
- **Socket Programming Libraries**:
   - Ensure the following libraries are available for socket programming:
     - `<sys/socket.h>`: For socket functions.
     - `<netinet/in.h>`: For Internet address family.
     - `<arpa/inet.h>`: For functions related to Internet addresses.
     - `<unistd.h>`: For Unix standard functions (like `close()`).

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/TanmayB2003/computer-networking.git
   cd computer-networking
   ```

2. Run the projects as described in their respective directories.

## Technologies Used
- **C/C++**: Core programming language
- **Socket Programming**: For network communication
- **Multi-threading**: To handle concurrent client requests
