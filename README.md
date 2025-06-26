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

Day 2

🔧 New Skills I’ve Recently Learned 📞💻

I've been gaining some hands-on experience with voice and network systems recently, and I wanted to share a few things I’ve learned along the way:

🔐 VPN Installations
I learned how to install and configure VPNs (Virtual Private Networks) to help users connect securely to internal systems from remote locations. This includes setting up the VPN client, making sure it's authenticated properly, and testing the secure connection.

📞 VoIP Phones – SIP vs ATA
I’ve also worked on setting up VoIP (Voice over IP) phones, and I got to understand the difference between two common types:

SIP Phones: These are digital IP phones that connect directly to the network. I learned how to patch the correct ports, provision the phones, and assign them to users using SIP credentials.

ATA Devices (Analog Telephone Adapters): These are used to convert traditional analog phones (POTS lines) to work over VoIP. I worked on tracking the Telephone Number (TN) of the analog line, connecting the ATA, and making sure the setup is protected using lightning protection to avoid electrical damage.

⚡ It’s been a great learning journey—seeing how modern phone systems work, and how older technologies are being integrated into today’s networks.

Excited to keep learning and growing in the world of IT and telecommunications!

#LearningByDoing #VoIP #VPN #Networking #SIP #ATA #ITSkills #Telecom #HandsOnExperience #EntryLevelEngineer

![image](https://github.com/user-attachments/assets/94b647b9-9734-4caa-968a-592963c4e54c)


