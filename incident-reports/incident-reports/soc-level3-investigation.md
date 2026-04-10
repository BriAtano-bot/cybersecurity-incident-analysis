# SOC Level 3 - Distributed Attack Analysis

## 🎯 Objective
Investigate distributed login attempts across multiple IPs.

---

## 🔍 Findings
- Multiple IPs involved (192.168.1.10, .11, .12)
- Repeated failed login attempts across different IPs
- Successful logins from suspicious IPs

---

## 📊 Evidence
- High frequency of failed login attempts
- Multiple IPs targeting the system
- Successful authentication from previously suspicious IPs

---

## 🧠 Analysis
The activity indicates a distributed brute force attack where multiple IPs attempt to gain access. Some attempts succeeded, suggesting possible compromise.

---

## 🚨 Risk Level
High — multiple attackers and successful authentication detected.

---

## 🛡️ Response
- Block all suspicious IPs (.10, .11, .12)
- Monitor for further activity
- Reset passwords
- Expand log analysis to other systems
