<p align="center">
  
  ![PYTHON](https://img.shields.io/badge/PYTHON-555555?style=for-the-badge)![3.10+](https://img.shields.io/badge/3.10%2B-0078FF?style=for-the-badge) ![PLATFORM](https://img.shields.io/badge/PLATFORM-555555?style=for-the-badge)![LINUX](https://img.shields.io/badge/LINUX-F15A24?style=for-the-badge) ![CATEGORY](https://img.shields.io/badge/CATEGORY-555555?style=for-the-badge)![NETWORKING](https://img.shields.io/badge/NETWORKING-F7C600?style=for-the-badge) ![TOOLS USED](https://img.shields.io/badge/TOOLS%20USED-555555?style=for-the-badge)![iproute2 | ping | subprocess](https://img.shields.io/badge/iproute2%20%7C%20ping%20%7C%20subprocess-E5736A?style=for-the-badge)
</p>

# operating-system-subnetting
## About the Code

This repository contains two implementations for IPv4 subnetting and network calculations:

### 1. IP Addressing (Python-only)

- Pure **Python implementation**.
- Converts IP addresses to integers and back.
- Converts CIDR to subnet masks.
- Calculates subnets based on required hosts.
- Displays network tables with **network ID, valid host range, and broadcast ID**.
- Validates special/reserved IPs (loopback, multicast, experimental).
- Fully functional **without any OS-specific tools**, so it runs on any system with Python and NumPy installed.

### 2. IP Subnetting (Linux-integrated)

- Extends the Python-only code by **integrating Linux system tools**.
- Automatically detects the host IP using the `ip` command (`ip -4 addr show`).
- Pings hosts in the subnet to check **reachability** using Linux `ping`.
- Ideal for Linux environments like Ubuntu, Debian, or AWS EC2.
- Simulated ping option included for environments where ICMP is blocked (e.g., some cloud servers).
- Provides real-time host scanning in addition to subnet calculations.

### In summary:
- Use the **Python-only code** if you want a cross-platform solution or just need subnetting tables.
- Use the **Linux-integrated code** if you want automatic host IP detection and reachable host scanning on Linux.
