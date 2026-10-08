# Secure TCP/IP Multi-Client Chat Application

**Python | TCP/IP | Socket Programming | Multithreading | Client-Server Architecture | wxPython**

## Project Overview

Secure TCP/IP Multi-Client Chat Application is a collaborative networking project developed to enable multiple users to communicate through a centralized chat server.

The application uses Python socket programming and TCP/IP communication to establish client-server connections, exchange messages, manage active user sessions, and support file sharing through a graphical user interface.

The project demonstrates fundamental computer networking concepts, including socket creation, IP addressing, port binding, connection establishment, concurrent client communication, and session termination.

**Project Type:** Academic Team Project  
**Year:** 2022–2023  
**Domain:** Computer Networking and Network Security

## Technologies Used

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Networking Protocol | TCP/IP |
| Network Communication | Socket Programming |
| Architecture | Client-Server |
| Concurrency | Multithreading |
| Graphical Interface | wxPython |
| Development Environment | PyCharm |
| Security Concepts | Symmetric Encryption |

## System Architecture

The application follows a centralized client-server architecture.


### Detailed Network Architecture

Explore the TCP/IP client-server architecture, connection
establishment process, and message communication workflow.

**[View Network Architecture and Communication Diagrams](docs/architecture.md)**


**Client A ↔ TCP/IP ↔ Central Chat Server ↔ TCP/IP ↔ Client B**

Additional clients can connect to the same server to participate in group communication.

### Server Responsibilities

- Bind to a designated host IP address and port.
- Listen for incoming TCP connection requests.
- Accept client connections.
- Manage connected clients using threads.
- Maintain information about active users.
- Relay messages between connected clients.
- Handle connection and disconnection events.

### Client Responsibilities

- Initialize a TCP socket.
- Connect to the server using its IP address and port.
- Send and receive messages.
- Participate in group conversations.
- Use nicknames for identification.
- Transfer files within the supported size limit.
- Disconnect from the server when finished.

## Key Features

### 1. Multi-Client Communication

The system supports communication between multiple clients connected to a centralized TCP server.

### 2. TCP Socket Programming

The application demonstrates socket-based connection establishment, network data exchange, and connection termination.

### 3. Multithreading

Multithreading supports concurrent communication and helps the server handle connected client operations.

### 4. Graphical User Interface

The chat interface uses wxPython to provide an interactive environment for sending messages, managing conversations, and connecting to the server.

### 5. Group Messaging

Connected clients can exchange messages through the central chat server.

### 6. Nickname Management

Users can identify themselves with nicknames instead of communicating through raw IP addresses.

### 7. File Transfer

The documented implementation supports file transfers up to **1 MB**. Files exceeding the limit trigger an error.

### 8. Client Session Management

The application supports client connection, active communication, and disconnection from the server.

## TCP/IP Communication Workflow

1. The server creates a TCP socket.
2. The server binds the socket to an IP address and port.
3. The server begins listening for incoming connections.
4. A client initializes its socket and establishes a connection.
5. The server accepts the incoming connection.
6. Client and server threads handle communication.
7. Messages are routed through the server to connected clients.
8. Users can exchange messages and files.
9. Clients terminate their sessions using the disconnect functionality.

## Network Security Considerations

The project documentation discusses symmetric encryption as a mechanism for protecting message confidentiality.

The exact encryption algorithm, key-management process, and end-to-end security properties have not yet been independently verified from the original source code.

Therefore, this repository presents the application as an academic networking and secure-messaging project rather than a production-ready encrypted communication platform.

## Demonstrated Results

The academic project documentation includes screenshots demonstrating:

- Server and client initialization.
- Connection between two clients and the chat server.
- Group-chat communication.
- Nickname assignment.
- Message and file transfer.
- File-size restriction.
- Be-right-back functionality.
- Client disconnection.

The documented tests demonstrate core communication and file-sharing functionality. They do not establish large-scale performance, production reliability, or a formal security audit.

## Technical Challenges

The project focused on several networking and application-design challenges:

- Establishing reliable TCP connections between clients and server.
- Supporting concurrent client communication.
- Routing messages to connected participants.
- Managing user connection and disconnection events.
- Integrating file-sharing functionality.
- Applying message confidentiality concepts.

## Project Documentation

The original academic material includes:

- Phase I project report.
- Phase II implementation report.
- Architecture and data-flow diagrams.
- Client and server execution screenshots.
- Graphical user-interface screenshots.
- Functional test results.

Supporting documentation and selected screenshots will be added to this repository.

## Source Code Availability

This repository currently serves as an engineering case study based on the academic project documentation.

The original runnable Python source files have not yet been uploaded. Implementation and installation instructions will be added after the source files are recovered or the application is reconstructed and tested.

## Team Collaboration

This application was developed collaboratively as an academic engineering project.

**Contributor:** Priyanka Sridhar and project teammates.

The project involved client-server networking, application design, graphical user-interface development, and functional testing.

## Key Networking Concepts Demonstrated

- TCP/IP communication
- IPv4 addressing and ports
- Client-server architecture
- Socket programming
- Connection establishment and termination
- Multithreading
- Data transmission
- Multi-client session management
- Network application troubleshooting

## Future Improvements

Potential future enhancements include:

- Recovering and publishing the original Python source code.
- Documenting and verifying the encryption implementation.
- Capturing TCP traffic using Wireshark.
- Adding automated connection and transfer tests.
- Improving connection-error handling.
- Documenting deployment and reproducible setup instructions.
- Adding screenshots and a detailed architecture diagram.

---

**Maintained by Priyanka Sridhar**

[GitHub Profile](https://github.com/PriyankaSridhar17) | [Network Engineering Portfolio](https://priyankasridhar17.github.io/priyanka-network-portfolio/)# secure-tcp-chat
TCP/IP multi-client chat application using Python socket programming, multithreading, GUI communication, and file transfer.

---

## Project Demonstration & Screenshots

The following screenshots are taken from the academic project's implementation and testing.

### Group Chat Application Interface
![Application Screenshot 1](screenshots/image%201.png)

### TCP/IP Client-Server Connection Establishment
![Client-Server Connection](screenshots/image%202.png)

### Client Nickname Assignment and User Identification
![Nickname Management](screenshots/image%203.png)

### Real-Time Messaging and File Transfer
![Message and File Transfer](screenshots/image%204.png)

### File Transfer Size Validation (1 MB Limit)
![File Size Validation](screenshots/image%205.png)

###  Client Disconnection and Session Termination
![Client Disconnection](screenshots/image%206.png)
