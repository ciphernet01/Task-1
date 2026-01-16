# Cyber Security Basics & Attack Surface Report

**Author:** SHREYANSH SINGH 
**Date:** 15 January 2026 
**Task:** Understanding Cyber Security Basics & Attack Surface

---

## 1. Introduction to Cyber Security

Cyber security refers to the practice of protecting systems, networks, programs, and data from digital attacks, damage, or unauthorized access. It involves a set of technologies, processes, and practices designed to safeguard digital assets and ensure the continuity of operations in the face of evolving threats.

---

## 2. The CIA Triad

The CIA triad is a fundamental model in cyber security, representing the three core principles of information security:

### **Confidentiality**
- **Definition:** Ensuring that information is accessible only to those authorized to have access.
- **Real-World Example:** Banking applications use encryption to protect user credentials and transaction data from being intercepted by unauthorized parties.

### **Integrity**
- **Definition:** Maintaining and assuring the accuracy and completeness of data over its entire lifecycle.
- **Real-World Example:** Digital signatures in email systems verify that the message has not been altered during transmission.

### **Availability**
- **Definition:** Ensuring that information and resources are accessible to authorized users when needed.
- **Real-World Example:** Social media platforms employ load balancers and redundant servers to handle high traffic and prevent downtime during peak usage.

---

## 3. Types of Cyber Attackers

Cyber attackers vary in motivation, skill level, and resources:

| Attacker Type         | Description                                                                 | Example                          |
|-----------------------|-----------------------------------------------------------------------------|----------------------------------|
| **Script Kiddies**    | Inexperienced individuals using pre-built tools to launch attacks.          | Using automated tools for DDoS.  |
| **Insiders**          | Employees, contractors, or partners who misuse access to harm the organization. | Disgruntled employee leaking data. |
| **Hacktivists**       | Attackers motivated by political, social, or ideological causes.            | Groups like Anonymous.           |
| **Nation-State Actors** | Government-sponsored hackers targeting other nations for espionage or disruption. | APT groups (e.g., APT28).        |

---

## 4. Attack Surface Overview

An attack surface refers to all the points where an unauthorized user can try to enter or extract data from a system. Common attack surfaces include:

### **Web Applications**
- Login pages, contact forms, search fields.
- **Example Vulnerability:** SQL injection in a login form.

### **Mobile Applications**
- Insecure data storage, weak authentication mechanisms.
- **Example Vulnerability:** Storing sensitive data in plain text on a device.

### **APIs (Application Programming Interfaces)**
- Unauthorized access, insecure endpoints.
- **Example Vulnerability:** Exposing user data through an unprotected API endpoint.

### **Networks**
- Unsecured Wi-Fi, phishing emails, malware.
- **Example Vulnerability:** Man-in-the-middle attack on a public Wi-Fi network.

### **Cloud Infrastructure**
- Misconfigured storage buckets, weak identity and access management (IAM).
- **Example Vulnerability:** Publicly accessible Amazon S3 bucket containing sensitive data.

---

## 5. OWASP Top 10 – Critical Web Application Security Risks

The OWASP Top 10 is a standard awareness document for developers and security professionals. It lists the most critical security risks to web applications.

| Risk Category                     | Description                                                                 |
|-----------------------------------|-----------------------------------------------------------------------------|
| **Broken Access Control**         | Restrictions on authenticated users are not properly enforced.              |
| **Cryptographic Failures**        | Sensitive data is exposed due to weak or missing encryption.                |
| **Injection**                     | Malicious data is sent to an interpreter (e.g., SQL, OS commands).          |
| **Insecure Design**               | Security flaws in the architecture or design of the application.            |
| **Security Misconfiguration**     | Default configurations, unnecessary features, or exposed ports.             |
| **Vulnerable Components**         | Using outdated or vulnerable third-party libraries or frameworks.           |
| **Authentication Failures**       | Weak passwords, session fixation, or broken authentication logic.           |
| **Software/Data Integrity Failures** | Unsigned code, compromised updates, or insecure CI/CD pipelines.         |
| **Security Logging & Monitoring Failures** | Inadequate logging, monitoring, and incident response.                 |
| **Server-Side Request Forgery (SSRF)** | Attackers trick the server into making requests to internal resources. |

---

## 6. Mapping Daily Applications to Attack Surfaces

| Daily Application | Attack Surface Example                                  | Potential Threat                            |
|-------------------|---------------------------------------------------------|---------------------------------------------|
| **Email**         | Phishing links, malicious attachments, spoofed senders. | Credential theft, malware infection.        |
| **WhatsApp**      | End-to-end encryption flaws, backup storage.           | Unauthorized message access, data leakage.  |
| **Banking App**   | Man-in-the-middle attacks, session hijacking.          | Financial fraud, identity theft.            |
| **Social Media**  | Third-party app permissions, malicious ads.             | Data harvesting, account takeover.          |

---

## 7. Data Flow and Attack Points

Understanding how data moves through a system helps identify where attacks can occur:
