# Voting System Project
Overview
This voting system project allows users to vote for candidates through a client-server architecture. The client sends the vote data to the server, which validates and stores the vote, ensuring that each voter can only vote once.

Core Features
Client-Side:

Connect to the server and send serialized vote data.

Display the result of the vote (success or failure).

Server-Side:

Listen for incoming client connections.

Deserialize the vote data and check if the voter has already voted.

Store the vote and send an appropriate response to the client.

Serialization:

Simple string-based serialization and deserialization of vote data.

Technologies Used
C++

Winsock2 library for networking (Windows platform)

Threads for handling multiple clients simultaneously

Project Progress
Client-Side Implementation
Socket Connection: Client connects to the server using TCP/IP.

Serialization: Votes are serialized into a string format for transmission.

Error Handling: Errors in the voting process are communicated back to the user.

Server Response: The client handles responses such as success or failure messages.

Server-Side Implementation
Socket Setup: Server listens for client connections on a specified port.

Vote Validation: Server checks if a voter has already voted using a registry.

Threading: The server handles multiple clients concurrently using threads.

Vote Recording: Successfully records votes in memory.

3. Configuration
Ensure both server and client are using the same IP and port.

Modify PORT and SERVER_ADDRESS if necessary.
