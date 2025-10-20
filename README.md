## Summary
Scanned network: 192.168.1.0/24 (Kali Linux). Host discovery found X live hosts. Performed TCP SYN scan and service detection.

## Commands used
- `sudo nmap -sn 192.168.1.0/24 -oN host-discovery.txt`
- `sudo nmap -sS --open --reason 192.168.1.0/24 -oN nmap-syn-scan.txt`
- `sudo nmap -sS -sV -p- 192.168.1.5 -oN 192.168.1.5-sv-allports.txt`

## Top findings
- 192.168.1.5 — Open: 22 (OpenSSH 7.9), 80 (Apache 2.4.29) — Risk: Medium — Mitigation: SSH keys, update Apache
