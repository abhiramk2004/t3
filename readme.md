# Vulnerability Scan Report – Windows 10 (Nmap)

## Overview
This repository contains the results and documentation for a basic vulnerability scan performed on a Windows 10 system using **Nmap**.  
This task fulfills the internship requirement for performing an introductory vulnerability assessment.

## Tool Used
- **Nmap (Network Mapper)** – for port scanning, service enumeration, OS detection, and safe NSE checks.

## Steps Performed
1. Identified target machine IP (localhost – `127.0.0.1`).
2. Conducted port scan across default and common ports.
3. Performed service and version detection.
4. Ran safe Nmap Scripting Engine (NSE) scripts.
5. Collected observations and mapped preventive measures.

## Summary of Key Findings
- Standard Windows 10 ports such as **135**, **139**, **445**, and **3389** were detected.
- SMB and RDP services were found active.
- Detected UPnP and NetBIOS traffic over UDP.
- OS fingerprinting indicated Windows 10 (64-bit).

## Security Recommendations
- Disable unused SMB features and ensure **SMBv1** is turned off.
- Restrict RDP access; enable **NLA** if remote access is required.
- Keep Windows Firewall active with inbound blocking default.
- Disable NetBIOS over TCP/IP if not needed.
- Keep Windows updated with the latest security patches.

## Repository Contents
- `README.md` – Documentation of the scan process and results.
- `scan_output.txt` – Raw output of the Nmap scan.

## Notes
This assessment was performed ethically on a personal system as part of a cybersecurity internship task.
