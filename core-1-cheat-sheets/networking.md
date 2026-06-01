# Core 1 Networking & Command Line Quick Reference

These are the core networking concepts I mastered for the Core 1 exam, mixed with actual terminal testing logs.

## 🔌 Essential Port Numbers (The Ones You Always Forget)
* **Port 22:** SSH (Secure Shell) - Encrypted remote access.
* **Port 23:** Telnet - Unencrypted (never use this in production!).
* **Port 53:** DNS (Domain Name System) - Resolves names to IPs.
* **Port 80 / 443:** HTTP / HTTPS - Web traffic.
* **Port 3389:** RDP (Remote Desktop Protocol) - Windows remote management.

## 💻 Terminal Command Testing
While studying networking protocols, I tested out the commands directly on my Linux environment to see how data moves.

### 1. Checking Interfaces
Tried running the old `ifconfig` command, but got stuck with a `>` prompt because of a typo! After hitting `Ctrl + C` to clear it, I used the modern alternative:
```bash
ip a
```
This gave me my local IP address (`192.168.1.XX`) and showed my active network cards.

### 2. Connectivity Testing
Verified internet routing by pinging Google's public DNS servers directly via its IP address:
```bash
ping 8.8.8.8
```
Got consistent responses around `12ms` to `15ms`, proving the local gateway was transfering packets out to the wider web with zero packet loss.
