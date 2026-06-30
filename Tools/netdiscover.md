# Netdiscover

## What is Netdiscover?

## Why use Netdiscover?
- Discover live hosts.
- Identify IP addresses.
- Identify MAC addresses.
- Passive and Active scanning.

## Installation

### Kali Linux
```bash
netdiscover
```

## Basic Syntax

```bash
netdiscover [options]
```

## Common Commands

### Passive Mode

```bash
netdiscover -p
```

### Scan a Specific Network

```bash
netdiscover -r 192.168.100.0/24
```

### Scan a Range

```bash
netdiscover -r 192.168.100.20-50
```

### Ignore Specific Addresses

```bash
netdiscover -r 192.168.100.0/24 -i eth0
```

## Understanding the Output

- IP Address
- MAC Address
- Vendor
- Count

## Practical Example

## Tips

- Works only on local networks.
- Requires Layer 2 connectivity.
- Great before using Nmap.

## Common Mistakes

## References
