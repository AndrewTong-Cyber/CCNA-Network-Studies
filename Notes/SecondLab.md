## OSI Model — 7 Layers

| Number | Layer |
|---|---|
| 7 | Application |
| 6 | Presentation |
| 5 | Session |
| 4 | Transport |
| 3 | Network |
| 2 | Data Link |
| 1 | Physical |

**Memory trick:**
> All People Seem To Need Data Processing

## TCP/IP Model — What Each Layer Does

| Layer | Name | What it does |
|---|---|---|
| L1 | Physical | Sends raw bits as electrical or radio signals |
| L2 | Data Link | Device to device communication using MAC addresses |
| L3 | Network | IP addressing and routing between networks |
| L4 | Transport | Delivers data reliably (TCP/UDP) |

TCP (Transmission Control Protocol)
= Reliable, slower, makes sure all data arrives correctly
= Used when accuracy matters (web browsing, email, file transfers)

UDP (User Datagram Protocol)
= Fast, less reliable, does not check if data arrives
= Used when speed matters more (video streaming, gaming, voice calls)

## PDU Names (Power distribution unit)

| Layer | PDU Name |
|---|---|
| L4 | Segment |
| L3 | Packet |
| L2 | Frame |
| L1 | Bit |

PDUs are used every time data travels across a network

## MAC Address

- Physical address burned into every device
- Never changes unlike IP addresses
- 6 bytes / 48 bits long
- First 3 bytes = company who made it (OUI)
- Last 3 bytes = unique to that specific device
- Example: AA:BB:CC:DD:EE:FF

## Ethernet Frame

- Think of it like an envelope carrying your data
- Contains source MAC address, destination MAC address, and data
- Switch uses this to know where to send data

## Key Terms

| Term | Simple definition |
|---|---|
| Unicast | Data sent to one specific device |
| Broadcast | Data sent to all devices on network |
| Unknown Unicast | Switch doesn't know destination so it floods everyone |
| Flood | Switch sends frame out all ports except the one it came in on |

## ARP (Address Resolution Protocol)

- ARP finds the MAC address of a known IP address
- Used when a device knows the IP but not the MAC

| Message | Type | What it does |
|---|---|---|
| ARP Request | Broadcast | Sent to everyone asking who has this IP |
| ARP Reply | Unicast | Sent back only to the device that asked |

## MAC Address Table

- Switch keeps a table of which MAC address is on which port
- When a frame arrives switch learns where that device is
- Next time it knows exactly where to send data
- If destination is unknown switch floods all ports

## Ping

- Tests if a device is reachable on the network
- Uses two messages:

| Message | What it means |
|---|---|
| ICMP Echo Request | Are you there? |
| ICMP Echo Reply | Yes I am here! |

- Command: ping (ip-address)

## LAN vs Switch vs Router

| Device | Role |
|---|---|
| Switch | Connects devices WITHIN a LAN |
| Router | Connects DIFFERENT LANs together |
| LAN | Small local network like home or office |

- Switches do NOT separate LANs
- Routers are used to connect separate LANs
