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

<img width="664" height="337" alt="CCNA Github 1" src="https://github.com/user-attachments/assets/c6fd100c-5de8-4fbb-ab9e-8f9f74c797fb" />

## Key IOS Commands Used

```bash
enable
configure terminal
interface
ip address
no shutdown
show ip interface brief
show running-config
ping

---

## Configuration Explanation
Router interfaces were manually configured using Cisco IOS CLI. IPv4 addresses and subnet masks were assigned to each interface based on their associated network segments.

Interfaces were administratively enabled using the `no shutdown` command and verified using operational show commands including:

```bash
show ip interface brief
show running-config
```

Each host device was assigned a static IPv4 address, subnet mask, and default gateway corresponding to its local network.
```
---

## Packet Flow and Communication Behavior

When devices initiated communication, ARP broadcasts were first generated to resolve unknown destination MAC addresses on the local network.

After successful ARP resolution, communication transitioned into unicast Ethernet forwarding between devices.

The Cisco router functioned as the Layer 3 forwarding device responsible for routing traffic between the separate IPv4 networks.

---

## Connectivity Verification

ICMP ping testing was performed between hosts located on separate IPv4 networks to verify successful end-to-end communication.

Successful replies confirmed:
- Correct interface configuration
- Proper IPv4 addressing
- Accurate subnet mask assignment
- Operational router interfaces
- Proper Layer 3 packet forwarding
