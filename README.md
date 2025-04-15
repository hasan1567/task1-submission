# Task 1 – Security Assessment Report (DVWA)

## 🔍 Objective
To analyze a mock vulnerable application (DVWA) and identify common web vulnerabilities using both manual and automated methods.

## 🧪 Environment
- Kali Linux (VMware)
- DVWA (http://localhost/DVWA)
- OWASP ZAP
- Firefox (Developer Tools)

## 🛠️ Tools Used
- OWASP ZAP (vulnerability scanner)
- DVWA (Damn Vulnerable Web Application)
- MariaDB, Apache2

## ✅ Steps Performed
1. Installed and configured DVWA on Kali Linux
2. Set security level to **Low**
3. Launched OWASP ZAP and ran an automated scan on `http://localhost/DVWA`
4. Manually tested:
   - SQL Injection (`' OR 1=1 --`)
   - XSS (`<script>alert('XSS')</script>`)
5. Exported scan report and captured key screenshots

## 📂 Files Included
- `DVWA_scan_2025-04-12.html` – ZAP HTML scan report
- `task1_report.txt` – Summary of findings
- `work 1.PNG` to `work 9.PNG` – Screenshots of scanning and testing process

## 🔒 Key Findings
- SQL Injection in `vulnerabilities/sqli`
- Stored XSS in `vulnerabilities/xss_stored`
- Weak input sanitization
- Security headers missing (until Helmet was applied later)

## 📌 Conclusion
Basic vulnerability assessment successfully completed. Common flaws were identified and documented. Screenshots and reports are included for review.

---
