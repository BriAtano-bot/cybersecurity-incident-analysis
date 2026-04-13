notes/http-https-fundamentals.md# HTTP & HTTPS Fundamentals

## 🌐 Overview
HTTP (HyperText Transfer Protocol) is the protocol used for communication between clients (browsers) and web servers.

HTTPS is the secure version of HTTP, using encryption (TLS/SSL) to protect data in transit.

---

## 🔄 HTTP Request & Response

### Request
A client sends a request to a server:
- Method (GET, POST, etc.)
- URL
- Headers
- Body (optional)

### Response
The server replies with:
- Status code
- Headers
- Body (content)

---

## 📊 Common HTTP Methods

- GET → Retrieve data
- POST → Send data (e.g., login)
- PUT → Update data
- DELETE → Remove data

---

## 📈 HTTP Status Codes

### 🟢 2xx (Success)
- 200 OK → Request successful

### 🟡 4xx (Client Errors)
- 401 Unauthorized → Authentication required
- 403 Forbidden → Access denied

### 🔴 5xx (Server Errors)
- 500 Internal Server Error

---

## 🔐 HTTP vs HTTPS

| Feature    | HTTP | HTTPS |
|------------|------|-------|
| Encryption |  No  | Yes   |
| Security   | Low  | High  |
| Port       | 80   | 443   |

---

## 🔍 Security Importance

HTTPS protects:
- Credentials (usernames/passwords)
- Sensitive data
- Prevents man-in-the-middle attacks

---

## 🧠 SOC Perspective

From a SOC Analyst perspective:

- Monitor repeated POST /login requests → possible brute force attack
- Analyze status codes (401, 403, 200) to detect suspicious behavior
- Identify unusual access patterns (e.g., access to /admin or /dashboard)

---

## 🚨 Example Attack Pattern

POST /login → 401  
POST /login → 401  
POST /login → 200  
GET /dashboard → 200  

This may indicate a successful brute force attack.

---

## 🛠️ Tools Used

- curl (manual requests)
- browser developer tools
- log analysis (access.log)

---

## 📌 Conclusion

Understanding HTTP/HTTPS is essential for:
- analyzing web traffic
- detecting attacks
- performing incident investigations
