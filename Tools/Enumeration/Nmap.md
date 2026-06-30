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
<img width="823" height="181" alt="nmap install" src="https://github.com/user-attachments/assets/c8d6c5c9-7654-47c2-aedd-6cb6724f030e" />

### Verify Installation

```bash
nmap --version
```
<img width="1125" height="141" alt="nmap --ver" src="https://github.com/user-attachments/assets/ff44a8a3-3628-48c8-be4f-d0cdac1a5d3e" />

---

## Basic Syntax

```bash
nmap [Options] <Target>
```

Example:

<img width="752" height="178" alt="nmap --help" src="https://github.com/user-attachments/assets/4715c69a-6b28-42cb-82c4-2ca15ac4b81b" />

```

## Common Commands

### Scan a single host

```bash
nmap <Target IP >
```
<img width="865" height="545" alt="Nmap ip " src="https://github.com/user-attachments/assets/816209e8-234c-4fe9-b176-9173e7496123" />


### Scan multiple hosts

```bash
nmap <Targer IP > <Target IP 2 >
```


### Scan a subnet

```bash
nmap <Target IP >
```

Example:
<img width="870" height="701" alt="nmap " src="https://github.com/user-attachments/assets/060b69dd-5d34-4621-98e7-625cd49b754b" />

```
### Scan specific ports

```
<img width="672" height="196" alt="nmap -p " src="https://github.com/user-attachments/assets/7853fd32-6586-46a0-9855-2f4fdae543f6" />


### Scan all ports

```bash
nmap -p- <Target IP >
```
<img width="777" height="650" alt="nmap -p-" src="https://github.com/user-attachments/assets/0ad48e32-d767-49c2-9c14-e4f317693d11" />


### Service detection

```bash
nmap -sV <Target IP >
```
<img width="1024" height="565" alt="nmap -sV " src="https://github.com/user-attachments/assets/68368cf9-9376-47fe-9c29-c0efb14ef02e" />

### OS detection

```bash
nmap -O <Target IP >
```
<img width="847" height="639" alt="nmap -O" src="https://github.com/user-attachments/assets/792e6301-d284-48be-a98b-2118724f6cd4" />

### Aggressive scan

```bash
nmap -A <Target IP >
```
<img width="1216" height="681" alt="nmap -A " src="https://github.com/user-attachments/assets/f27a844d-dcf2-4511-8595-6de2a8d641da" />

### SYN Scan

```bash
nmap -sS <Target IP >
```
<img width="807" height="535" alt="nmap -sS " src="https://github.com/user-attachments/assets/e2602d33-a3f0-491d-adb9-85df672e0710" />

### UDP Scan

```bash
nmap -sU <Target IP >
```

---

## Useful NSE Scripts

```bash
nmap --script vuln <Target IP >
```
<img width="967" height="709" alt="nmap --script" src="https://github.com/user-attachments/assets/c933ddb5-0245-48ca-a5c5-562d6f85035e" />

```bash
nmap --script smb-enum-shares <Target IP >
```

---

## My Notes

- `-sV` is one of the most useful options during enumeration.
- `-A` is useful but slower because it performs multiple detection techniques.
- `-p-` scans all 65535 ports.
- #The Target IP is MetaSploitable2 

---

## References

https://nmap.org
