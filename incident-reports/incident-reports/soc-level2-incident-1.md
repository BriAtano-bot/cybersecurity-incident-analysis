# SOC Level 2 - Incident Investigation

## 🎯 Objective
Analyze authentication logs to detect possible brute force attack.

---

## 🔍 Findings
- Multiple failed login attempts detected from IP 192.168.1.10
- One successful login after repeated failures
- Pattern indicates possible brute force attack

---

## 📊 Evidence
- High number of failed login attempts
- Successful authentication from same IP

---

## 🧠 Analysis
The sequence of failed attempts followed by a successful login suggests a brute force attack that eventually succeeded.

---

## 🛡️ Response
- Block suspicious IP
- Enforce account lockout policy
- Monitor authentication logs
