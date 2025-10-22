# FUTURE_CS_02 - Security Alert Monitoring & Incident Response

This repository documents a cybersecurity intern-led SOC analysis performed on sample log data using **Elastic Stack (Kibana, Elasticsearch, Logstash)**. The analysis focuses on **threat detection, incident response, and remediation**, aligned with OWASP Top 10.

---

## 🛠️ Tools Used
- **Elastic Stack** (Kibana, Elasticsearch, Logstash) running on **Windows via Opera Browser**  
- **Sample Log Files**  

---

## 📊 Key Features
- Real-time log analysis via **Kibana Discover**  
- Detection of malware (**Trojan, Rootkit, Spyware, Worm, Ransomware**)  
- Login failure tracking and brute-force detection  
- Connection attempt monitoring  
- Alert severity classification  

---

## 📅 Incident Timeline

| Timestamp       | User    | IP Address     | Action           | Threat                  | Severity |
|-----------------|---------|---------------|-----------------|------------------------|----------|
| 2025-07-03 05:48:14 | bob     | 10.0.0.5      | malware detected | Trojan Detected         | High     |
| 2025-07-03 08:42:14 | bob     | 203.0.103.77  | malware detected | Worm Infection          | High     |
| 2025-07-03 04:46:14 | bob     | 172.16.0.3    | malware detected | Ransomware Behavior     | High     |
| 2025-07-03 04:19:14 | alice   | 198.51.100.42 | malware detected | Rootkit Signature       | High     |
| 2025-07-03 04:53:14 | eve     | 10.0.0.5      | malware detected | Rootkit Signature       | High     |
| 2025-07-03 05:45:14 | david   | 172.16.0.3    | malware detected | Trojan Detected         | High     |
| 2025-07-03 07:45:14 | charlie | 172.16.0.3    | malware detected | Trojan Detected         | High     |
| 2025-07-03 04:41:14 | alice   | 172.16.0.3    | malware detected | Spyware Alert           | Medium   |

> ⚠️ These events were captured and verified from the Kibana Discover screenshots.

---

## 🧠 Recommendations
1. **Isolate infected hosts** to prevent lateral movement  
2. **Trigger endpoint malware scans** on affected machines  
3. **Audit user credentials** and enforce password resets if needed  
4. **Monitor flagged IP ranges** for unusual connection attempts  
5. **Review access logs** for any suspicious file access  

---

## 📬 Notification Plan
- Alert **SOC Lead** immediately  
- Share the report with **IT Security Manager**  
- Prepare **containment and remediation instructions** for affected endpoints  

---

## 📸 Dashboard Screenshots

*Example screenshots in this repository:*  
- `trojan.png`  
- `rootkit sign.png`  
- `worm infection.png`  
- `spyware.png`  
- `login failed.png`  
- `connection attempt.png`  

---

*This README captures Task 2 findings for your SOC analysis project, using Elastic Stack on Windows.*
