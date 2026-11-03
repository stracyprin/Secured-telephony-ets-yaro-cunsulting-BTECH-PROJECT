# Secured Telephony System - ETS YARO CONSULTING

**BTECH PROJECT 2026 | FOMIC POLYTECHNIC University | Network and Security**

## Problem Statement
ETS YARO CONSULTING used analog telephony which was not secure, costly, required physical lines, and affected communication between departments and clients (fuel station landlords). Voice quality was affected by interference and maintenance was expensive, reducing company credibility.

## Proposed Solution
Deployment of a Secured Company Telephony System using **Elastix Server** with:
- **Wireless VoIP communication** instead of physical lines
- **Authentication** of users (SIP extensions)
- **Encryption** of voice data
- **Centralized management** via Elastix web interface

## Architecture
**Old Architecture:** Analog phones -> Physical lines -> Analog switch
**New Architecture (Figure 3.2.1 a 2):** 3CX Softphones / IP Phones -> WiFi Network -> Elastix Server (192.168.1.x) -> Firewall

This allows internal calls between departments for free and secure communication.

## Implementation - What I Did

1.  **Installed Elastix Server:** Language, disk partition, network config, hostname, MySQL DB (Screenshots Fig 3.3.3 a1-a8)
2.  **Installed & Configured Firewall:** To protect Elastix server (Fig 3.3.3 1)
3.  **Configured Elastix:** Web authentication, SIP extensions creation (Fig 3.4 a1-a3)
4.  **Configured Clients:** 3CX Phone on users PCs with SIP credentials (Fig 3.5 1-2)
5.  **Tested:** Internal calls, call quality, security

## Security Measures Implemented
- **Confidentiality:** SIP authentication, Elastix admin password, Firewall rules
- **Integrity:** Encrypted VoIP packets vs analog interception
- **Availability:** Centralized Elastix system easier to maintain than analog lines

## Results
- Successful deployment of secured VoIP system for ETS YARO CONSULTING
- Cost reduction: No more analog line costs
- Improved communication between departments and clients
- Secure calls: Authentication required, no more eavesdropping on analog lines
- Easy maintenance via Elastix GUI

## Tools Used
Elastix 2.x, 3CX Softphone, CentOS, SIP Protocol, Firewall, Wireshark for testing

## Author
METAFE DEFFO STRACY GUILEINE - BTECH Network and Security - FPU - 2026
 under DR.IBRAHIM KOFI
