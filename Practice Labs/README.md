# Practice Labs

Practice exams and lab documentation completed while studying for CCNA Introduction to Networks (ITN) and CCNA Switching, Routing and Wireless Essentials (SRWE). Each document walks through the configuration device by device, with Packet Tracer screenshots, an explanation of the commands, and the errors that came up along the way.

## Tools used
- Cisco Packet Tracer (8.x)

## Index

| File | Topics Covered |
|------|----------------|
| ITN Practice Skills Assessment | IPv4 subnetting (/27 and /28), IPv4/IPv6 dual stack, router hardening, SSH, Telnet on a switch, host addressing |
| SRWE Practice Exam Part 1 | LACP EtherChannels, trunking, VLANs, SVI inter-VLAN routing on a Layer 3 switch, router-on-a-stick, SSH, static routes |
| SRWE Practice Lab Part 2 | Port security, DHCP snooping, Dynamic ARP Inspection, PortFast and BPDU Guard, static and floating static routes (IPv4/IPv6), DHCP server and client, wireless verification |

## Labs in detail

### ITN Practice Skills Assessment
One router (CS Department) with two LANs, LAB 124-C and LAB 214-A.
- **Subnetting:** two passes over 192.168.1.0/24, first 30 hosts per subnet (/27), then 14 hosts per subnet (/28) carved from one of the /27 blocks
- **Router:** hostname, encrypted enable secret, secured console and VTY lines, minimum password length, MOTD banner, SSH with a 1024-bit RSA key and a local user
- **Interfaces:** IPv4 and IPv6 addressing on both Gigabit interfaces, with link-local addresses and descriptions
- **Switch:** Telnet management with a VLAN 1 SVI and default gateway
- **Hosts and server:** IPv4 and IPv6 addressing, with the router link-local address as the IPv6 default gateway

### SRWE Practice Exam Part 1
A two-LAN topology behind one edge router.
- **Sciences LAN:** a Layer 3 switch and two access switches carrying VLANs 10, 20 and 30, routed with SVIs
- **Arts LAN:** one access switch carrying VLANs 40, 50 and 60 plus a management VLAN 99, routed with router-on-a-stick subinterfaces
- Three LACP EtherChannels between the switches, configured as trunks
- Routed link between the Layer 3 switch and the edge router, and a WAN link to the ISP
- SSH management, passwords, banners, and static routes
- Error reference with the problems that came up and how they were fixed

### SRWE Practice Lab Part 2
A multi-site topology with two HQ LANs, a Remote Office, a Remote Branch with a wireless AP, and an ISP router.
- **Switch hardening:** VLANs, port security, DHCP snooping, Dynamic ARP Inspection, PortFast with BPDU Guard, and unused ports moved to a dedicated VLAN and shut down
- **Routing:** static and floating static routes in both IPv4 and IPv6 on the Central and Branch routers
- **DHCP:** router-on-a-stick with a DHCP pool for the branch LAN, while the same router gets its WAN address as a DHCP client
- **Wireless:** laptop association with the access point in infrastructure mode

## Skills practiced
- Designing an IPv4 addressing scheme with subnetting
- Configuring dual-stack IPv4/IPv6 interfaces and hosts
- Device hardening and SSH configuration
- Building LACP EtherChannels and trunks between switches
- Inter-VLAN routing with SVIs and with router-on-a-stick
- Layer 2 security: port security, DHCP snooping, DAI, PortFast, BPDU Guard
- Static and floating static routing for IPv4 and IPv6
- Configuring a router as both DHCP server and DHCP client
- Troubleshooting from real command errors and verifying with show commands

## About
These documents were created while studying for the CCNA Introduction to Networks (ITN) and Switching, Routing and Wireless Essentials (SRWE), focused on hands-on configuration and verification rather than just theory.
