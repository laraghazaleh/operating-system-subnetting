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
