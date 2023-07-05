# Socket.io

## Web Sockets

### 1.What is a Web Socket?

WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection.

### 2.Describe the Web Socket request/response handshake and what happens once the connection is established.

The WebSocket protocol enables interaction between a web browser (or other client application) and a web server with lower overhead than half-duplex alternatives such as HTTP polling, facilitating real-time data transfer from and to the server. This is made possible by providing a standardized way for the server to send content to the client without being first requested by the client, and allowing messages to be passed back and forth while keeping the connection open. In this way, a two-way ongoing conversation can take place between the client and the server. 

### 3.Web Sockets provide a standardized way for the server to send content to a client without first receiving a ____ from that client.

request

## Socket.io Tutorial

### 1.What does the event handler io.on() do?

The io.on event handler handles connection, disconnection, etc., events in it, using the socket object.

### 2.Describe some possible proof of life or proof that the code works as expected

We set up the server to log messages on connections and disconnections.an we include the client script and initialize the socket object there, so that clients can establish connections when required. The script is served by our io server at '/socket.io/socket.io.js'. If you go to localhost:3000 now (make sure your server is running), you will get Hello World printed in your browser.

### 3.What does socket.emit() do?

socket.emit function can create and fire custom events.

## Socket.io vs Web Sockets

### 1.What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).

WebSocket is the communication Protocol that provides bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer. When clients trigger the request to the server, it does not close the connection on receiving the response; it rather persists and waits for the Client or server to terminate the request.

Socket.IO is a library that enables real-time and full-duplex communication between the Client and the Web servers. It uses the WebSocket protocol to provide the interface. Generally, it is divided into two parts; both WebSocket vs Socket.io are event-driven libraries.

### 2.When would you use Socket.IO?

.I handle all the degradation of your technical alternatives to get full-duplex communication in real-time.

.It also handles the various support level and the inconsistencies from the browser.

.It also gives the additional feature room support for basic publish infrastructure and thinks like automatic reconnect.

.Currently, AFAIK is the most used one and easier to help with vanilla web sockets.

### 3.When would you use WebSockets?

.It provides full-duplex communication, which helps in persisting the connection established between the Client and the Web Server.

.It also lives up to the standards and provides the accuracy and efficiency stream events to and from with negligible latency.

.WebSocket removes the overhead and reduce complexity.

.It makes real-time communication effortless and efficient.

## OSI Model Explained

### What are a couple of key takeaways from this video?

.OSI model is basically a way of letting two different computers or networks communicate with each other.

.OSI model consists of 7 layers: application, presentation, session, transport, network, datalink, physical.

.each layer uses a certain protocol.

.each layer handles certain jobs which are handles using their specific protocols.

## TCP Handshakes Explained

### Translate the gist of this video to a non-technical friend.

Basically, a handshake is a way of establishing a connection between a client and a server, it starts by the client sending a request to the server asking to connect, then the server replys with an aknlowledgment, then it sends back a request for client asking for a connection, after, the client responds with another request saying yes basically.