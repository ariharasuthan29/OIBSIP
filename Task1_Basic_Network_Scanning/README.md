# Task 1: Basic Network Scanning with Nmap

## Oasis Infobyte Cyber Security Internship

### Objective

The objective of this task is to perform a basic network scan on a local machine using **Nmap**. The scan identifies active hosts, open TCP ports, running services, and the target operating system while providing a basic security assessment of the discovered services.

---

## Project Information

**Intern:** Ariharasuthan S

**Internship:** Oasis Infobyte – Cyber Security Internship

**Task:** Task 1 – Basic Network Scanning with Nmap

**Operating System:** Windows 11 (24H2–25H2)

**Tool Used:** Nmap 7.99

---

## Tools & Technologies

- Nmap 7.99
- Windows Command Prompt
- Windows 11
- GitHub

---

## Target Details

| Parameter | Value |
|----------|-------|
| Target IP | 10.60.253.154 |
| Scan Type | Local Machine Scan |
| Scan Date | 07 July 2026 |

---

## Commands Executed

```bash
nmap --version

ipconfig

nmap -sV 10.60.253.154

nmap -O 10.60.253.154

nmap -A 10.60.253.154
```

---

## Scan Results

### Host Status

- Host is reachable.
- Latency: **0.00058 seconds**
- Network Distance: **0 hops**

---

### Operating System Detection

```
Microsoft Windows 11
Version: Windows 11 24H2 – 25H2
```

---

### Open Ports

| Port | State | Service | Description |
|------|------|---------|-------------|
| 135 | Open | MSRPC | Microsoft Remote Procedure Call |
| 139 | Open | NetBIOS Session Service | Windows File & Printer Sharing |
| 445 | Open | Microsoft-DS (SMB) | Server Message Block File Sharing |

---

### SMB Security

The aggressive scan reported:

- SMB Message Signing: **Enabled**
- SMB Signing Requirement: **Required**

This configuration helps protect against SMB relay attacks by ensuring message integrity during SMB communication.

---

## Security Analysis

### Port 135 – Microsoft RPC

- Used for communication between Windows services.
- Necessary for several Windows functions.
- Should not be exposed to untrusted networks.

**Risk Level:** Medium

---

### Port 139 – NetBIOS

- Supports legacy Windows file and printer sharing.
- May expose shared resources if improperly configured.

**Risk Level:** Medium

---

### Port 445 – SMB

- Used for Windows file and printer sharing.
- Frequently targeted by malware and ransomware.
- Should never be exposed directly to the Internet.

**Risk Level:** High

---

## Observations

- The target machine is active and reachable.
- Only **3 out of the 1000 commonly scanned TCP ports** were open.
- Most ports were closed, reducing the attack surface.
- Nmap successfully identified the operating system.
- SMB security settings indicate message signing is enabled, improving security.

---

## Recommendations

- Keep Windows updated with the latest security patches.
- Enable Windows Firewall.
- Disable file sharing when not required.
- Restrict SMB access to trusted networks.
- Use strong passwords.
- Enable Multi-Factor Authentication (MFA) for administrative accounts.
- Regularly perform vulnerability and network scans.

---

## Conclusion

This project successfully demonstrated the use of **Nmap** for basic network reconnaissance. The scan identified the target operating system, active services, and open ports while providing valuable insights into the system's network exposure. The findings highlight the importance of minimizing exposed services, maintaining up-to-date systems, and implementing appropriate security controls to reduce potential attack vectors.

---

## Repository Structure

```
Task1_Basic_Network_Scanning/
│
├── README.md
├── scan_results.txt
├── scan_commands.txt
└── Screenshots/
    ├── 01_nmap_version.png
    ├── 02_ipconfig.png
    ├── 03_service_scan.png
    ├── 04_os_detection.png
    └── 05_aggressive_scan.png
```

---

## References

- https://nmap.org/
- https://nmap.org/book/
- https://learn.microsoft.com/windows/security/

---

**Author:** Ariharasuthan S

**Internship:** Oasis Infobyte Cyber Security Internship
