#fundamentals #flashcards/fundamentals

[HTTP/1.1](https://en.wikipedia.org/wiki/HTTP) is a text based protocol that works over TCP.

HTTP works because plain text _is_ binary. Because HTTP uses TCP, if the HTTP request or response is too big to fit into a single TCP packet it can be broken up into many packets and reconstructed in the correct order on the other side. **TCP guarantees that the data is in order and complete**.

At the heart of HTTP is the `HTTP-message`: the format that the text in an HTTP request or response must use. From [RFC 9112 Section 2.1](https://datatracker.ietf.org/doc/html/rfc9112#name-message-format):

```
start-line CRLF
*( field-line CRLF )
CRLF
[ message-body ]
```

_[`CRLF`](https://developer.mozilla.org/en-US/docs/Glossary/CRLF) (written in plain text as `\r\n`) is a carriage return followed by a line feed. It's a Microsoft Windows (and HTTP) style newline character_.

Primagen: I call `\r\n` "Registered Nurse"... it helps me remember the order of the characters

Let's break down each part:

|Part|Example|Description|
|---|---|---|
|`start-line CRLF`|`POST /users/primeagen HTTP/1.1`|The request (for a request) or status (for a response) line|
|`*( field-line CRLF )`|`Host: google.com`|Zero or more lines of HTTP headers. These are key-value pairs.|
|`CRLF`||A blank line that separates the headers from the body.|
|`[ message-body ]`|`{"name": "TheHTTPagen"}`|The body of the message. This is optional.|

Both HTTP requests and responses follow this same format, though the contents of each section will differ.

Data is transmitted unencrypted. Encryption can be added with [TLS](https://de.wikipedia.org/wiki/Transport_Layer_Security) -> HTTP/S

---
## Questions
Explain HTTP::The [hypertext transfer protocol](https://de.wikipedia.org/wiki/Hypertext_Transfer_Protocol) is a stateless protocol which is designed to transfer information between networked devices.