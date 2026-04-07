# Incident Report 3

## 📌 Description
Every security requirement in this lab has a point value. 
If you find that a given security requirement is met, then you will add the points for the requirement to the total. 
If the security requirement is not met, then no points are added. 
In the end, you will need to determine the correct number of points based on your findings. 

## ⚠️ Incident
In this lab, I assumed the role of a Security Engineer and assessed the security readiness of a new Apache web server. 

## 🔍 Analysis
In Terminal window I've used the commands given to me in a .txt file.
I've check if the Apache web server was running the last veesion.
I've check if the directory listing was disable (if the server was secure the directory listing should be disable).
I've check if I easily can see the Apache server version, a secure web server should not easily reveal its version information to attackers.
I've check if the server redirect all unencrypted traffic (HTTP) to an encrypted service (HTTPS). 
I should see a message indicating that all traffic is being redirected ("301 Redirect"). 
If instead I see, in this case, "THIS IS MY WEBSITE" then traffic is not being redirected.
I've check if the server browser is safe, in this case, a valid SSL certificate like "THIS IS MY WEBSITE". 
If instead I see a message indicating an issue with the SSL certificate (e.g. "SSL Certificate problem: self signed certificate"), 
then this security requirement is not met.

## 🧾 Evidence
If you type a code wrong, is better to start over, unless you detect what you had done wrong early and fast.
In this lab, I found that just 1 point meet the requirements of security.
And you can cut/copy and paste from the file of commands given.

## 🛠️ Conclusion
Now I have to give the IT team the report, and that is security protocol of the server are not implemented correctly.

## 🛡️ Mitigation
Ask to the IT team to remake and meet the requirements, using my report to help them.
