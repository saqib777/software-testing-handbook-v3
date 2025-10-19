
## 22.1 Introduction

In today’s digital world, **security testing** is not a luxury — it’s a necessity.  
A single vulnerability can expose an entire system to **data breaches**, **unauthorized access**, or **financial loss**.  

**Security Testing** ensures that the software:
- Protects data and resources properly.
- Is resilient against attacks.
- Maintains confidentiality, integrity, and availability — the **CIA Triad** of security.

---

## 22.2 What is Security Testing?

Security testing verifies that a software system **guards data and resources** against possible intruders or misuse.  
It aims to find **loopholes and weaknesses** before hackers do.

### Objectives:
- Identify and fix vulnerabilities.
- Ensure user data protection.
- Validate authentication and authorization mechanisms.
- Confirm that encryption and security policies are enforced.

---

## 22.3 Types of Security Testing

| Type | Purpose | Example |
|------|----------|----------|
| **Vulnerability Scanning** | Automatically detect known weaknesses. | Using Nessus to find open ports or weak SSL. |
| **Penetration Testing** | Simulate real attacks to exploit vulnerabilities. | Ethical hacker tries SQL injection on login form. |
| **Security Auditing** | Manual or automated review of code and configurations. | Reviewing access control policies. |
| **Risk Assessment** | Analyze business risks of vulnerabilities. | Evaluating exposure from outdated libraries. |
| **Ethical Hacking** | Authorized simulation of malicious activities. | Testing password strength and session hijacking. |
| **Posture Assessment** | Combination of audits, scans, and penetration tests. | Evaluating overall system readiness. |

---

## 22.4 Key Security Concepts

| Concept | Description |
|----------|--------------|
| **Authentication** | Verifying user identity (e.g., username/password, biometrics). |
| **Authorization** | Determining what actions the user is allowed to perform. |
| **Confidentiality** | Ensuring data is accessible only to authorized users. |
| **Integrity** | Preventing data from being altered or corrupted. |
| **Availability** | Ensuring system uptime and access when needed. |
| **Non-repudiation** | Preventing users from denying their actions. |

---

## 22.5 The CIA Triad

| Element | Meaning | Example |
|----------|----------|----------|
| **Confidentiality** | Protect sensitive data from unauthorized access. | Encrypt passwords in transit and storage. |
| **Integrity** | Ensure information isn’t modified by unauthorized users. | Use digital signatures and checksums. |
| **Availability** | Keep services operational even under attack. | Use load balancers and DDoS protection. |

---

## 22.6 Security Testing Process

1. **Understand the Application**  
   - Identify sensitive data, user roles, and entry points.  

2. **Define Threat Model**  
   - Analyze potential attackers, goals, and techniques (e.g., insider threats, external hackers).  

3. **Plan and Prepare**  
   - Establish test scope, tools, and permissions.  

4. **Perform Vulnerability Scanning**  
   - Use tools to find common vulnerabilities.  

5. **Conduct Penetration Testing**  
   - Attempt to exploit discovered weaknesses manually or via scripts.  

6. **Analyze Results and Report**  
   - Summarize findings, impact, and suggested fixes.  

7. **Implement Fixes and Retest**  
   - Ensure vulnerabilities are patched and secure.

---

## 22.7 Common Security Vulnerabilities

| Vulnerability | Description | Example |
|----------------|--------------|----------|
| **SQL Injection** | Inserting malicious queries into input fields. | `' OR '1'='1` bypassing login validation. |
| **Cross-Site Scripting (XSS)** | Injecting malicious JavaScript into web pages. | `<script>alert('Hacked!')</script>` |
| **Cross-Site Request Forgery (CSRF)** | Forcing users to execute unwanted actions. | Submitting hidden requests while logged in. |
| **Broken Authentication** | Weak login implementation. | Reusing session IDs after logout. |
| **Insecure Direct Object Reference (IDOR)** | Manipulating object references to access restricted data. | Changing `user_id=101` to `user_id=102`. |
| **Sensitive Data Exposure** | Poor encryption or unsecured storage. | Storing passwords in plain text. |
| **Security Misconfiguration** | Default credentials or open ports. | Admin/Admin login left unchanged. |
| **Insufficient Logging and Monitoring** | No tracking of malicious activities. | Attacks go unnoticed due to lack of alerts. |

---

## 22.8 Penetration Testing Lifecycle

1. **Reconnaissance (Information Gathering)**  
   - Collect domain, server, and network info using tools like Nmap or Whois.

2. **Scanning**  
   - Identify open ports, running services, and vulnerabilities.

3. **Exploitation**  
   - Attempt to gain unauthorized access or privileges.

4. **Privilege Escalation**  
   - Try to move from normal to admin-level access.

5. **Post-Exploitation**  
   - Extract sensitive data, test persistence, and create proof of concept.

6. **Reporting**  
   - Summarize findings with risk ratings and recommendations.

---

## 22.9 Common Security Testing Tools

| Tool | Use Case | Description |
|------|-----------|-------------|
| **OWASP ZAP** | Web app security | Detects XSS, SQLi, and more. |
| **Burp Suite** | Penetration testing | Intercepts and manipulates web traffic. |
| **Nmap** | Network scanning | Identifies open ports and services. |
| **Metasploit** | Exploitation framework | Tests vulnerabilities and payloads. |
| **Nikto** | Web vulnerability scanner | Checks for insecure configurations. |
| **Wireshark** | Network protocol analyzer | Monitors live network traffic. |
| **John the Ripper** | Password cracking | Tests password strength. |
| **Acunetix** | Automated web scanning | Comprehensive website security testing. |

---

## 22.10 Example Security Test Scenarios

| Scenario | Expected Behavior | Risk if Failed |
|-----------|------------------|----------------|
| Login form SQL injection | Should reject invalid inputs safely. | Database exposure or login bypass. |
| Password reset function | Should validate identity securely. | Account takeover. |
| Session management | Should expire after logout/inactivity. | Session hijacking. |
| File upload | Should accept only safe file types. | Malicious file upload (e.g., `.exe`). |
| API key exposure | Should hide keys from public access. | Unauthorized API access. |
| HTTPS enforcement | All pages should use HTTPS. | Data interception via MITM attack. |
| Error messages | Should not reveal stack traces. | Information leakage to attackers. |

---

## 22.11 Risk Rating Example

| Risk Level | Description | Example |
|-------------|--------------|----------|
| **Critical** | Immediate risk, system compromise possible. | SQL injection vulnerability in login. |
| **High** | Exploitable but requires some conditions. | Weak password policy. |
| **Medium** | Limited impact or requires specific setup. | Missing security headers. |
| **Low** | Minor issue, negligible impact. | Non-HTTPS image URLs. |

---

## 22.12 Reporting Format Example

**Title:** SQL Injection in Login Form  
**Severity:** Critical  
**Description:** Application does not sanitize input fields properly.  
**Impact:** Database compromise and credential theft possible.  
**Steps to Reproduce:**
1. Go to login page.  
2. Enter `' OR '1'='1` in username field.  
3. Gain unauthorized access.  

**Fix:** Use parameterized queries and input validation.

---

## 22.13 Best Practices

- Implement input validation and sanitization.  
- Use strong authentication (2FA, OAuth).  
- Encrypt data in transit (TLS/SSL) and at rest (AES).  
- Rotate and protect API keys and secrets.  
- Apply principle of least privilege (POLP).  
- Regularly update dependencies and patches.  
- Run security scans before every major release.  
- Log all access attempts and monitor anomalies.  

---

## 22.14 OWASP Top 10 (2021)

| Rank | Category | Description |
|------|-----------|-------------|
| A01 | Broken Access Control | Users can access unauthorized data. |
| A02 | Cryptographic Failures | Weak or missing encryption. |
| A03 | Injection | SQL, OS, LDAP injections. |
| A04 | Insecure Design | Flawed security architecture. |
| A05 | Security Misconfiguration | Default credentials, open ports. |
| A06 | Vulnerable Components | Outdated libraries. |
| A07 | Identification and Authentication Failures | Weak login or session management. |
| A08 | Software and Data Integrity Failures | Unverified updates or dependencies. |
| A09 | Security Logging and Monitoring Failures | Missing activity tracking. |
| A10 | Server-Side Request Forgery (SSRF) | External resource access exploited. |

---

## 22.15 End Notes

Security is not a one-time test — it’s a **continuous process**.  
Every line of code, every configuration, and every release can introduce new risks.  

> “Security testing isn’t about finding flaws —  
> it’s about building trust in every interaction your system has.”

---

