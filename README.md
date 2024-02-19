# TCP Server for String Reversal

This is a simple TCP server written in Java that allows multiple clients to connect simultaneously and reverses strings sent by clients. The server limits the maximum number of clients to 10 and introduces a delay using `Thread.sleep()` to simulate processing.

## Usage

### Prerequisites

- Java Development Kit (JDK) installed on your system.

### Running the Server

1. Compile the Java source code:

    ```bash
    javac TCPServer.java
    ```

2. Run the server:

    ```bash
    java TCPServer
    ```

3. The server will start listening on port 12345 by default.

### Connecting Clients

You can connect clients to the server using any TCP client application. Here's an example of connecting using Telnet:

```bash
telnet localhost 12345
```
3. Sending Strings
Once connected, you can send strings to the server. The server will reverse each string and send the reversed string back to the client. A delay of 1 second is introduced for processing each string.

4. Exiting
To exit the server, simply terminate the process.

5. Customization
You can customize the server port by modifying the PORT constant in the TCPServer class.
Adjust the maximum number of clients allowed by changing the MAX_CLIENTS constant in the TCPServer class.
Modify the processing delay by changing the argument of Thread.sleep() in the ClientHandler class.
