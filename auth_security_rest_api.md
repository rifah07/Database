# Auth & Security for REST APIs: Introduction and Questions

## Introduction to Authentication and Security in REST APIs

API authentication and security are vital for protecting resources and data when exposing services over the web. REST APIs, being stateless and data-rich, are often targeted for unauthorized access and attacks. Modern REST API security relies on robust authentication (verifying user identity), authorization (controlling user permissions), encrypted data transfer, and continuous monitoring.

Common authentication strategies include:
- **Basic Authentication**: Username and password sent with each request (insecure without HTTPS).
- **API Keys**: Unique tokens issued to users for access, often via headers (should be rotated frequently).
- **Token-Based Authentication (JWT)**: Encodes user identity and claims in a secure, compact token.
- **OAuth 2.0**: Delegated access using third-party providers, ideal for SSO and complex scenarios.

Best practices:
- Always use HTTPS/TLS for encrypted communication.
- Rotate and invalidate tokens and API keys regularly.
- Implement rate limiting and centralized secret management.
- Use strong password policies and secure password storage (hashed).
- Employ multi-factor authentication (MFA) for critical APIs.

## Common Auth & Security Questions and Answers

1. **What is the difference between authentication and authorization?**  
   Authentication verifies *who* the user is; authorization determines *what* they can access.

2. **Describe token-based authentication in REST APIs.**  
   Token-based authentication generates a secure token (like JWT) after a successful login, which is then sent with each API request to authenticate the user.

3. **How do API keys work and what are their limitations?**  
   API keys are unique tokens given to users; included in the header of each request. They are easy to implement but less secure than tokens if keys are exposed or mismanaged.

4. **Explain OAuth 2.0 and its role in REST API security.**  
   OAuth 2.0 enables delegated access without sharing passwords, letting users log in with providers (Google, Facebook) and granting token-based, scoped access for third parties.

5. **What is JWT and why is it popular?**  
   JWT (JSON Web Token) is a compact, URL-safe token with header, payload, and signature. It allows stateless authentication, custom claims, and is easy to validate.

6. **Why should HTTPS always be used for APIs?**  
   HTTPS encrypts data in transit, protecting credentials, tokens, and sensitive payloads from interception and man-in-the-middle attacks.

7. **What are some REST API security best practices?**  
   - Use HTTPS/TLS only  
   - Rotate keys/tokens  
   - Set token short expiration and support refresh  
   - Employ rate limiting  
   - Avoid hardcoded secrets in source code  
   - Centralize secret management

8. **How do you secure sensitive API endpoints?**  
   Require strong authentication, role-based access control, and rate limiting. Use scopes/permissions and monitor access logs for anomalies.

9. **What is multi-factor authentication (MFA) and why use it in APIs?**  
   MFA requires two or more independent credentials (e.g., password + OTP), adding an extra security layer against credential compromise.

10. **How can you revoke or invalidate user tokens or API keys?**  
    Maintain a blacklist of tokens/keys, implement expiration and rotation policies, and monitor usage for suspicious activity.

---
