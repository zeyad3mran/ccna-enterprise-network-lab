# 🌐 Enterprise Network Project - CCNA Lab

## Overview
Multi-site enterprise network simulation built in Cisco Packet Tracer,
simulating a real enterprise environment with HQ and two branch offices.

## 🖧 Network Topology
- **HQ:** 2 Switches, 1 Router (2911), 1 DHCP/DNS Server
- **Branch A & B:** 1 Switch, 1 Router (2911) each
- **WAN Links:** Serial connections (HWIC-2T)
- **Internet:** NAT/PAT via HQ Router

## ✅ Technologies Implemented
- VLANs & Trunking (802.1Q) — VLAN 10/IT, 20/HR, 30/Sales, 99/Management
- Inter-VLAN Routing (Router-on-a-Stick)
- OSPF Single Area Routing (Area 0)
- Centralized DHCP Server with IP Helper-Address Relay
- Extended Named ACLs (Security Policies)
- NAT/PAT Overload (Internet Connectivity)
- Port Security with Sticky MAC
- SSH v2 Remote Management
- STP Tuning (PortFast + BPDU Guard)

## 📋 IP Addressing Scheme
| Site | VLAN | Name | Subnet |
|------|------|------|--------|
| HQ | 10 | IT | 10.10.10.0/24 |
| HQ | 20 | HR | 10.10.20.0/24 |
| HQ | 30 | Sales | 10.10.30.0/24 |
| HQ | 99 | Management | 10.10.99.0/24 |
| Branch A | 10 | IT | 10.20.10.0/24 |
| Branch A | 20 | HR | 10.20.20.0/24 |
| Branch A | 30 | Sales | 10.20.30.0/24 |
| Branch B | 10 | IT | 10.30.10.0/24 |
| Branch B | 20 | HR | 10.30.20.0/24 |
| Branch B | 30 | Sales | 10.30.30.0/24 |
| WAN | - | HQ↔BranchA | 10.0.12.0/30 |
| WAN | - | HQ↔BranchB | 10.0.13.0/30 |

## 🛠️ Tools Used
- Cisco Packet Tracer
- Cisco 2911 Routers
- Cisco 2960 Switches

## 📁 Files
- `ccna-enterprise-network-lab.pkt` — Cisco Packet Tracer project file
  ## 📸 Screenshots

### Network Topology
![Topology](topology.png)

## 👤 Author
**Zeyad Mohamed**
CCNA Candidate | Networking Student
