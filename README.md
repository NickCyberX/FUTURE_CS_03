# 🛡️ Wi-Fi Security Assessment Report

## 📋 Overview

This project is part of a cybersecurity internship task focused on evaluating the security of a home Wi-Fi network. The goal was to identify vulnerabilities, assess network activity, and recommend improvements using tools like **Nmap** and **Wireshark**.

---

## 🎯 Objectives

- Analyze the encryption and password strength of the home Wi-Fi.
- Detect open ports and active services using Nmap.
- Identify unauthorized or suspicious devices on the network.
- Monitor and analyze network traffic using Wireshark.

---

## 🧰 Tools & Environment

| Tool        | Purpose                                   |
|-------------|--------------------------------------------|
| Kali Linux  | Penetration testing environment (VirtualBox) |
| Nmap        | Host discovery and port scanning           |
| Wireshark   | Network traffic capture and protocol analysis |
| VirtualBox  | To run Kali Linux in a virtualized environment |

---

## 🚀 Steps Performed

### 1. Network Discovery

nmap -sn 192.168.1.0/24


Used to discover active devices on the subnet.

### 2. Port & Service Scanning


nmap -sV 192.168.1.X


Used to identify open ports and running services.

### 3. Packet Capture with Wireshark

- Launched Wireshark on the active interface.
- Monitored live traffic.
- Applied filters (e.g., `http`, `dns`) to isolate useful traffic.
- Analyzed observed protocols like DHCP, ICMPv6, and mDNS.

### 4. Router Configuration Review

- Confirmed WPA2 encryption.
- Ensured WPS is disabled.
- Verified strong admin and Wi-Fi passwords.
- Reviewed connected device list.

---

## ✅ Findings

- No unauthorized devices found on the network.
- No dangerous ports (e.g., Telnet, FTP) were open.
- Strong encryption (WPA2-PSK) in use.
- Network traffic showed no signs of active threats.

---

## 💡 Recommendations

- Periodically audit connected devices.
- Regularly update router firmware.
- Upgrade to WPA3 if possible.
- Disable unused features like UPnP and remote access.

---

## ⚠️ Challenges

- **No Wi-Fi Adapter**: Monitor mode scanning and wireless packet capture were not possible.
- **VM Limitations**: Full network visibility was restricted due to VirtualBox NAT mode.

---

## 📁 Report

Download the full detailed report:  
📄 `WiFi Security Assessment Report.docx` (to be uploaded to the repo)

---

## 📌 Author

- **Intern:** `Tobechukwu Nicholas`
- **Platform:** `Future Interns`

---

## 📜 License

This project is for educational purposes as part of a cybersecurity internship. No real user data was intercepted, and all testing was conducted in a legal, home-network environment.
```
