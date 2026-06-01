# Core 1 Networking & Command Line Quick Reference

These are the core networking concepts I mastered for the Core 1 exam, mixed with actual Command Prompt testing logs.

## 🔌 Essential Port Numbers (The Ones You Always Forget)
* **Port 22:** SSH (Secure Shell) - Encrypted remote access.
* **Port 23:** Telnet - Unencrypted (never use this in production!).
* **Port 53:** DNS (Domain Name System) - Resolves names to IPs.
* **Port 80 / 443:** HTTP / HTTPS - Web traffic.
* **Port 3389:** RDP (Remote Desktop Protocol) - Windows remote management.

## 💻 Terminal Command Testing
While studying networking protocols, I tested out the commands directly in the Windows Command Prompt (CMD) to see how data moves in real time.

### 1. Checking Interfaces
To find my local IP address, subnet mask, and default gateway, I used the classic Windows networking tool:
```cmd
ipconfig
```
This gave me my local IPv4 address (e.g., `192.168.1.XX`) and confirmed my connection to my home router.

### 2. Connectivity Testing
Verified internet routing and DNS resolution by pinging Google's public DNS servers directly via its IP address to ensure packets were leaving my local gateway:
```cmd
ping 8.8.8.8
```
Got consistent responses with zero packet loss, proving my network interface card (NIC) was talking to the wider web perfectly.
