# CCNA Multi-Network Router Configuration and Connectivity Lab

## Overview
Configured a Cisco router and multiple end hosts across separate IPv4 networks using Cisco IOS CLI. Established inter-network communication through manual interface configuration, static addressing, subnet mask assignment, and Layer 3 routing verification.

This lab focused on operational network configuration and packet communication behavior including ARP resolution, broadcast traffic, and unicast forwarding between separate networks.

---

## Technical Objectives
- Configure router interfaces using Cisco IOS CLI
- Assign IPv4 addresses and subnet masks
- Enable and verify router interfaces
- Configure static host addressing
- Validate Layer 3 communication between networks
- Verify operational interface states
- Observe ARP broadcast and unicast packet behavior
- Test connectivity using ICMP echo requests

---

## Technologies and Concepts
- Cisco IOS
- IPv4 Addressing
- Subnetting
- Router Interface Configuration
- Static Host Configuration
- ARP
- ICMP
- Broadcast vs Unicast Communication
- Layer 3 Routing
- CLI Administration

---

## Network Topology
(Add topology screenshot here)

<img width="664" height="337" alt="CCNA Github 1" src="https://github.com/user-attachments/assets/c6fd100c-5de8-4fbb-ab9e-8f9f74c797fb" />

## Key IOS Commands Used

```bash
enable
configure terminal
interface g0/0
ip address
no shutdown
show ip interface brief
show running-config
ping

Example below.

*Ref 1: Network Diagram*
