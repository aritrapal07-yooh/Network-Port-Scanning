# 🛡️ Network Port Scanning & Reconnaissance Using Nmap

### Cyber Security Internship – Task 1



\


---

## 📌 Project Overview

This project focuses on understanding the fundamentals of **Network Reconnaissance and Port Scanning** using Nmap (Network Mapper), a widely used open-source network discovery and security auditing tool.

The primary objective is to identify active hosts, examine TCP port states, recognize running network services, and understand potential security exposures within an authorized local network environment.

This practical exercise provides hands-on experience with essential network security assessment techniques used in cybersecurity and ethical hacking.

## 🎯 Objectives

- Understand the fundamentals of network reconnaissance.
- Identify local IP addresses and network configurations.
- Discover active hosts within an authorized network.
- Perform TCP port scanning using Nmap.
- Identify open, closed, and filtered ports.
- Understand commonly used network ports and services.
- Explore basic service and version detection.
- Save and analyze scan results in multiple formats.
- Understand the importance of network security and attack surface management.

## 🛠️ Tools & Technologies

| Tool           | Purpose                                  |
| -------------- | ---------------------------------------- |
| Nmap           | Network discovery and port scanning      |
| Wireshark      | Network packet analysis                  |
| Kali Linux     | Cybersecurity testing environment        |
| Linux Terminal | Executing commands and analyzing results |

## ⚙️ Practical Implementation

### 1. Nmap Installation

Installed Nmap in the Kali Linux environment.

```bash
sudo apt update
sudo apt install nmap -y
```

Verified the installation:

```bash
nmap --version
```

### 2. Local Network Configuration

Identified the system's IP address and network interface.

```bash
ip addr
```

Checked the default gateway:

```bash
ip route
```

### 3. Host Discovery

Performed host discovery within an authorized local network.

```bash
nmap -sn 192.168.1.0/24
```

*Note: The network range above is an example. Replace it with the authorized subnet used in your practical.*

### 4. TCP Port Scanning

Performed a TCP Connect scan against an authorized test device.

```bash
nmap -sT --top-ports 100 127.0.0.1
```

### 5. Service Version Detection

Examined services and version information on selected authorized ports.

```bash
nmap -sV -p 80,443 127.0.0.1
```

### 6. Saving Scan Results

Exported scan results in three different formats using Nmap's output option.

```bash
nmap -sT --top-ports 100 127.0.0.1 -oA network_scan
```

This generated the following files:

| Filename             | Description                |
| -------------------- | -------------------------- |
| `network_scan.nmap`  | Human-readable scan report |
| `network_scan.xml`   | Structured XML scan report |
| `network_scan.gnmap` | Grepable scan output       |

## 📊 Understanding Port States

| Port State | Description                                                     |
| ---------- | --------------------------------------------------------------- |
| Open       | An application is listening on the port                         |
| Closed     | The device is reachable, but no application is listening        |
| Filtered   | Network filtering prevents Nmap from determining the port state |

### Common Network Ports

| Port | Service | Purpose                  |
| ---- | ------- | ------------------------ |
| 21   | FTP     | File transfer            |
| 22   | SSH     | Secure remote access     |
| 25   | SMTP    | Email transfer           |
| 53   | DNS     | Domain name resolution   |
| 80   | HTTP    | Web communication        |
| 443  | HTTPS   | Secure web communication |
| 3306 | MySQL   | Database service         |
| 3389 | RDP     | Remote desktop           |

## 📁 Project Structure

```text
Task-1-Network-Port-Scanning/
│
├── README.md
│
├── Results/
│   ├── network_scan.nmap
│   ├── network_scan.xml
│   └── network_scan.gnmap
│
└── Screenshots/
    ├── nmap_installation.png
    ├── ip_configuration.png
    ├── host_discovery.png
    └── port_scan_results.png
```

## 🔍 Key Learnings

Through this practical exercise, I gained an understanding of:

- Network reconnaissance fundamentals.
- TCP communication and port states.
- Host discovery techniques.
- Nmap scanning and output formats.
- Common network services and their associated ports.
- Basic network security assessment.
- The importance of identifying unnecessary exposed services.

## 🔐 Security Recommendations

- Disable unnecessary network services.
- Keep operating systems and applications updated.
- Configure firewalls properly.
- Use strong authentication mechanisms.
- Restrict unauthorized network access.
- Regularly monitor exposed network services.

## 📸 Practical Evidence

Screenshots and scan reports are included in the `Results/` directories to document the practical implementation.

## 📝 Conclusion

This project provided practical exposure to network reconnaissance and TCP port scanning using Nmap.

It helped build a foundation in network security assessment, service identification, and understanding network exposure.

The knowledge gained from this exercise will support further learning in ethical hacking, vulnerability assessment, penetration testing, and cybersecurity.

## 👨‍💻 Author

**Aritra Pal**

Cyber Security Enthusiast | B.Tech – Computer Science & Engineering

Interested in:

- Cyber Security
- Ethical Hacking
- Network Security
- Vulnerability Assessment
- Digital Forensics

🔗 **LinkedIn:** [https://www.linkedin.com/in/aritrapal07/](https://www.linkedin.com/in/aritrapal07/)

---

## ⚠️ Disclaimer

This project is intended strictly for educational purposes and authorized security testing.

All network scanning activities should be performed only on systems and networks for which explicit permission has been granted.

The author does not support or encourage unauthorized scanning or any illegal cyber activities.

---

**Cyber Security Internship | Task 1 | Network Port Scanning Using Nmap**

