#TCP Client Application (C++ / Winsock2)

This is a simple **TCP client** built using the **Winsock2 API** in C++. It connects to a TCP server, receives an initial message, and then enters a loop where it sends and receives messages (echo style).

---

## Features:

- TCP connection with IPv4 using Winsock2
- Receives welcome message from the server
- Interactive user prompt for sending messages
- Graceful exit with `"exit"` or `"EXIT"`

---

##  How It Works:

1. Initializes Winsock2 (version 2.2)
2. Creates a TCP socket
3. Connects to the server at the provided IP and port
4. Receives a welcome message
5. Enters a loop:
   - Takes user input
   - Sends it to the server
   - Waits for an echo response
6. Cleans up on `"exit"`

---

## Requirements:

- Windows OS
- C++ Compiler with Winsock support (MSVC or MinGW)
- A TCP server running at the specified IP and port

---

##  Configuration:

Edit these constants in the source code to match your server:
```cpp
#define SERVER_IP "127.0.0.1"  // Replace with your server IP
#define SERVER_PORT 0000       // Replace with your server port
