# Firewall Setup and Testing (UFW on Linux)

## Overview
This project demonstrates configuring and testing basic firewall rules using **UFW (Uncomplicated Firewall)** on Linux.  
The goal was to understand how to allow and block specific network traffic, and verify the effects of firewall rules.

## What I Did
1. Checked the current firewall status.
2. Enabled UFW.
3. Added a rule to block inbound traffic on **port 23** (Telnet).
4. Tested the Telnet connection after blocking the port.
5. Added a rule to allow **SSH** on port 22.
6. Tested SSH connectivity to verify the allowed rule.
7. Removed the Telnet block rule to restore the original configuration.
   
## Tools Used
- **Linux UFW** — Command-line firewall management tool.
- **Telnet** — For testing blocked ports.
- **OpenSSH** — For testing allowed ports.

## Outcome
- Successfully configured UFW to block and allow specific ports.
- Verified rule effects through connection testing.
- Gained practical understanding of firewall traffic filtering.
