# 📡 Enterprise Network Design for RIS Tech (Cisco Packet Tracer)

## 📌 Project Overview
This project demonstrates the design and implementation of a scalable and secure enterprise network for a robotics company, RIS Tech, using Cisco Packet Tracer.

The network connects multiple departments across a Headquarters (HQ) and a Remote Branch, implementing real-world networking concepts including VLANs, routing, NAT, VoIP, and security.

---

## 🏢 Network Architecture

### 🔹 Headquarters (HQ)
- VLAN-based departmental segmentation:
  - VLAN 10 – Administration
  - VLAN 20 – Sales
  - VLAN 30 – HR
  - VLAN 40 – R&D
  - VLAN 50 – Public
  - VLAN 60 – Voice
- Router-on-a-Stick for Inter-VLAN routing
- Centralized services (DHCP, DNS, HTTP, FTP)

### 🔹 Branch Network
- Connected to HQ via routers
- Uses RIP for communication with HQ
- Uses default routing to access Internet via HQ

---

## 🚀 Key Features

- VLAN segmentation for departments
- Inter-VLAN routing using subinterfaces
- OSPF (HQ internal routing)
- RIP (HQ ↔ Branch communication)
- DHCP for automatic IP allocation
- NAT (PAT Overload) for Internet access
- VoIP communication using IP Phones and Dial Peers
- DNS, HTTP, FTP servers
- ACLs for network security

---

## 🌐 IP Addressing Scheme

| VLAN | Department | Subnet |
|------|------------|--------|
| 10 | Administration | 192.168.146.0/24 |
| 20 | Sales | 192.168.94.0/24 |
| 30 | HR | 192.168.129.0/24 |
| 40 | R&D | 192.168.126.0/24 |
| 50 | Public | 192.168.1.0/24 |
| 60 | Voice | 192.168.60.0/24 |

Public IP (NAT): **203.0.114.1**

---

## 📞 VoIP Implementation

- IP Phones configured in all departments
- Voice VLAN (VLAN 60)
- Inter-branch calling using Dial Peers
- Numbering plan configured using ephone-dn

---

## 🔐 Security

- ACLs implemented to restrict inter-department access
- VLAN isolation
- NAT hides internal addressing

---

## 🧪 Testing & Verification

- Inter-VLAN communication (ping)
- Internet access using NAT
- DNS resolution
- HTTP and FTP server access
- VoIP calling between branches
- ACL restrictions tested

---

## 📷 Screenshots

<img width="975" height="382" alt="image" src="https://github.com/user-attachments/assets/fac3bbaa-11dd-4e71-85fe-ab82d73a7017" />

<img width="659" height="350" alt="image" src="https://github.com/user-attachments/assets/9d5a4677-c83a-49b2-818a-873984bb63a8" />

<img width="729" height="421" alt="image" src="https://github.com/user-attachments/assets/1e0c7cac-c0c5-45f6-bd80-a2ab77e33f98" />

<img width="409" height="472" alt="image" src="https://github.com/user-attachments/assets/85a6dd65-7979-4396-ae2f-42ff211708bb" />








---

## ⚠️ Note

The complete Packet Tracer (.pkt) file is not publicly shared to maintain originality and prevent direct duplication.

However, all configurations, screenshots, and explanations are provided. The project can be fully demonstrated and explained if required.

---

## 🧠 Learning Outcomes

- Enterprise network design
- VLAN & Inter-VLAN routing
- OSPF & RIP routing protocols
- NAT and IP addressing
- VoIP configuration
- Network security using ACLs

---

## 👩‍💻 Author

Ramsha Shafique
