# Interface-Assignment
Interface Assignment
You are tasked with designing a system to handle various types of network connections in a distributed computing environment. Each type of connection (HTTP, FTP, and WebSocket) supports different sets of operations.

Create four interfaces:

Connectable with a connect() method.
Disconnectable with a disconnect() method.
Sendable with a send(String message) method.
Receivable with a receive() method.
Create three classes:

HTTPConnection implements Connectable, Disconnectable, Sendable, and Receivable.
FTPConnection implements Connectable, Disconnectable, and Sendable.
WebSocketConnection implements Connectable, Disconnectable, Sendable, and Receivable.
You must design a NetworkManager class that manages an array of different connection types (HTTP, FTP, WebSocket). The NetworkManager should:

Establish connections for all connectable types.
Send a message to all sendable types.
Receive messages from all receivable types.
Disconnect all disconnectable types.
Description:
Challenge:

The NetworkManager must handle the connections dynamically, based purely on the interfaces each connection type implements.
You cannot use instanceof or type-checking operations. The solution must leverage the interfaces to invoke the appropriate methods polymorphically.
Additional Requirement: You may need to ensure that messages sent through WebSocket are always received. Thus, WebSocket connections must guarantee that the receive() method is called after every send() operation without external checks.

Assignment Criteries
1. Business Logic
2. Implementation
3. Coding Standards
4. Code Modularity
