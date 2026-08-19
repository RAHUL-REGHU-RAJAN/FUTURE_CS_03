# API Security Assessment

> **Future Interns — Cyber Security Internship | Task 3**

A practical API security testing project using **Postman** and the **JSONPlaceholder public test API**. The assessment focuses on reviewing API endpoints, inspecting responses, and documenting basic security observations.

## 🔎 About the Project

APIs are a key part of modern web applications and can expose important information if they are not properly secured.

For this task, selected JSONPlaceholder endpoints were tested using read-only `GET` requests. The returned data and HTTP responses were reviewed from an API-security perspective.

This project is intended for **learning and practical security assessment**, not for attacking a production system.

## 🎯 Objectives

- Test selected REST API endpoints.
- Inspect HTTP status codes and JSON responses.
- Review the information exposed by API responses.
- Understand authentication and authorization considerations.
- Identify areas that would require stronger controls in a production API.
- Document the testing process and supporting evidence.

## 🌐 Target

**API:** JSONPlaceholder

**Base URL:**
```text
https://jsonplaceholder.typicode.com
```

JSONPlaceholder is a public mock API used for development, testing, and learning.

## 🧪 Endpoints Tested

| Method | Endpoint | Purpose |
|---|---|---|
| GET | `/users` | Retrieve user information |
| GET | `/posts` | Retrieve post information |
| GET | `/comments` | Retrieve comment information |

### Example Request

```http
GET https://jsonplaceholder.typicode.com/users
```

The tested endpoints returned **HTTP 200 OK** responses.

## 🛠️ Tools

- **Postman** — API requests and response inspection
- **Browser Developer Tools** — additional request/response inspection
- **GitHub** — project documentation and submission

## 🔬 Testing Approach

The assessment was kept simple and non-intrusive:

```text
Select Endpoint
      ↓
Send GET Request
      ↓
Check Response
      ↓
Inspect JSON Data
      ↓
Review Security Considerations
      ↓
Document Findings
```

The review mainly considered:

- Endpoint accessibility
- Returned information
- HTTP status codes
- Authentication requirements
- Data exposure
- General API security controls

## 📸 Evidence

The repository contains Postman evidence for the three endpoints tested:

- `GET Users`
- `GET Posts`
- `GET Comments`

The screenshots show the request URL, HTTP response status, headers, and returned JSON data.

## 📊 Security Observations

The assessment identified areas that should be considered when designing a production API:

### Public Endpoint Access
The selected JSONPlaceholder endpoints can be accessed without an authentication token. This is expected because the service is a public testing API.

For a production API containing private information, sensitive endpoints should require appropriate authentication and authorization.

### Data Exposure
The `/users` response contains multiple user-related fields, while `/comments` includes fields such as names and email addresses.

For a real application, APIs should return only the information required by the client.

### Production Controls

A production API should consider:

- Authentication
- Authorization
- Rate limiting
- Input validation
- Data minimization
- HTTPS
- Logging and monitoring

> **Note:** These observations are made in the context of API security learning. JSONPlaceholder is intentionally a mock API, so its public behavior should not automatically be classified as a vulnerability.

## 📁 Repository Structure

```text
API-Security-Assessment/
│
├── README.md
├── Report/
│   └── API_Security_Risk_Analysis_Report.docx
│
└── Evidence/
    ├── GET_Users.png
    ├── GET_Posts.png
    └── GET_Comments.png
```

## 🛡️ Scope

### Included
- Public JSONPlaceholder API
- Read-only GET requests
- Response inspection
- Basic API security review
- Documentation and evidence collection

### Not Included
- Authentication bypass
- Credential attacks
- Destructive testing
- DoS/flooding
- Unauthorized systems
- Data modification or exfiltration

## 🧠 Skills Demonstrated

**API Testing • Postman • REST APIs • HTTP • JSON Analysis • API Security • Data Exposure Review • Security Documentation**

## 📄 Deliverables

- API Security Assessment Report
- Postman testing evidence
- README documentation

## ⚠️ Disclaimer

This project was performed against a public mock API for educational purposes. No unauthorized access, destructive testing, denial-of-service activity, or data exfiltration was performed.

---

**Rahul**  
*Cybersecurity | Ethical Hacking | Security Analysis*

**Future Interns — Task 03**
