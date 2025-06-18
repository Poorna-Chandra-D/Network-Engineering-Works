# Network-Engineering-Works

Day 1

🔌 Getting Started with VLANs — A Quick Guide! 🌐

As I continue diving deeper into networking, one of the key concepts I’ve explored is VLAN (Virtual Local Area Network) — and it's a game changer for network segmentation and management!
💡 So, what exactly is a VLAN?
Think of it as creating multiple virtual networks within a single physical switch. Devices on the same VLAN can communicate as if they're on their own private network, even across switches — while staying isolated from others.

🎯 Why VLANs?
✅ Better security (limit access between departments)
✅ Reduced network congestion (smaller broadcast domains)
✅ Easier to manage (especially in enterprise setups)
🔧 How to create a VLAN on a Cisco Switch:

Switch> enable
Switch# configure terminal
Switch(config)# vlan 10
Switch(config-vlan)# name HR
Switch(config-vlan)# exit
Switch(config)# interface FastEthernet 0/1
Switch(config-if)# switchport mode access
Switch(config-if)# switchport access vlan 10
Switch(config-if)# exit

📍Each port is assigned to a VLAN using a unique ID (1–4094).
🔁 Want devices in different VLANs to talk?
 You’ll need a router or Layer 3 switch — this is known as Inter-VLAN Routing or Router-on-a-Stick.
hashtag#Networking hashtag#VLAN hashtag#CCNA hashtag#Cisco hashtag#ITInfrastructure hashtag#TechLearning hashtag#NetworkEngineer hashtag#BeginnersGuide hashtag#LabLife hashtag#Cybersecurity

![image](https://github.com/user-attachments/assets/cdbfa4de-915e-4728-b765-d71541486a2c)
