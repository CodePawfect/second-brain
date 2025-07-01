#fundamentals #flashcards/fundamentals 

What is a protocol?::A protocol is a set of rules and standards that define how information is exchanged between devices and systems.

What is a port?::Ports are numeric identifiers used by transport layer protocols like TCP and UDP to distinguish between multiple applications or services on the same device. They ensure that incoming data is delivered to the correct application.

What is a socket?::A socket is an endpoint for communication, defined by an IP address, a port number, and a transport protocol (typically TCP or UDP). Sockets are used by applications to establish network connections and exchange data.

How websockets work?
?
A websocket connections start off as a HTTP request. If both sides agree through HTTP Headers, they switch to websocket mode on the same TCP connection.

Client:
```
GET /chat HTTP/1.1
Host: example.com
Upgrade: websocket
Connection: Upgrade
Sec-WebSocket-Key: ...
```

Server:
```
HTTP/1.1 101 Switching Protocols
Upgrade: websocket
Connection: Upgrade
Sec-WebSocket-Accept: ...
```

From then on, they exchange messages wrapped in a frame that tells each side how to interpret the data.
+++

What is the difference between read from a file and read from a network connection?
?
When you read from a **file**, you're in control of the reading process. You decide:

- When to read
- How much to read
- When to stop reading.
- You pull data from the file.

When you read from a **network connection**, the data is **pushed** to you by the remote server. You don't have control over when the data arrives, how much arrives, or when it stops arriving. Your code has to be ready to receive it when it comes.
+++

What is Hypertext?
?
Hypertext is text which is not constrained to be linear.
Hypertext is text which contains **links** to other texts. 

HyperMedia is a term used for hypertext which is not constrained to be text: it can include graphics, video and sound , for example.
+++
