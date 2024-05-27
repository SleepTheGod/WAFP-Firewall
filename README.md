# Windows Advanced Firewall Protection (WAFP)

## Overview

Windows Advanced Firewall Protection (WAFP) is an advanced PowerShell script designed to enhance Windows Firewall security and mitigate various types of network attacks, such as DDoS, DoS, ICMP spoofing, TCP attacks, UDP attacks, and more.

## Features

- Add and remove firewall rules
- Enable and disable firewall logging
- Enable and disable firewall monitoring
- Enable and disable DDoS protection
- SYN flood protection
- ICMP flood protection
- UDP flood protection

## Usage

### Add a Firewall Rule


.\WAFP.ps1 -Command add -Name <name> -Action <Allow|Block> -Direction <In|Out> -Protocol <TCP|UDP|Any> -LocalPort <port> -RemotePort <port> -LocalAddress <address> -RemoteAddress <address> -Description <description>

Remove a Firewall Rule
.\WAFP.ps1 -Command remove -Name <name>

Enable Firewall Logging
.\WAFP.ps1 -Command enablelogging

Disable Firewall Logging
.\WAFP.ps1 -Command disablelogging

Enable Firewall Monitoring
.\WAFP.ps1 -Command enablemonitoring

Disable Firewall Monitoring
.\WAFP.ps1 -Command disablemonitoring

Enable DDoS Protection
.\WAFP.ps1 -Command disableddosprotection

Disable DDoS Protection
.\WAFP.ps1 -Command disableddosprotection
