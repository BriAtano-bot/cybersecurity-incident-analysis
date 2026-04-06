# Incident Report 2

## 📌 Description
You will assume the role of a Penetration Tester. 
You are with cracking a list of passwords that you previously exfiltrated from a vulnerable web application. 
The vulnerable application was successfully exploited, resulting in leaked passwords that require cleartext (or cracked) values. 
Once acquired, you can use them to extend your attacks against the system or even pivot within the internal network to another system. 
The goal of this exercise is to identify the password hashing algorithm and attempt to crack the password.

## ⚠️ Incident
The goal of most penetration tests is to find as many vulnerabilities as possible in the specified time period.

## 🔍 Analysis
We had to code in a Terminal Emulator.

## 🧾 Evidence
  - By definition, hashing algorithms cannot be reversed, but many older hashing algorithms can now be decoded due to weaknesses in the ways they were created. 
    If we can discover what algorithm was used to create the hash, we may be able to decode the original text used. 
  - I used the hash-identifier tool to attempt to determine the original hashing algorithm used.
    Hash-identifier runs a series of tests on a given hash value to attempt to determine the algorithm used to create the hash. 
    This is important because trying to decode a hash using the wrong algorithm won't yield the results we're looking for.
  - Crack the hashed password using a tool called John the Ripper.
  - John the Ripper will compare our hash with a wordlist made up of several known hashes and their original text.
  - If our hash is in the wordlist we selected, when John the Ripper finishes running, you'll see the password displayed in the middle of the output.

## 🛠️ Conclusion
Every word and space and symbol, counts, make sure you type everything right, or you going to be in a merry-go-round.

## 🛡️ Mitigation
N/A
