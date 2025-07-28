# khalidbankapplication

This is a secure banking application built using Spring Boot and Spring Security, focusing on real-world authentication, authorization, and API protection best practices. It showcases stateless JWT-based authentication, custom filters, and complete security event handling.

## 🚀 Key Features

- **JWT Authentication**: Stateless login flow with secure token generation and validation.
- **Custom Authentication Provider**: Validates user credentials using Spring Security's authentication flow.
- **Password Security**: Integrated with HaveIBeenPwned API to check for compromised passwords.
- **Role-Based Access Control**: API access managed via roles (`USER`, `ADMIN`) and authorities.
- **Custom Filters**:
  - Request validation filter
  - CSRF token cookie filter
  - Logging filters (before/after/at)
  - JWT token generator and validator
- **CSRF & CORS Protection**:
  - CSRF tokens stored in cookies
  - CORS configured for frontend (e.g., `localhost:4200`)
- **Custom Exception Handling**:
  - Returns JSON responses for `401 Unauthorized` and `403 Forbidden` errors
  - Headers like `eazybank-error-reason` and `eazybank-denied-reason` included
- **Database**:
  - Uses MySQL
  - Managed via SQLectron
- **Containerized**: Application is Dockerized for consistent deployment.
- **API Testing**: All endpoints tested using Postman.

## 🛠️ Technologies Used

- Java 17  
- Spring Boot 3.x  
- Spring Security 6.x  
- JWT (Java Web Token)  
- MySQL  
- Docker  
- SQLectron  
- Postman  
