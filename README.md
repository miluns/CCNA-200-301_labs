# CCNA 200-301 Laboratory Portfolio
Technical implementation of CCNA 200-301 laboratory scenarios. Focused on L2/L3 architecture, protocol analysis, and network redundancy. Includes Cisco IOS configurations for OSPF, STP/LACP, HSRP and core infrastructure protocols.

## Project Structure
The laboratories are categorized by functional domain, following the official Cisco exam blueprint. Each directory contains the .pkt source file and, where applicable, exported device configurations in plain text.

01. **Network Fundamentals**  
Basic connectivity, IPv4 addressing, VLSM, and initial device hardening.  
> [!IMPORTANT] Key implementations: SSH access, line security, interface management, and OSI model flow analysis.

02. **Ethernet Switching**  
Layer 2 technologies focusing on loop prevention and logical segmentation.
- Key implementations: VLAN/Trunking (802.1Q), VTP/DTP, STP (802.1D) tuning, Rapid-PVST+, and LACP EtherChannel.

03. **IP Routing & Services**  
Advanced Layer 3 configurations, dynamic routing protocols, and redundancy.  
'''Key implementations:* OSPFv2 (Multi-area), EIGRP, Floating Static Routes, HSRP (First Hop Redundancy), and DHCP Server/Relay.'''

04. **IPv6 Fundamentals**  
Migration and configuration of IPv6 networks.  
'Key implementations: IPv6 SLAAC, Stateful DHCPv6, and IPv6 Static/Default routing.'

## Featured Implementation:
- **Redundant Enterprise Network (Lab 29)**  
The scenario demonstrates a resilient network architecture integrating multi-area OSPFv2 for scalable reachability, HSRP for high availability, and EtherChannel for increased bandwidth with STP path cost tuning.  
**Verification:** show standby brief, show ip ospf neighbor, show ip route.  
**Location:** 03-IP-Routing-Services/Lab29_HSRP

- **Multi-Area OSPF Scalability (Lab 28)**  
This implementation focuses on hierarchical OSPFv2 design to optimize SPF calculations and routing table size.   Includes backbone/non-backbone area management and path selection tuning through manual cost adjustments.  
**Verification:** show ip ospf database, show ip protocols.  
**Location:** 03-IP-Routing-Services/Lab28_OSPF_Part3

- **Layer 2 Convergence and Aggregation (Lab 23)**  
Emphasis on LAN stability through LACP (802.3ad) link bundling and Rapid-PVST+ for sub-second convergence.  
Deployment includes PortFast and BPDU Guard for access layer protection.  
**Verification:** show etherchannel summary, show spanning-tree.  
**Location:** 02-Ethernet-Switching/Lab23_EtherChannel

## Technical Specifications
- Environment: Cisco Packet Tracer 8.2+
- Documentation: Device running-configs are provided in .ios or .txt format for accessibility without the simulator.
- Focus: Security (ACLs/Port-Security), Scalability (VLSM/OSPF), and Reliability (FHRP/STP).

## Usage

To review a specific configuration without opening Packet Tracer:
