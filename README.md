# Task 2: Security Alert Monitoring & Incident Response

👨‍💻 Intern: Shahid Hasan  
🧠 Task Code: FUTURE_CS_02  
🛠️ Tools: Splunk Enterprise, access.log

---

## Objective

To identify suspicious activity and potential attacks from server logs using Splunk and document incident responses.

---

## Incidents Detected

### 1. SQL Injection Attempt

- **IP Address:** 10.0.0.5  
- **Payload:** `' OR '1'='1`  
- **Status Code:** 403  
- **Risk Level:** High  
- **Mitigation:** Use parameterized queries and input validation

---

### 2. Reflected XSS Attack

- **IP Address:** 192.168.1.105  
- **Payload:** `<script>alert(1)</script>`  
- **Status Code:** 200  
- **Risk Level:** Critical  
- **Mitigation:** Sanitize output, use CSP headers

---

### 3. Brute Force Login Attempts

- **IP Address:** 203.0.113.25, 10.0.0.5  
- **Endpoint:** `/admin/login`  
- **Status Codes:** 401, 404, 500  
- **Risk Level:** Medium  
- **Mitigation:** Implement rate limiting, IP blocklist, MFA

---

## 📄 Full Report

Read the detailed task report here: [`task2_report.pdf`](task2final.pdf)

---

## Screenshots

Located in `/screenshots/`:
- `sql_injection_detected.png`
- `xss_detected.png`
- `brute_force_attempts.png`

---

## Conclusion

Splunk enabled quick identification of critical web app vulnerabilities. This simulation helped strengthen my skills in log forensics, incident triage, and security response.
