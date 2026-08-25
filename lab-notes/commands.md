# Lab Command Reference 

A reference Library of the primary Linux and Nmap commands I used during the assessment including their purpose, for my own personal reference and a better explanation of my work. 

## Configuring the Network

### `ip addr`

Displays IP addresses, interface status, and network interfaces. Able to confirm the sudo assignment of the IP addresses to the VMs were successful and correct.

### `ping` 

Confirmed and tested basic network connectivity and communication between the Attacker and Target over the isolated network. 

## Local Service Enumeration

### `ss -tunap`

Identify listening services on my Target's system and compare local socket information.

## Network Reconnaissance

### `nmap`

Basic TCP port scan against the target. Established the initial Attack surface.

### `nmap -p-`

Expanded initial port scan to services outside the default Nmap range.

### `nmap -sT`

TCP connect scan used to verify port accessibility. 

### `sudo nmap -sU -p 53`

Assessed whether DNS was exposed over UDP.

## Host Assessment 

### `chage -l`

Used to conduct the password aging assessment. 

### `sudo ufw status`

Used to check the host firewall status, which returned inactive. 

> **Note:** This is a brief reference summary of the primary commands, not a full index of every command used. 
