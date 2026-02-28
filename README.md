# Network-Engineering-Works

A growing collection of my day-by-day learning notes and hands-on work in **networking** and **telecommunications**—focused on practical skills (CCNA-level concepts, switching, VLANs, VPNs, and VoIP).

---

## Day 1 — Getting Started with VLANs (Virtual LANs)

As I continue diving deeper into networking, one of the key concepts I explored is **VLANs (Virtual Local Area Networks)**—a powerful way to segment and manage networks.

### What is a VLAN?
A VLAN lets you create **multiple logical networks on a single physical switch**. Devices in the same VLAN behave as if they’re on the same separate switch/network, even when spread across multiple switches (using trunks), while staying isolated from other VLANs.

### Why use VLANs?
- **Better security**: separate departments/roles (e.g., HR vs Engineering)
- **Reduced congestion**: smaller broadcast domains
- **Easier management**: cleaner design and simpler troubleshooting in enterprise networks

### Basic VLAN configuration (Cisco switch example)

```text
Switch> enable
Switch# configure terminal
Switch(config)# vlan 10
Switch(config-vlan)# name HR
Switch(config-vlan)# exit

Switch(config)# interface fastEthernet 0/1
Switch(config-if)# switchport mode access
Switch(config-if)# switchport access vlan 10
Switch(config-if)# exit
```

**Notes:**
- VLAN IDs range from **1–4094**.
- Access ports connect end devices (PCs, printers, phones).
- To allow communication **between VLANs**, you need **Inter-VLAN Routing** via a **router** (Router-on-a-Stick) or a **Layer 3 switch**.

**Lab Snapshot (Day 1):**  
![VLAN Lab](https://github.com/user-attachments/assets/cdbfa4de-915e-4728-b765-d71541486a2c)

**Tags:** `#Networking` `#VLAN` `#CCNA` `#Cisco` `#ITInfrastructure` `#Cybersecurity`

---

## Day 2 — VPN + VoIP Basics (SIP vs ATA)

Recently I gained hands-on exposure to **VPN installations** and **VoIP setup**, and I learned how both fit into modern network environments.

### VPN Installations
I practiced installing and configuring **VPNs (Virtual Private Networks)** so users can connect securely to internal systems from remote locations. This included:
- installing the VPN client
- configuring authentication
- testing the secure tunnel and access to internal resources

### VoIP Phones — SIP vs ATA
I also worked on VoIP provisioning and learned the difference between two common endpoint types:

**SIP Phones**
- Digital IP phones that connect directly to the network
- Tasks I practiced:
  - patching the correct switch ports
  - provisioning devices
  - assigning phones to users using SIP credentials

**ATA Devices (Analog Telephone Adapter)**
- Used to connect traditional analog phones to a VoIP system
- Tasks I practiced:
  - tracking the Telephone Number (TN) / line mapping
  - connecting and validating ATA registration
  - ensuring protection (e.g., lightning protection) to avoid electrical damage

This was a great learning experience—seeing how modern IP telephony works while still supporting legacy analog devices.

**Lab Snapshot (Day 2):**  
![VoIP / ATA Notes](https://github.com/user-attachments/assets/94b647b9-9734-4caa-968a-592963c4e54c)

**Tags:** `#LearningByDoing` `#VoIP` `#VPN` `#Networking` `#SIP` `#ATA` `#Telecom`

---

## Roadmap (Next Topics to Explore)
- Trunk ports (802.1Q) and VLAN propagation
- Inter-VLAN routing (Router-on-a-Stick vs L3 switch SVIs)

