# SRWE Labs & Assessments

A collection of Cisco Packet Tracer labs completed as part of CCNA study, covering EtherChannel link aggregation, Spanning Tree Protocol, VLANs, Inter-VLAN routing, DHCP, and practice assessments that tie everything together.

Each folder contains:
- `.pkt` topology files (open with Cisco Packet Tracer)
- `.docx` practice exam and assessment files (open with Microsoft Word)
- Fully configured devices with working connectivity, ready to explore and verify

## Tools used
- Cisco Packet Tracer (8.x)
- Microsoft Word (for assessment files)

## Index

| Folder | Topics Covered |
|--------|----------------|
| [EtherChannel-Labs](./EtherChannel-Labs) | LACP, PAgP, EtherChannel with STP, LACP with VLAN 01, port-channel trunking |
| [Inter-Vlan-Routing-Labs](./Inter-Vlan-Routing-Labs) | VLAN creation, 802.1Q trunks, router-on-a-stick, two-switch topologies, DHCP for multiple VLANs |
| [Practice Labs](./Practice%20Labs) |  Practice Exam Part 1,  Practice Lab Part 2, INT Skill Exam |
| [Final Lab](./Final%20Lab) | Final Assessment |

## Labs in detail

### EtherChannel-Labs
| Lab | Topics Covered |
|-----|----------------|
| EtherChannel LACP | LACP (IEEE 802.3ad), `active`/`passive` modes, port-channel interface |
| EtherChannel PAgP | PAgP (Cisco proprietary), `desirable`/`auto` modes |
| EtherChannel with STP (LACP) | How STP treats an LACP bundle as one logical link, root bridge and port roles |
| EtherChannel with STP (PAgP) | PAgP bundle with STP, verifying blocked and forwarding ports |
| EtherChannel-LACP with VLAN 01 | LACP bundle carrying VLAN 01 over a trunk |

### Inter-Vlan-Routing-Labs
| Lab | Topics Covered |
|-----|----------------|
| Inter VLAN Routing | Basic VLAN setup and router-on-a-stick |
| Inter VLAN Routing 02 | Additional VLANs, subinterfaces, 802.1Q encapsulation |
| Inter VLAN Routing 03 | Inter-VLAN routing practice with different addressing |
| Inter VLAN Routing 04 | Two switches connected by a trunk, VLANs spanning both switches |
| Inter VLAN Routing with DHCP | DHCP pools per VLAN, excluded addresses, `ip helper-address` |

### Practice Labs and Final Lab
- **Practice Exam Part 1**: configuration and theory practice
- **Practice Lab Part 2**: hands-on lab practice
- **INT Skill Exam**: hands-on lab practice
- **Final Assessment**: final skills assessment for the course

## Skills practiced
- Configuring EtherChannel with LACP and PAgP
- Understanding how STP interacts with link aggregation
- Creating VLANs and assigning access ports
- Configuring 802.1Q trunk links
- Router-on-a-stick Inter-VLAN routing
- Configuring DHCP for multiple VLANs
- Verifying and troubleshooting connectivity with `ping`, `show etherchannel summary`, `show vlan brief`, `show interfaces trunk`, and `show ip route`


## About
These labs were built while studying for the CCNA Switching, Routing and Wireless Essentials (SRWE), focused on hands-on configuration and verification rather than just theory.

