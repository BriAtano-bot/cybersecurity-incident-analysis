# SOC Investigation 1 - Failed Login Analysis

## 📌 Scenario
Analyzed authentication logs to detect suspicious login attempts.

---

## 🔍 Findings
- Multiple failed login attempts detected
- IP 192.168.1.10 appears several times
- Indicates possible brute force attempt

---

## 📊 Evidence
Used grep and wc to identify patterns in logs.

---

## 🛠️ Conclusion
Suspicious activity detected from a single IP.

---

## 🛡️ Recommendation
- Block the IP
- Monitor login attempts
- Implement account lockout policies
