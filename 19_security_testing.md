# 19.1 Introduction

------

Modern applications handle sensitive information like user credentials, payments, and personal data.  
**Security testing** ensures that this information remains protected from threats such as hacking, data theft, or misuse.

It verifies that the system:
- Guards against unauthorized access.  
- Protects data in storage and transmission.  
- Handles attacks gracefully without revealing internal details.

---

## 19.2 What is Security Testing?

**Definition:**  
Security Testing is a process of identifying vulnerabilities and ensuring the system’s data and resources are protected from potential intruders.

It aims to answer:
- Is user data safe?  
- Can attackers exploit system weaknesses?  
- Does the system handle invalid or malicious inputs properly?

---

## 19.3 Objectives of Security Testing

- Identify potential security risks and vulnerabilities.  
- Prevent unauthorized access and data breaches.  
- Ensure compliance with security standards (e.g., OWASP, ISO 27001).  
- Verify proper encryption, authentication, and authorization.  
- Build user trust and protect brand reputation.

---

## 19.4 Key Areas of Security Testing

| Area | Description |
|------|--------------|
| **Authentication** | Verifies user identity (e.g., username & password). |
| **Authorization** | Ensures users can only access what they’re permitted to. |
| **Confidentiality** | Keeps data private through encryption. |
| **Integrity** | Ensures data isn’t altered or corrupted. |
| **Non-repudiation** | Ensures actions can’t be denied later (e.g., digital signatures). |
| **Availability** | Ensures system remains available under attack or heavy use. |

---

## 19.5 Common Security Threats

| Threat | Description | Example |
|--------|--------------|---------|
| **SQL Injection** | Attackers inject malicious SQL code to access data. | `' OR 1=1; --` |
| **Cross-Site Scripting (XSS)** | Inserting scripts in web pages viewed by others. | `<script>alert('Hacked!')</script>` |
| **Cross-Site Request Forgery (CSRF)** | Forces a user to perform unwanted actions. | Auto-submitting hidden forms. |
| **Session Hijacking** | Stealing or manipulating session tokens. | Cookie theft. |
| **Brute Force Attack** | Repeatedly trying passwords until one works. | Password guessing. |
| **Denial of Service (DoS)** | Overloading system resources to make it unavailable. | Sending millions of requests per second. |
| **Data Leakage** | Sensitive information exposed unintentionally. | API responses exposing emails or keys. |

---

## 19.6 Types of Security Testing

| Type | Description | Example |
|------|--------------|---------|
| **Vulnerability Scanning** | Automated tools scan for known vulnerabilities. | Using Nessus or OpenVAS. |
| **Penetration Testing (Ethical Hacking)** | Simulates real attacks to find weaknesses. | Attempting unauthorized access. |
| **Security Auditing** | Manual review of code and configurations. | Reviewing API security headers. |
| **Risk Assessment** | Identifies and prioritizes potential risks. | High-risk: data exposure in APIs. |
| **Ethical Hacking** | Authorized hacking to uncover system flaws. | Red team exercises. |
| **Posture Assessment** | Combined review of vulnerabilities, risks, and audits. | Full system security overview. |

---

## 19.7 Security Testing Process

1. **Identify Security Goals**  
   Define what needs protection (e.g., data, authentication system).

2. **Threat Modeling**  
   Identify potential attack vectors (e.g., SQL injection, brute force).

3. **Test Planning**  
   Choose tools, define test scope, and decide testing type (manual or automated).

4. **Execution**  
   Perform penetration testing, vulnerability scans, and code reviews.

5. **Reporting**  
   Document vulnerabilities, severity, and recommendations.

6. **Fix and Retest**  
   Apply patches, harden configurations, and validate fixes.

---

## 19.8 Security Testing Tools

| Tool | Category | Description |
|------|-----------|-------------|
| **Burp Suite** | Penetration Testing | Widely used for web app security testing. |
| **OWASP ZAP** | Open-source Scanner | Detects vulnerabilities like XSS, SQLi. |
| **Nmap** | Network Scanner | Finds open ports and services. |
| **Nessus** | Vulnerability Scanner | Scans for known CVEs and risks. |
| **Metasploit** | Exploitation Framework | Tests and validates security weaknesses. |
| **Wireshark** | Packet Analyzer | Monitors and analyzes network traffic. |

---

## 19.9 OWASP Top 10 Security Risks (Latest Overview)

1. Broken Access Control  
2. Cryptographic Failures  
3. Injection Attacks  
4. Insecure Design  
5. Security Misconfiguration  
6. Vulnerable Components  
7. Identification and Authentication Failures  
8. Software and Data Integrity Failures  
9. Security Logging and Monitoring Failures  
10. Server-Side Request Forgery (SSRF)

---

## 19.10 Example Scenario

**Example: Banking Application Login Security Test**

| Step | Description |
|------|--------------|
| 1 | Try SQL Injection on login: `' OR '1'='1` |
| 2 | Try brute force password attempts. |
| 3 | Attempt to bypass 2FA (Two-Factor Authentication). |
| 4 | Check if error messages reveal system info. |
| 5 | Validate secure HTTPS connection and cookie encryption. |

**Goal:**  
Ensure login system blocks attacks, encrypts data, and prevents unauthorized access.

---

## 19.11 Security Testing Best Practices

- Follow **OWASP Guidelines**.  
- Use **HTTPS** with valid certificates.  
- Enforce **strong password policies**.  
- Implement **input validation and sanitization**.  
- Regularly **update dependencies** and apply patches.  
- Conduct **security testing early and continuously**.  
- Log and monitor suspicious activities.  
- Limit access using **least privilege principle**.  

---

## 19.12 Benefits of Security Testing

✅ Protects user data and organizational reputation.  
✅ Prevents financial and legal consequences.  
✅ Ensures compliance with GDPR, ISO, HIPAA, etc.  
✅ Builds customer confidence.  
✅ Reduces long-term security costs.

---

## 19.13 Limitations

⚠️ Cannot guarantee 100% security.  
⚠️ Requires specialized expertise.  
⚠️ May not detect zero-day vulnerabilities.  
⚠️ Time-consuming for large systems.  

---

## 19.14 Summary

Security Testing ensures that an application remains **confidential**, **integral**, and **available**, even under attack.  
By simulating real-world hacking attempts, testers identify weak points before malicious users can exploit them.

---

## 19.15 End Notes

> “Security is not a one-time process — it’s an ongoing commitment.”  
> The goal isn’t just to protect systems, but to **protect trust**.

---

