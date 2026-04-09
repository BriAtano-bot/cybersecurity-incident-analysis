# Linux Fundamentals - Level 1

## 🎯 Objective
Learn the basic usage of Linux systems, including navigation, file management, and essential commands.

---

## 🐧 What is Linux?
Linux is an open-source operating system widely used in servers, cybersecurity, and networking.

---

## 📂 File Navigation
Basic commands:

- pwd → shows current directory
- ls → lists files
- cd → change directory

---

## 📁 File Management
- mkdir → create directory
- touch → create file
- cp → copy files
- mv → move/rename files
- rm → delete files

---

## 🔍 Viewing Files
- cat → display file content
- less → view large files
- head / tail → preview file sections

---

## 🔐 Permissions (Basic)
- chmod → change permissions
- understanding read/write/execute

---

## 🧠 What I Learned
- How to navigate Linux systems
- How to manage files and directories
- Importance of Linux in cybersecurity

---

## 🧪 Practical Experience
- Completed TryHackMe Linux Fundamentals Level 1
- Used terminal commands in a real environment

---

## 🚀 Next Steps
- Learn intermediate Linux commands
- Work with logs and system processes
- Combine Linux with networking tools

- ---

## 💡 Personal Notes
Linux is essential for cybersecurity because most servers run on it. Learning the terminal is a key step toward becoming a SOC analyst.

---

## 🔎 Useful Commands

### grep
Search for specific text inside files.

Example:
grep "error" logfile.txt

---

### & (Run in background)
Runs a command in the background so the terminal can still be used.

Example:
sleep 10 &

---

## 🧠 Why "&" is Useful

Running commands in the background allows multitasking, which is useful when:

- running long processes
- monitoring systems
- performing multiple operations simultaneously

---

### && (AND operator)
Run the next command only if the previous one succeeds.

Example:
mkdir test && cd test

---### Difference between & and &&

- & → runs command in background
- && → runs next command only if previous succeeds

---

### > (Overwrite output)
Redirect output to a file (overwrites existing content).

Example:
echo "hello" > file.txt

---

### >> (Append output)
Add output to a file without deleting existing content.

Example:
echo "world" >> file.txt

---

## 🔍 Advanced Useful Commands

### find
Search for files and directories.

Example:
find /home -name "file.txt"

---

### wc (word count)
Counts lines, words, and characters.

Example:
wc logfile.txt

---

### -R (Recursive search)
Used with commands like grep to search inside folders.

Example:
grep -R "error" /var/log
