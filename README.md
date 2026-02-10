# Week 6 – Advanced Security Audit & Secure Deployment

**Project:** Juice Shop Security Enhancement  
**Author:** Muhammad Ali Kashif  
**Week:** 6  
**Date:** February 2026

## 📌 Overview

This repository contains all deliverables for Week 6 of the Cybersecurity Internship. The focus was advanced security audits, compliance checks, secure deployment, and penetration testing to ensure the Juice Shop application is robust and secure.

## 🛠 Tools & Technologies

- OWASP ZAP – Web application vulnerability scanning
- Nikto – Web server security scanning
- Lynis – System security auditing
- Trivy – Container & dependency vulnerability scanning
- Burp Suite – Manual penetration testing
- Docker – Secure container deployment
- Node.js / Express – Application backend

## 🔒 Security Audits & Compliance

| Tool | Purpose | Key Findings |
|------|---------|--------------|
| OWASP ZAP | Web vulnerability scanning | Detected cross-site scripting, weak headers |
| Nikto | Web server scanning | Found outdated server components |
| Lynis | System & configuration audit | Identified missing security configurations |
| Trivy | Container & dependency scanning | Found HIGH & CRITICAL vulnerabilities in libraries |

**OWASP Top 10 Compliance Checklist:**
- ✔ Injection – SQLi testing completed
- ✔ Broken Authentication – Session & token review
- ✔ Security Misconfiguration – Server & container scans
- ✔ Vulnerable Components – CVE detection & recommendations applied
- ✔ Sensitive Data Exposure – HTTPS and JWT verified

## 🛠 Secure Deployment Practices

**Docker Security:**
- Minimal base images used
- Containers scanned regularly with Trivy
- No processes run as root

**Automatic Updates & Dependency Scanning:**
- Node.js and OS dependencies updated
- Vulnerable libraries patched
- Regular update scripts enabled

## 🕵️ Final Penetration Testing

Manual penetration testing via Burp Suite:
- Tested login, input forms, and session management
- Documented vulnerabilities mitigated
- JWT and private key handling secured

**Key Results:**
- 23 vulnerabilities detected (1 CRITICAL, 3 HIGH, 7 MEDIUM, 12 LOW)
- High-risk secrets removed
- Application ready for secure deployment