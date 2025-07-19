# Z-SHIELD 🔒
**Professional Offensive Security Toolkit by ZAIN NADEEM**

Z-SHIELD is a fully terminal-based offensive security toolkit built in Bash, designed to provide fast, aggressive, and visually professional cybersecurity assessments using only Kali Linux's built-in tools.

---

## 📌 Features

- 🎯 Fast & aggressive reconnaissance with clean tabular output
- ⚔️ Exploitation automation (Metasploit integration)
- 🧬 Malware scanning & suspicious file analysis
- 🌐 Live network monitoring and sniffing
- ✅ Clean UI, animated banner, and modular design
- 💡 Built for real-world offensive operations

---

## 📁 Modules Overview

### 1️⃣ Reconnaissance Module
**Purpose:** Fast information gathering on target domains or IPs.

- Performs aggressive open-port scanning using `nmap`
- Detects DNS records using `dnsenum`
- Automatically detects WordPress sites with `wpscan`
- Shows all results in clean, color-coded tables directly in the terminal

📂 Tools Used: `nmap`, `dnsenum`, `wpscan`

```bash
╭──────────────────────────────────────────╮
│         Z-SHIELD Recon Module            │
╰──────────────────────────────────────────╯

+--------+------------------------+
| PORT   | STATE & SERVICE        |
+--------+------------------------+
| 80/tcp | open  http             |
| 443/tcp| open  https            |
+--------+------------------------+

+--------+------------------------+
| TYPE   | DATA                   |
+--------+------------------------+
| A      | 192.0.2.1              |
| MX     | mail.example.com       |
+--------+------------------------+
```

2️⃣ Exploitation Module
Purpose: Launch Metasploit Framework with preset payload handling.

Automatically checks if msfconsole is installed

Prepares common handlers like reverse shells

Clean interactive menu

📂 Tools Used: msfconsole (Kali built-in)

```bash
╭──────────────────────────────────────────╮
│         Z-SHIELD Exploitation            │
╰──────────────────────────────────────────╯
```
3️⃣ Malware Analysis Module
Purpose: Scan directories for malware or suspicious files.

Scans user-specified folders using clamscan

Results shown in clean tables with color-coded threat indication

Fast scanning, CLI-friendly

📂 Tools Used: clamscan

```bash
╭──────────────────────────────────────────╮
│       Z-SHIELD Malware Analysis          │
╰──────────────────────────────────────────╯

+-------------------------+---------------+
| FILE                    | STATUS        |
+-------------------------+---------------+
| /home/user/infected.sh  | MALWARE FOUND |
+-------------------------+---------------+

```

4️⃣ Network Monitoring Module
Purpose: Monitor traffic on a selected network interface.

Live packet capture using tcpdump

Interface selector included

Can also show real-time connection tracking

📂 Tools Used: tcpdump, netstat, iftop

```bash
╭──────────────────────────────────────────╮
│     Z-SHIELD Network Monitoring          │
╰──────────────────────────────────────────╯

```
🚀 Installation
Run the following commands on Kali Linux:

```bash
git clone https://github.com/zainnadeem786/zshield.git

cd zshield

chmod +x install.sh

sudo ./install.sh

Then run:
./zshield
```
```bash
✅ Requirements
Z-SHIELD requires Kali Linux with the following tools pre-installed (they are by default):


nmap
dnsenum
wpscan
tcpdump
clamscan
netstat
msfconsole (optional for exploitation)
```

⚠️ Disclaimer
Z-SHIELD is intended for educational and authorized penetration testing only. Unauthorized use against systems you don't own or have explicit permission to test is illegal and unethical.

👨‍💻 Developed By
ZAIN NADEEM
Cybersecurity Engineer | Python Developer | Ethical Hacker

Z-SHIELD is part of an ongoing professional offensive toolkit project developed and maintained by Zain Nadeem. Contributions, ideas, and forks are welcome.

## 📄 License

This project is licensed under the [MIT License](./LICENSE) .

