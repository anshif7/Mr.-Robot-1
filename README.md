# Mr. Robot: 1 - VulnHub CTF Write-Up 🐱‍💻

---

## 📌 Overview

This repository contains a complete penetration testing walkthrough and report for the **Mr. Robot: 1** boot-to-root CTF challenge hosted on **VulnHub**.

Inspired by the TV show *Mr. Robot*, the VM simulates a realistic web attack scenario where the attacker must exploit misconfigurations, weak credentials, and vulnerable binaries to capture hidden flags and escalate to root.

---

## 🎯 Objectives

- Enumerate exposed services and files
- Brute-force WordPress admin credentials
- Upload a PHP reverse shell for remote access
- Escalate privileges via a vulnerable SUID binary
- Capture all three flags and achieve full root control

---

## 🛠️ Tools Used

- `nmap`
- `gobuster`
- `wpscan`
- `hydra`
- `burp suite`
- `python` (for TTY upgrade)
- `PHP reverse shell`
- Linux post-exploitation techniques

---

## 📜 Flags Captured

| Flag No. | Location                    | Description                   |
|:---------|:----------------------------|:-------------------------------|
| Key 1    | `robots.txt` and `fsocity.dic` | Wordlist for brute-force |
| Key 2    | `/home/robot/` directory     | After user shell access        |
| Key 3    | `/root/` directory (root shell) | Final flag after privilege escalation |

---

## 🔓 Exploitation Summary

- Discovered WordPress login page and weak admin credentials using `fsocity.dic`
- Gained admin panel access and uploaded a PHP reverse shell via the theme editor
- Escalated privileges by exploiting a vulnerable **SUID nmap binary** to spawn a root shell
- Captured all flags and documented mitigation recommendations

---

## 📑 Full Report

📖 See the full step-by-step penetration testing report here:

- [`MrRobot1-Report.md`](./MrRobot1-Report.md)

---

## 📖 About VulnHub

[VulnHub](https://www.vulnhub.com/) provides legally safe vulnerable machines for penetration testing practice and cybersecurity training.

---

## 📄 License

Open-source for educational and personal learning use.

---

## 📝 Author

**Anshif P.**

---

