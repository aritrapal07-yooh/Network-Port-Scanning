# Nmap 7.99 scan initiated Thu Nov  5 17:27:45 2026 as: /usr/lib/nmap/nmap -sT --top-ports 100 -oN scan_results.txt 192.168.10.0/24
Nmap scan report for 192.168.10.1
Host is up (0.0052s latency).
Not shown: 95 filtered tcp ports (no-response)
PORT      STATE  SERVICE
135/tcp   open   msrpc
139/tcp   open   netbios-ssn
445/tcp   open   microsoft-ds
8080/tcp  closed http-proxy
49152/tcp closed unknown
MAC Address: 00:50:56:C0:00:08 (VMware)

Nmap scan report for 192.168.10.2
Host is up (0.0012s latency).
Not shown: 99 closed tcp ports (conn-refused)
PORT   STATE SERVICE
53/tcp open  domain
MAC Address: 00:50:56:E1:D3:FA (VMware)

Nmap scan report for 192.168.10.254
Host is up (0.00040s latency).
All 100 scanned ports on 192.168.10.254 are in ignored states.
Not shown: 100 filtered tcp ports (no-response)
MAC Address: 00:50:56:FD:2A:5E (VMware)

Nmap scan report for 192.168.10.129
Host is up (0.00065s latency).
All 100 scanned ports on 192.168.10.129 are in ignored states.
Not shown: 100 closed tcp ports (conn-refused)

# Nmap done at Thu Nov  5 17:27:50 2026 -- 256 IP addresses (4 hosts up) scanned in 4.92 seconds
