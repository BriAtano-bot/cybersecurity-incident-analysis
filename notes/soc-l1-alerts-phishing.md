# SOC L1 Alert Handling & Phishing Analysis

## 🎯 Overview
This document summarizes key concepts related to SOC L1 alert handling, triage processes, and phishing email analysis.

---

# 🚨 SOC L1 Alert Reporting

## 📌 Definition
Alert reporting is the process of documenting security alerts in a clear and structured way for further investigation.

## 🧠 Key Responsibilities
- Monitor SIEM alerts
- Document incidents clearly
- Escalate when necessary

## 📄 What an Alert Report Includes
- Summary of the alert
- Source (SIEM, logs, user report)
- Affected systems
- Initial assessment

---

# 🔍 SOC L1 Alert Triage

## 📌 Definition
Triage is the process of analyzing alerts to determine their severity and validity.

## 🧠 Steps in Triage

1. Identify the alert source
2. Validate if it is a true positive or false positive
3. Check related logs
4. Determine severity (Low / Medium / High)
5. Escalate if needed

---

## ⚠️ Triage Outcomes

- **False Positive** → no action needed
- **True Positive (Low)** → monitor
- **True Positive (High)** → escalate to L2

---

# 🎣 Phishing Emails in Action

## 📌 Definition
Phishing emails are used to trick users into revealing sensitive information or executing malicious actions.

---

## 📧 Common Indicators

- Suspicious sender address
- Urgent or threatening language
- Fake links (spoofed domains)
- Unexpected attachments

---

## 🔍 Email Analysis Process

1. Check sender email address
2. Inspect links (hover to verify domain)
3. Analyze attachments
4. Look for social engineering techniques

---

## 🧠 Example Scenario

- User receives email requesting password reset
- Link redirects to fake login page
- Credentials are captured by attacker

---

# 🛡️ SOC Perspective

From a SOC Analyst perspective:

- Correlate phishing emails with login activity
- Monitor for compromised accounts
- Identify patterns across users

---

# 📌 Conclusion

Effective alert handling and phishing detection are critical for:
- early threat detection
- incident response
- minimizing security risks
