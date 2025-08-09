# Nmap Scan Results – 172.20.10.2

## Overview
This project contains the results of a basic Nmap scan conducted on host **172.20.10.2** to identify open ports and running services.

## Scan Command
nmap -sV 172.20.10.2


## Findings
| Port | State | Service | Version | Significance |
|------|-------|---------|---------|--------------|
| 21/tcp | open | FTP | vsftpd 3.0.5 | Used for file transfers. May be vulnerable to brute-force or misconfigurations. |
| 22/tcp | open | SSH | OpenSSH 10.0p2 Debian 5 | Used for secure remote login. Common brute-force target. |

## Observations
- Both services are running on default ports.
- FTP is unencrypted by default.
- SSH is secure but should use strong authentication.

## Recommendations
- Restrict SSH access to trusted IPs.
- Use SFTP or FTPS instead of plain FTP.
- Disable anonymous FTP login.

