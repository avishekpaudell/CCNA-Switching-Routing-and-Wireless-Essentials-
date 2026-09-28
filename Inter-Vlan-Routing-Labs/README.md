
# Inter-VLAN Routing Labs

Cisco Packet Tracer labs on Inter-VLAN routing, covering how devices in different VLANs communicate through a router, how VLANs span multiple switches, and how DHCP is used across VLANs.

## Objective
- Create VLANs and assign ports to them
- Configure trunk links between switches and routers
- Enable communication between different VLANs using a router
- Extend VLANs across two switches
- Assign IP addresses to VLAN devices automatically using DHCP
- Verify connectivity between VLANs

## Files

| File | Topic |
|------|-------|
| `Inter vlan routing.pkt` | Basic Inter-VLAN routing |
| `Inter vlan routing 02.pkt` | Inter-VLAN routing (lab 2) |
| `Inter vlan routing 03pkt.pkt` | Inter-VLAN routing (lab 3) |
| `Inter vlan routing 04 with two switches.pkt` | Inter-VLAN routing with two switches |
| `Inter vlan Routing with DHCP.pkt` | Inter-VLAN routing with DHCP |

## Background

By default, devices in different VLANs cannot talk to each other, because each VLAN is a separate broadcast domain and a separate subnet. Traffic between VLANs must pass through a Layer 3 device such as a router.

### Common Inter-VLAN routing methods

| Method | Description |
|--------|-------------|
| Router-on-a-stick | One router interface is split into subinterfaces, one per VLAN, using 802.1Q encapsulation over a trunk link |
| Legacy (one link per VLAN) | A separate physical router interface is used for each VLAN |
| Layer 3 switch (SVI) | A multilayer switch routes between VLANs using switch virtual interfaces |

### Key concepts
- **Access ports** carry traffic for a single VLAN
- **Trunk ports** carry traffic for multiple VLANs using 802.1Q tagging
- Each VLAN needs its own subnet and its own default gateway
- With two switches, the link between them must be a trunk so VLANs can span both
- **DHCP** can assign IP address, subnet mask, and default gateway to hosts in each VLAN automatically

## Verification Commands

```
show vlan brief
show interfaces trunk
show ip interface brief
show ip route
show running-config
show ip dhcp binding
```

Use `ping` between PCs in different VLANs to confirm Inter-VLAN routing works. The `show ip dhcp binding` command applies to the DHCP lab.

## Tools
- Cisco Packet Tracer (8.x)
