#fundamentals

The [hypertext transfer protocol](https://de.wikipedia.org/wiki/Hypertext_Transfer_Protocol) is a stateless protocol which is designed to transfer information between networked devices.

## HTTP Request
A Request contains:
- a [URL](https://de.wikipedia.org/wiki/Uniform_Resource_Locator) to locate the server and the resource to query
- [Header](https://de.wikipedia.org/wiki/Liste_der_HTTP-Headerfelder) are Key-Value pairs with meta information
- Optional Request Body with data

## HTTP Methods
The HTTP method tells the server what the client wants to do with the data. Common examples include GET and POST.

## HTTP Response
The Response contains:
- HTTP status code represent the outcome of an HTTP request (range from 1xx to 5xx)
- Header are Key-Value pairs with meta information
- Optional Response Body 

Data is transmitted unencrypted. Encryption can be added with [TLS](https://de.wikipedia.org/wiki/Transport_Layer_Security) -> HTTP/S