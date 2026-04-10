# SOC Level 2 - Brute Force Detection

## 🎯 Objective
Analyze authentication logs to detect suspicious login attempts.

---

## 🔍 Findings
- Multiple failed login attempts from IP 192.168.1.10
- Successful login after repeated failures
- Indicates potential brute force attack

---

## 📊 Evidence
- High number of failed login attempts
- Pattern of repeated access from same IP
- Successful authentication after failures

---

## 🧠 Analysis
The attacker performed multiple failed login attempts followed by a successful login, indicating a possible brute force attack.

---

## 🚨 Risk Level
High — unauthorized access may have been achieved.

---

## 🛡️ Response
- Block suspicious IP (192.168.1.10)
- Monitor authentication logs
- Enforce account lockout policies
- Reset affected user credentials
