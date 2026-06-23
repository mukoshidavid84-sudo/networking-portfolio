# Project 4: Inter-VLAN Routing Using Router-on-a-Stick

## Objective
To configure Inter-VLAN routing between VLAN 10 (HR) and VLAN 20 (IT) using a router connected to a switch.

## Devices Used
- 1 Cisco 2960 Switch
- 1 Cisco 1941 Router
- 4 PCs

## VLAN Configuration
- VLAN 10 → HR Department (PC0, PC1)
- VLAN 20 → IT Department (PC2, PC3)

## Switch Configuration
- Ports Fa0/1 - Fa0/2 assigned to VLAN 10
- Ports Fa0/3 - Fa0/4 assigned to VLAN 20
- Fa0/24 configured as trunk port

## Router Configuration
- Subinterface g0/0.10 → VLAN 10 (192.168.10.1/24)
- Subinterface g0/0.20 → VLAN 20 (192.168.20.1/24)
- 802.1Q encapsulation used for VLAN tagging

## IP Addressing
HR VLAN:
- PC0 → 192.168.10.10
- PC1 → 192.168.10.11
Gateway: 192.168.10.1

IT VLAN:
- PC2 → 192.168.20.10
- PC3 → 192.168.20.11
Gateway: 192.168.20.1

## Testing
- Successful ping within VLANs
- Successful communication between VLAN 10 and VLAN 20
- Initial packet loss observed due to ARP resolution

## Conclusion
This project demonstrated Inter-VLAN Routing using router-on-a-stick configuration, allowing communication between separate VLANs while maintaining network segmentation.
