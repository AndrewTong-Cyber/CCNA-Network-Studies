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

## TCP/IP Model

| TCP/IP Layer | What it does | Example |
|---|---|---|
| Application | What the user sees | HTTP, DNS, FTP |
| Transport | Delivers data reliably | TCP, UDP |
| Internet | IP addressing and routing | IP |
| Link | Physical connection and MAC addresses | Ethernet, WiFi |

TCP (Transmission Control Protocol)
= Reliable, checks all data arrives (web, email, files)

UDP (User Datagram Protocol)
= Fast, does not check if data arrives (streaming, gaming)

HTTP (Hypertext Transfer Protocol)
= Protocol that loads websites

DNS (Domain Name System)
= Translates website names to IP addresses

FTP (File Transfer Protocol)
= Transfers files between computers over a network

## PDU Names (Protocol Data Unit)

| Layer | PDU Name |
|---|---|
| L4 | Segment |
| L3 | Packet |
| L2 | Frame |
| L1 | Bit |

PDUs are used every time data travels across a network

## MAC Address (Media Access Control)

- Permanent physical ID burned into every device
- Never changes unlike IP addresses
- Used to identify and send data between devices on a local network like LAN
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

I know where you live (IP) but I don't know your name (MAC) yet

| Message | Type | What it does |
|---|---|---|
| ARP Request | Broadcast | Sent to everyone asking who has this IP |
| ARP Reply | Unicast | Sent back only to the device that asked |

## MAC Address Table

- A table inside a switch that maps MAC addresses to ports
- Switch learns MAC addresses automatically as devices send data
- If destination MAC is known = sends directly to that port
- If destination MAC is unknown = floods all ports

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
