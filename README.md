# Task 1: Basic Network Scanning with Nmap

## Objective

Perform a network scan to identify open ports and services using Nmap.

## Tool Used

- Nmap 7.99

## Target

- IP Address: 10.208.204.77

## Commands Used

```bash
ipconfig

nmap -sV -O 10.208.204.77
```

## Scan ResultS

### Open Ports and Services

| Port | Service | Description |
|--------|---------|------------|
| 135/tcp | MSRPC | Windows service communication |
| 139/tcp | NetBIOS-SSN | File and printer sharing |
| 445/tcp | Microsoft-DS (SMB) | Windows file sharing |
| 2869/tcp | HTTPAPI (UPnP) | Device discovery service |
| 3306/tcp | MySQL | Database service |

## Port Explanation

### Port 135 (MSRPC)
Used by Windows services for communication between applications and system components.

### Port 139 (NetBIOS)
Used for file and printer sharing in Windows networks.

### Port 445 (SMB)
Used for Windows file sharing and network resource access.

### Port 2869 (HTTPAPI/UPnP)
Used for network device discovery and communication.

### Port 3306 (MySQL)
Default port used by MySQL database servers.

## Findings

- Five open TCP ports were identified.
- Windows networking services are active.
- A MySQL database service is running.
- The operating system was detected as Microsoft Windows 11.

## Conclusion

The Nmap scan successfully identified open ports, running services, and operating system information. This demonstrates how Nmap can be used for basic network reconnaissance and service enumeration.

## Outcome

Successfully completed a basic network scan using Nmap and analyzed the discovered services.
