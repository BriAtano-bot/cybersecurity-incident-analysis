# Windows Threat Detection & Kill Chain

## 🎯 Overview
This document summarizes key concepts related to Windows logging, threat detection, and attack lifecycle analysis.

---

## 🧠 Unified Kill Chain

The kill chain describes the stages of a cyber attack:

1. Reconnaissance
2. Initial Access
3. Execution
4. Persistence
5. Privilege Escalation
6. Lateral Movement
7. Exfiltration

---

## 🪟 Windows Logging for SOC

### 📜 Key Logs

- Security Logs → login attempts
- System Logs → system events
- Application Logs → app-related activity

---

## 🔐 Important Events

- Failed login attempts
- Successful logins
- Account changes
- Suspicious processes

---

## 🔍 Windows Threat Detection

SOC Analysts monitor:

- Unusual login patterns
- Multiple failed attempts
- Unexpected processes
- Abnormal user behavior

---

## ⚔️ Pentesting Perspective

Understanding attacker behavior helps:
- predict attacks
- detect early indicators
- improve response

---

## 🛡️ SOC Perspective

- Correlate logs across systems
- Identify attack stages using kill chain
- Respond quickly to suspicious activity

---

## 📌 Conclusion

Windows logging and threat detection are critical for:
- identifying attacks
- understanding attacker behavior
- improving SOC response
