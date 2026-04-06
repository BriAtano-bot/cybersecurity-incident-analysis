# Incident Report 1

## 📌 Description
In this first lab, I assume the role of SOC Analyst tasked with reviewing a series of log records that show a password attack on an SSH server.

## ⚠️ Incident
A series of log records that show a password attack on an SSH server

## 🔍 Analysis
The date and time of the event.
The hostname of the system that recorded the event.
Descriptive text stating that the user failed to authenticate because they entered the wrong password.
Descriptive text stating that the source of the failed authentication attempt is the system IP given.

## 🧾 Evidence
We've been given a ssh_authentication_log.txt file, with all the information given to complete the task.

## 🛠️ Conclusion
Even if that log shows a failed authentication attempts, it also shows the adversary now knows the name of some valid user account on the target. 
Eventually the additional password attacks, will be focus in that username.

## 🛡️ Mitigation
A good defense against these techniques is multi-factor authentication. 
Where you need a username and password and a temporary code sent to you via text or available from an authenticator application.
