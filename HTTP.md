#fundamentals

The [hypertext transfer protocol](https://de.wikipedia.org/wiki/Hypertext_Transfer_Protocol) is a stateless protocol which is designed to transfer information between networked devices.

## HTTP Request
A Request contains:
- a [URL](https://de.wikipedia.org/wiki/Uniform_Resource_Locator) + [URI](https://de.wikipedia.org/wiki/Uniform_Resource_Identifier) to locate the server and resource it wants to query
- [Header](https://de.wikipedia.org/wiki/Liste_der_HTTP-Headerfelder) as Key-Value pairs with meta information
- Optional Request Body with data transmitted to the server

## HTTP Methods
The HTTP method tells the server what the client wants to do with the data. Common examples include GET and POST.

## HTTP Response
The Response contains:
- HTTP status which indicates if the operation was successfully (range from 1xx to 5xx)
- Header as Key-Value pairs with meta information
- Optional Response Body with data transmitted to the client

Data is transmitted unencrypted. Encryption is added with [TLS](https://de.wikipedia.org/wiki/Transport_Layer_Security) -> HTTP/S