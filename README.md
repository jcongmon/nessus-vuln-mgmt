# Nessus Vulnerability Management
![Architecture Diagram](https://i.imgur.com/pJ4jihU.png)

## Introduction

In this project, I used Microsoft Azure and Nessus to demonstrate the full vulnerability management process, from identification to remediation. I deployed a vulnerable virtual machine intentionally configured with outdated software to simulate real-world scenarios and set up a Vulnerability Management Scanner. Using both unauthenticated and credentialed scans, I identified vulnerabilities, implemented remediations, and verified the fixes through follow-up scans.

The following virtual machines were provisioned in Azure on the same virtual network:
- Windows 10 with Nessus Essentials
- Windows 10 with Adobe Reader v10.0, Firefox v97.0, and VLC Media Player v1.1.7.

## Vulnerability Scans Before Remediation
Unauthenticated Vulnerability Scans
![Unauthenticated Vulnerability Scans](https://i.imgur.com/LqJ6bJE.png)
Credentialed Vulnerability Scans
![Credentialed Vulnerability Scans](https://i.imgur.com/nQEN3Wa.png)
Credentialed Vulnerability Scans, Breakdown
![Credentialed Vulnerability Scans](https://i.imgur.com/SZvwRfb.png)
Credentialed Vulnerability Scans, Firefox Example
![Credentialed Vulnerability Scans](https://i.imgur.com/IFeWiqG.png)

## Vulnerability Scans After Remediation
Credentialed Vulnerability Scans
![Credentialed Vulnerability Scans](https://i.imgur.com/5L5NqQx.png)

Adobe Reader, Firefox, and VLC Media Player were uninstalled to "remediate" vulnerabilities. Windows 10 was updated to the latest version.

## Conclusion

This project involved a secure Azure network with a Nessus Vulnerability Scanner and a vulnerable Windows 10 VM featuring outdated software and disabled security controls. Using Nessus, I conducted unauthenticated and credentialed scans, identifying 48 critical and 63 high vulnerabilities before remediation. After addressing the issues, follow-up scans found reduced counts to 1 critical and 15 high vulnerabilities. 
