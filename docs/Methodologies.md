# 🔍 Methodologies Used in Vulnerability Assessment

This document outlines the methodologies followed during the penetration testing of the OWASP Juice Shop application.

---

## 🔐 Assessment Type
- **Black Box Testing**
  - No access to internal code
  - Simulates real-world external attacker

## 🧪 Testing Approach

### 1. Reconnaissance
- Enumerated public files (`robots.txt`, `main.js`)
- Discovered hidden paths using Dirb/Gobuster

### 2. Vulnerability Scanning
- Automated scans via **OWASP ZAP**
- Verified issues manually to reduce false positives

### 3. Manual Testing Techniques
- **SQL Injection (SQLi)**: Used payloads like `' OR '1'='1' --` to bypass login
- **Cross-Site Scripting (XSS)**: Injected scripts into feedback fields
- **Broken Access Control**: Attempted actions reserved for admin users
- **Insecure Direct Object Reference (IDOR)**: Modified URL parameters to access other users’ data
- **Information Disclosure**: Located sensitive data like password hashes and routes in JS files
- **Cross-Site Request Forgery (CSRF)**: Simulated via forged POST requests
- **Business Logic Abuse**: Repeated interactions to receive multiple discount codes

### 4. Risk Analysis
- Categorized vulnerabilities into Critical, High, Medium, Low, and Informational
- Prioritized based on impact and likelihood

### 5. Documentation & Reporting
- Recorded evidence of vulnerabilities
- Provided mitigation strategies and CWE references
- Prepared report using screenshots and technical details

---

## 🧠 Standards and Guides Followed

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [OWASP Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [OWASP ASVS](https://owasp.org/www-project-application-security-verification-standard/)
- [PTES – Penetration Testing Execution Standard](https://www.pentest-standard.org/)
- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)

---

## 🧑‍💻 Target Environment

- **Application URL**: `http://localhost:3000/`
- **Assessment Period**: 01/03/2025 – 30/04/2025
- **Platform**: OWASP Juice Shop (Angular + Node.js + SQLite)
- **Host OS**: Kali Linux
- **Browser**: Firefox
