# REST API Introduction

## Introduction to REST API

REST (Representational State Transfer) API is a web service architecture that uses standard HTTP methods to perform operations on resources identified by URIs (Uniform Resource Identifiers). RESTful APIs follow principles such as statelessness (each request contains all info to be processed), client-server separation, cacheability, uniform interface, and layered systems.

Common HTTP methods used in REST are:
- **GET**: Retrieve data from a resource
- **POST**: Create a new resource
- **PUT**: Update an existing resource
- **PATCH**: Partially update a resource
- **DELETE**: Remove a resource

Data is typically exchanged in JSON format. REST APIs provide a consistent and predictable interface for clients to interact with server-side data.

## Common REST API Questions and Answers

1. **What is REST?**  
   REST is an architectural style for designing networked applications using stateless, client-server communication, typically over HTTP with standard methods for CRUD operations on resources.

2. **What are the main HTTP methods used in REST?**  
   GET, POST, PUT, PATCH, DELETE.

3. **What does stateless mean in REST?**  
   Each request from client to server must contain all the information needed to understand and process the request. The server does not store any client context between requests.

4. **What status codes are commonly used in REST API?**  
   - `200 OK`: Successful request  
   - `201 Created`: Resource created successfully  
   - `400 Bad Request`: Invalid input or malformed request  
   - `401 Unauthorized`: Authentication failed  
   - `404 Not Found`: Resource not found  
   - `500 Internal Server Error`: Server-side error

5. **Explain the difference between PUT and PATCH.**  
   PUT updates the entire resource; PATCH applies partial updates to a resource.

6. **What is a resource in REST?**  
   A resource is an object or representation of something which can be manipulated via the API, and is identified by a URI.

7. **What data format is commonly used in REST APIs?**  
   JSON (JavaScript Object Notation) is the most common due to its lightweight and human-readable format.

8. **What is HATEOAS?**  
   Hypermedia As The Engine Of Application State (HATEOAS). It’s a REST constraint where responses include links to other related resources/actions, allowing dynamic navigation of the API.

9. **How do you secure a REST API?**  
   Common methods include using API keys, OAuth, JWT (JSON Web Tokens), and HTTPS to secure data transmission.

10. **Can you give an example of a simple GET request?**  
    ```
    GET /api/users HTTP/1.1
    Host: example.com
    Authorization: Bearer <token>
    ```
    This fetches a list of users from the server.

---

This document provides a clear and concise explanation of REST API fundamentals along with practical interview questions and answers to help prepare for technical discussions on REST APIs.
