# Nmap

## What is Nmap?

Nmap (Network Mapper) is an open-source tool used for network discovery, host identification, service enumeration, and security auditing.

---

## Why use Nmap?

- Discover live hosts
- Identify open ports
- Detect running services
- Detect service versions
- Detect operating systems
- Run NSE scripts

---

## Installation
### Kali Linux

```bash
sudo apt install nmap
```
<img width="823" height="186" alt="nmap install " src="https://github.com/user-attachments/assets/72dc3a3f-cc31-45a8-9049-77d30fa42cc0" />

### Verify Installation

```bash
nmap --version
```
<img width="1001" height="145" alt="nmap --version" src="https://github.com/user-attachments/assets/ee2ebd64-5d1e-48d3-81e7-815b5e3bb138" />

---

## Basic Syntax

```bash
nmap [Options] <Target>
```

Example:

<img width="899" height="538" alt="nmap meta " src="https://github.com/user-attachments/assets/87c4f77b-e902-4714-85f0-e35de0af2001" />

```

## Common Commands

### Scan a single host

```bash
nmap <Target IP >
```

### Scan multiple hosts

```bash
nmap <Targer IP > <Target IP 2 >
```

### Scan a subnet

```bash
nmap 192.168.0.0/24
...
<img width="570" height="687" alt="nmap " src="https://github.com/user-attachments/assets/0b742928-1d4f-4663-b6d6-131785992556" />

...
### Scan specific ports

```
<img width="644" height="186" alt="nmap - p " src="https://github.com/user-attachments/assets/bb2e234b-61e5-4bfc-9887-bb15f7bd0ff7" />


### Scan all ports

```bash
nmap -p- <Target IP >
```
<img width="989" height="656" alt="nmap -p- " src="https://github.com/user-attachments/assets/c307fe84-bb6a-42d8-939f-35a989f056b3" />


### Service detection

```bash
nmap -sV 192.168.1.10
```

### OS detection

```bash
nmap -O 192.168.1.10
```

### Aggressive scan

```bash
nmap -A 192.168.1.10
```

### SYN Scan

```bash
nmap -sS 192.168.1.10
```

### UDP Scan

```bash
nmap -sU 192.168.1.10
```

---

## Useful NSE Scripts

```bash
nmap --script vuln 192.168.1.10
```

```bash
nmap --script smb-enum-shares 192.168.1.10
```

---

## My Notes

- `-sV` is one of the most useful options during enumeration.
- `-A` is useful but slower because it performs multiple detection techniques.
- `-p-` scans all 65535 ports.

---

## References

https://nmap.org
