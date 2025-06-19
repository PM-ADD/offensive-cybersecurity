# Multithreaded FTP Brute Force Script

## 📌 Overview

This Python script performs a **multithreaded brute-force attack** against an FTP server. It is optimized for speed using Python's `threading` and `queue` libraries, enabling concurrent login attempts.

**Important:** This script is meant strictly for **authorized security assessments**, training, or controlled environments like penetration testing labs.

## ⚠️ Legal Disclaimer

> ⚠️ This tool is for **educational and ethical hacking purposes only**.
>
> Do **NOT** use it on networks or systems without **explicit written permission**.
>
> Misuse of this tool may be **illegal** and subject to penalties under cybersecurity laws.

## 🚀 Features

- Uses Python threads to increase brute-force speed.
- Color-coded output using `colorama`.
- Graceful queue termination upon finding valid credentials.
- Customizable target host, port, user, and wordlist.

## 🧰 Requirements

- Python 3.x
- `colorama` module (`pip install colorama`)


## ⚙️ Configuration

Inside the script, configure:

```python
host = '192.168.1.195'     # Target FTP server IP
port = 21                  # FTP port (default: 21)
user = 'kali'              # Username to brute-force
n_threads = 30             # Number of concurrent threads
```

## 🛠️ Usage

1. **Install dependencies:**

   ```bash
   pip install colorama
   ```

2. **Prepare a wordlist:**

   Add passwords to `wordlist.txt`, one per line.

3. **Run the script:**

   ```bash
   python3 ftp_bruteforce.py
   ```

4. **Sample Output:**

   ```
   [+] Passwords to try: 500
   [!] Trying: admin123
   [!] Trying: password
   [+] Found credentials:
       Host: 192.168.1.195
       User: kali
       Password: toor
   ```

## 🧯 Defensive Recommendations

To protect against FTP brute-force attacks:

- Disable FTP or replace it with secure alternatives (e.g., SFTP, FTPS).
- Enforce account lockout policies on repeated failed attempts.
- Monitor and alert on brute-force patterns.
- Use firewalls or IDS/IPS to detect and block attack behavior.
