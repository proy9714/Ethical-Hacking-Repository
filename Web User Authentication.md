## Sessions vs Cookies vs Tokens

| Aspect         | Sessions                                | Cookies                               | Tokens                          |
| -------------- | --------------------------------------- | ------------------------------------- | ------------------------------- |
| **Storage**    | Server-side                             | Client-side                           | Client-side                     |
| **Usage**      | User session management, authentication | User session tracking, preferences    | Authentication, authorization   |
| **Security**   | More secure (data stored server-side)   | Less secure (vulnerable to theft)     | Secure (can be encrypted)       |
| **Expiration** | Can expire based on session settings    | Can have expiration times             | Can have short expiration times |
| **Scope**      | Application-wide                        | Domain-wide                           | Application-wide or domain-wide |
| **Data Size**  | Can handle larger data                  | Limited data size (around 4KB)        | Can handle larger data          |
| **Examples**   | User authentication, session management | Storing session IDs, user preferences | JWTs for API authentication     |

**Sessions**:
- Stored server-side, used for managing user sessions and authentication.
- More secure but requires server resources for storage and management.

**Cookies**:
- Stored client-side, used for session IDs, preferences, and tracking.
- Less secure due to vulnerabilities like theft or tampering.

**Tokens**:
- Stored client-side, used for authentication and authorization.
- Secure, can have short expiration times, suitable for API authentication.

---
## Cookies vs Local Storage vs Session Storage

| Aspect             | Cookies                                 | Local Storage                  | Session Storage               |
| ------------------ | --------------------------------------- | ------------------------------ | ----------------------------- |
| **Scope**          | Domain-wide                             | Domain-wide                    | Tab/Window-specific           |
| **Lifespan**       | Can have expiration times               | Persists after browser closure | Cleared on tab/window closure |
| **Storage Limit**  | Limited (usually around 4KB per cookie) | Larger (up to 5MB per domain)  | Moderate (browser-specific)   |
| **Automatic Send** | Sent with every HTTP request            | Not sent automatically         | Not sent automatically        |
| **Usage**          | User sessions, preferences, tracking    | Offline caching, user settings | Temporary session data        |
| **Security**       | Vulnerable to theft, XSS attacks        | Safer for sensitive data       | Safer for temporary data      |

**Cookies**:
- Used for session IDs, user authentication, preferences.
- Limited storage, vulnerable to security risks.

**Local Storage**:
- Ideal for larger data storage, persists across sessions.
- Not sent automatically with requests, shared across tabs.

**Session Storage**:
- Used for temporary session data, cleared on tab closure.
- Scoped to the current tab or window, safer for transient data.

---
## LINKS

![Session vs Token Authentication in 100 Seconds (Fireship)](https://www.youtube.com/watch?v=UBUNrFtufWo)

- **Fantastic** and succinct explanation of Cookie Sessions vs JWT. 
- Advantages and drawbacks of each.

---
## 🔗 [[Json Web Tokens (JWT)]]