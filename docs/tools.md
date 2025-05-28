# 🛠 Tools Used for Vulnerability Assessment

This document lists and describes the tools employed during the vulnerability assessment of the OWASP Juice Shop application.

---

## 1. OWASP ZAP (Zed Attack Proxy)
- **Purpose**: Automated vulnerability scanning
- **Functions**:
  - Spidering web pages
  - Active/passive scans
  - Fuzzing and input manipulation

## 2. Burp Suite (Community Edition)
- **Purpose**: Manual testing and attack simulation
- **Functions**:
  - Proxy to intercept and modify HTTP/HTTPS traffic
  - Repeater, Intruder, and Decoder tools

## 3. Nikto
- **Purpose**: Web server scanning
- **Functions**:
  - Detects outdated software
  - Identifies insecure headers and files

## 4. Nmap *(optional)*
- **Purpose**: Network scanning
- **Functions**:
  - Port and service discovery
  - OS fingerprinting and script scanning

## 5. Dirb / Gobuster
- **Purpose**: Hidden file and directory enumeration
- **Functions**:
  - Brute-force paths based on wordlists
  - Discover admin panels, configuration files, etc.

## 6. Browser Developer Tools (Firefox)
- **Purpose**: Client-side inspection
- **Functions**:
  - Analyzing source code and JavaScript
  - Monitoring network requests
