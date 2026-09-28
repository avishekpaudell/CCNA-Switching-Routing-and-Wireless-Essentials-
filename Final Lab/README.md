
# Final Lab

Final Packet Tracer assessment for CCNA Switching, Routing and Wireless Essentials (SRWE). One router (R1) and two switches (S1, S2) support two VLANs of hosts plus a management VLAN, with dual-stack IPv4/IPv6.

## Tools used
- Cisco Packet Tracer (8.x)
- Microsoft Word (for the documentation file)

## Index

| Part | Topics Covered |
|------|----------------|
| Part 1 | Physical build: rack the devices, place the PCs, cable the topology |
| Part 2 | Hardening on R1, S1, S2 (hostname, banner, passwords, SSH), R1 loopback and subinterfaces, switch management SVIs |
| Part 3 | VLANs and trunking with native VLAN 6, Layer 2 EtherChannel between S1 and S2, static access ports with port security, unused ports parked in VLAN 5 |
| Part 4 | Default routes to Loopback0, two DHCP pools, host addressing (DHCP for IPv4, static for IPv6) |

## Labs in detail

### Part 1: Build the network
Main Wiring Closet in Physical Mode: rack with power distribution device, R1, S1 and S2, and PC-A and PC-B cabled up to the rack.

### Part 2: Initial settings and hardening
- Hostname, MOTD banner, minimum password length of 10, encrypted enable secret, service password-encryption
- Console and VTY passwords
- SSH with a local user account on all three devices
- R1 loopback and subinterfaces, and a management SVI on each switch

### Part 3: VLANs, trunking and EtherChannel
- Trunk ports on native VLAN 6
- LACP EtherChannel between S1 and S2
- Access ports with port security
- Unused ports assigned to VLAN 5 and shut down

### Part 4: Host support
- Default routes on R1 pointing to Loopback0
- DHCP pools `CCNA-A` (VLAN 2) and `CCNA-B` (VLAN 3)
- Hosts addressed with DHCP for IPv4 and static addressing for IPv6

## Skills practiced
- Building a physical topology in Packet Tracer
- Device hardening and SSH configuration
- Trunking, native VLANs, and LACP EtherChannel
- Port security and securing unused ports
- Router subinterfaces, default routes, and DHCP pools
- Dual-stack IPv4/IPv6 addressing
- Troubleshooting from real command errors, such as the EtherChannel and native VLAN mismatches

## About
This assessment was completed while studying for the CCNA Switching, Routing and Wireless Essentials (SRWE), focused on hands-on configuration and verification rather than just theory.
