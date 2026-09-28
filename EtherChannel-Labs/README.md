# EtherChannel Labs

Cisco Packet Tracer labs on EtherChannel (link aggregation), covering LACP, PAgP, and EtherChannel used together with Spanning Tree Protocol and VLANs.

## Objective
- Bundle multiple physical links between switches into a single logical link
- Compare LACP and PAgP negotiation protocols
- See how EtherChannel works together with Spanning Tree Protocol
- Use EtherChannel with VLANs and trunking
- Verify the bundle using show commands

## Files

| File | Topic |
|------|-------|
| `Etherchannel LACP.pkt` | EtherChannel using LACP |
| `Etherchannel PAgp.pkt` | EtherChannel using PAgP |
| `Etherchannel with STP (Lacp).pkt` | EtherChannel (LACP) with Spanning Tree Protocol |
| `Etherchannel with STP (PaGp).pkt` | EtherChannel (PAgP) with Spanning Tree Protocol |
| `Etherchannel-LACP with VLAN 01.pkt` | EtherChannel (LACP) with VLAN 01 |

## Background

EtherChannel groups several physical Ethernet links into one logical link called a port-channel. This increases available bandwidth, adds redundancy, and allows Spanning Tree Protocol to treat the bundle as a single link, so the member links are not blocked individually.

### LACP vs PAgP

| | LACP | PAgP |
|---|------|------|
| Standard | IEEE 802.3ad (open standard) | Cisco proprietary |
| Modes | `active`, `passive` | `desirable`, `auto` |
| Multi-vendor support | Yes | Cisco devices only |

### Rules for forming a bundle
- Both sides must use the same protocol (LACP with LACP, PAgP with PAgP)
- Modes must be compatible: `active` with `active` or `passive`, `desirable` with `desirable` or `auto`
- Member ports must match in speed, duplex, and switchport mode
- Two `passive` or two `auto` ports will not form a bundle, since neither side starts negotiation

## Verification Commands

```
show etherchannel summary
show etherchannel port-channel
show interfaces trunk
show spanning-tree
show vlan brief
show running-config
```

In `show etherchannel summary`, a port-channel marked `SU` is a working Layer 2 bundle, and member ports marked `P` are bundled into it.

## Tools
- Cisco Packet Tracer (8.x)
