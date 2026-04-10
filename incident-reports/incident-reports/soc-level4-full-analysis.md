# SOC Level 4 - Multi-Source Attack Investigation

## 🎯 Objective
Correlate authentication logs with web server logs to identify a complete attack chain.

---

## 🔍 Findings
- IP 192.168.1.10 performed multiple failed login attempts
- Same IP accessed web endpoints (/login, /dashboard)
- Successful login followed by access to protected resource (/dashboard)
- Additional suspicious activity from IPs 192.168.1.11 and 192.168.1.12

---

## 📊 Evidence
- Repeated failed login attempts (auth.log)
- HTTP requests showing login attempts (POST /login → 401, 200)
- Access to restricted areas (/admin → 403)
- Successful login followed by dashboard access

---

## 🧠 Analysis
The attacker conducted reconnaissance via web endpoints, followed by brute force login attempts. After gaining access, the attacker accessed a protected resource, indicating system compromise.

---

## 🚨 Risk Level
Critical — confirmed unauthorized access and post-login activity.

---

## 🛡️ Response
- Block all suspicious IPs (.10, .11, .12)
- Invalidate active sessions
- Reset compromised credentials
- Investigate data access and potential exfiltration
- Increase monitoring across systems
