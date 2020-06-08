# Alchemy Reading Notes
## Class 06

### HTTP
- Hyper Text Transfer Protocol (HTTP) is a stateless request-response application layer protocol. 
-  HTTP is used to build distributed, collaborative, hypermedia information systems. HTTP is the foundation for the world wide web.
- It is a client-server model; host designed to provide a service is called a server. Clients are hosts that make requests to that service.

### HTTP Requests
- A HTTP/1.1 request is formatted in text and transferred using TCP. The first line of the request contains the METHOD, URL, and HTTP VERSION. The following lines are the request HEADERS.
- Some request methods:
    - GET
    - HEAD
    - POST
    - PUT
    - DELETE
    - CONNECT
    - OPTIONS
    - TRACE
    - PATCH

### REST

- REST is acronym for REpresentational State Transfer.
- That means we can reference, manipulate, and transfer state.
- Generally speaking, RESTful endpoints deliver data in JSON format. The best practice is to supply a header with metadata and a collection of results

#### Rest Documentation
- The standard for documenting REST APIs is with a “live” documentation system: Open API (formerly “Swagger”)
