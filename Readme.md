# Linux System Administration Scripts Collection

## 👤 Author

**Name:** Pawan Yadav


---

## 📌 Overview

This project contains a collection of **basic Linux system administration scripts** designed to automate common tasks such as monitoring login attempts, system activity, and user information.

Each script is written in **Bash** and is beginner-friendly, with clear steps and comments.

---

## 📂 Scripts Included

### 1️⃣ Show Last 10 Failed Login Attempts

* **Description:**
  Displays the last 10 failed login attempts from system logs.
* **Log File Used:** `/var/log/auth.log`
* **Commands Used:** `grep`, `tail`
* **Purpose:**
  Helps in detecting unauthorized access attempts.

---

### 2️⃣ Display Last 5 System Reboots

* **Description:**
  Shows the most recent 5 system reboot records.
* **Commands Used:** `last`, `head`
* **Purpose:**
  Useful for tracking system uptime history and reboots.

---

### 3️⃣ Dynamic Welcome Message (/etc/motd)

* **Description:**
  Updates the system welcome message with dynamic system details.
* **Information Displayed:**

  * Hostname
  * IP Address
  * System Uptime
  * Last Login
* **Commands Used:** `hostname`, `uptime`, `last`, `awk`
* **Note:** Requires **sudo privileges**.

---

### 4️⃣ User Session Logger

* **Description:**
  Logs currently logged-in users along with timestamps.
* **Log File:** `/var/log/user_sessions.log`
* **Commands Used:** `who`, `date`
* **Purpose:**
  Helps track user activity over time.

---

### 5️⃣ Extract Usernames from /etc/passwd

* **Description:**
  Extracts all usernames from the `/etc/passwd` file.
* **Output File:** `userlist.txt`
* **Command Used:** `cut`
* **Purpose:**
  Useful for listing all system users.

---

## ⚙️ Requirements

* Linux OS (Ubuntu/Debian recommended)
* Bash shell
* Root/sudo access (for some scripts)

---

## ▶️ How to Run

1. Give execute permission:

```bash
chmod +x script_name.sh
```

2. Run the script:

```bash
./script_name.sh
```

---

## ⚠️ Notes

* Some scripts require **sudo privileges** (especially those accessing `/etc/motd` or `/var/log`).
* Ensure log files exist before execution.
* Scripts are tested on **Ubuntu/Debian-based systems**.

---

## 🎯 Purpose of Project

This project is part of a **Linux System Administration learning module**, aimed at:

* Understanding system logs
* Automating administrative tasks
* Practicing shell scripting

---

## 📌 Conclusion

These scripts demonstrate basic but essential system administration tasks using Bash. They are useful for beginners to understand how Linux handles logs, users, and system information.

---
