# Nmap

## Purpose
Nmap is a network scanning tool used to discover hosts, open ports, running services, and operating systems.

## Common Commands

### Ping Scan
```bash
nmap -sn 192.168.1.0/24
```

### Service Detection
```bash
nmap -sV 192.168.1.10
```

### SYN Scan
```bash
nmap -sS 192.168.1.10
```

### OS Detection
```bash
nmap -O 192.168.1.10
```

### Aggressive Scan
```bash
nmap -A 192.168.1.10
```

## Notes
- Always start with enumeration.
- Scan only systems you are authorized to test.
