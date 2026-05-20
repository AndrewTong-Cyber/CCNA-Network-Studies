# Lab 02 - Ethernet LAN Switching

**Topics:** MAC address tables, ARP, Ping, 
Unicast vs Broadcast, Switch learning process

**File:** Lab_02.pkt

**What I did:** Built a network with 2 switches and 
4 PCs. Used ping to generate traffic and watched 
switches learn MAC addresses automatically. 
Viewed MAC address tables on both switches using 
the show mac address-table command. Practiced 
using CLI commands on switches for the first time.

## Screenshots

**PC1 pinged PC3 successfully (0% loss)**

<img width="795" height="459" alt="ping-pc1-to-pc3" src="https://github.com/user-attachments/assets/2da1d6ba-5664-4059-b5b9-276458abde54" />

**PC2 pinged PC4 successfully (0% loss)**

<img width="646" height="426" alt="ping-pc2-to-pc4" src="https://github.com/user-attachments/assets/d844ae23-0c29-471e-b13e-fde77f892d00" />

**SW1 MAC address table populated with 4 devices**
<img width="934" height="426" alt="sw1-mac-table" src="https://github.com/user-attachments/assets/1ac87bae-7b43-413a-b0b3-d3babd84c6d6" />

**For example Fa0/2 Port would belong to PC2**

**SW2 MAC address table populated with 2 devices**
<img width="934" height="426" alt="sw2-mac-table" src="https://github.com/user-attachments/assets/5eec02e9-3aa0-4112-a5ad-eccf36144869" />
