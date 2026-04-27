# VoIP-IP Telephony Networking Project
## Overview
A fully simulated enterprise VoIP telephony network designed in Cisco Packet Tracer. The network spans 4 departments — ICT, Finance, Sales, and HR — each with dedicated IP phones, PCs, printers, and a centralised server room, all interconnected through a routed network with separate voice and data VLANs.

## Network Topology

4 departmental routers: ICT, Finance, Sales, HR
1 central server room switch connected to HTTP, DNS, EMAIL, DHCP servers
4 department switches managing local devices
40+ IP phones distributed across all departments
40+ PCs across all departments
4 printers (one per department)
Inter-router connectivity via point-to-point links (10.10.10.x/30 subnets)


## Department Configuration
DepartmentData VLANVoice VLANData NetworkVoice NetworkICT40100192.168.100.96/27172.16.100.96/27Finance10100192.168.100.0/27172.16.100.0/27Sales30100192.168.100.64/27172.16.100.64/27HR20100192.168.100.32/27172.16.100.32/27

## Key Features

Voice and data traffic separated using VLANs on every department switch
DHCP configured for automatic IP assignment to phones and PCs
Inter-department calling enabled through dial-plan configuration on each router
Centralised server room providing HTTP, DNS, EMAIL, and DHCP services to the entire network
Subnetting applied across all departments using /27 and /30 masks


## Tech Stack

Tool: Cisco Packet Tracer
Protocols: VoIP, SCCP, DHCP, DNS, HTTP
Concepts: VLANs, subnetting, inter-VLAN routing, CME, dial-peer configuration, point-to-point links


## How to Open

Install Cisco Packet Tracer (free via Cisco NetAcad)
Open CN_Lab_Project_VoIP_Final.pkt
Click any router to inspect CME and dial-plan configuration
Use Simulation Mode to test voice calls between departments


## What I Learned

Designing a multi-department enterprise network from scratch
Configuring VoIP using Cisco CME across multiple routers
Separating voice and data traffic using VLANs
Subnetting a network efficiently across departments
How DHCP, DNS, and HTTP services integrate into a routed enterprise topology


