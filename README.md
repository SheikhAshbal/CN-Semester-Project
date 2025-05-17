# 🎓 Secure University Network System Design and Implementation

This project is a comprehensive network infrastructure simulation using **Cisco Packet Tracer**, designed to represent a **secure, scalable, and segmented university network**. The topology includes a main campus network, two branch campuses, a DMZ zone, WAN links, and firewall security measures.

---

## 🧠 Project Overview

- Developed a hierarchical and segmented IP-based network
- Integrated Main Campus and Branch Campus subnets
- Implemented VLAN segmentation: WLAN, LAN, DMZ, and Management
- Configured Dynamic routing and secure firewall rules
- Designed WAN/backbone links with CIDR subnets
- Documented IP planning and subnetting clearly

---

## 🗂️ IP Addressing Plan

### 🏫 Main University Network

| Category   | Network & Subnet Mask | Valid Host Addresses              | Default Gateway | Broadcast Address   |
|------------|------------------------|-----------------------------------|------------------|----------------------|
| WLAN       | 10.10.0.0/16           | 10.10.0.1 to 10.10.255.254        | 10.10.0.1        | 10.10.255.255        |
| LAN        | 172.16.0.0/16          | 172.16.0.1 to 172.16.255.254      | 172.16.0.1       | 172.16.255.255       |
| Management | 192.168.10.0/24        | 192.168.10.1 to 192.168.10.254    | 192.168.10.1     | 192.168.10.255       |
| DMZ        | 10.20.20.0/27          | 10.20.20.1 to 10.20.20.30         | 10.20.20.1       | 10.20.20.31          |

### 🏢 Branch Campus Network

| Category | Network & Subnet Mask | Valid Host Addresses               | Default Gateway | Broadcast Address    |
|----------|------------------------|------------------------------------|------------------|-----------------------|
| WLAN     | 10.11.0.0/16           | 10.11.0.1 to 10.11.255.254         | 10.11.0.1        | 10.11.255.255         |
| LAN      | 172.17.0.0/16          | 172.17.0.1 to 172.17.255.254       | 172.17.0.1       | 172.17.255.255        |

---

## 🌐 WAN/Backbone Links

| No. | Link Description                   | Network Address     | Subnet Mask         |
|-----|------------------------------------|----------------------|----------------------|
| 1   | CLOUD Area (General Internet)      | 8.0.0.0              | 255.0.0.0            |
| 2   | HQ-ISP Internet Link               | 20.20.20.0/30        | 255.255.255.252      |
| 3   | Branch-ISP Internet Link           | 30.30.30.0/30        | 255.255.255.252      |
| 4   | HQ Firewall - ISP Link             | 105.100.50.0/30      | 255.255.255.252      |
| 5   | Branch Firewall - ISP Link         | 205.200.100.0/30     | 255.255.255.252      |
| 6   | HQ Firewall to MLSW1 Link          | 10.20.20.32/30       | 255.255.255.252      |
| 7   | HQ Firewall to MLSW2 Link          | 10.20.20.36/30       | 255.255.255.252      |
| 8   | Branch Firewall to MLSW1 Link      | 10.20.20.40/30       | 255.255.255.252      |
| 9   | Branch Firewall to MLSW2 Link      | 10.20.20.44/30       | 255.255.255.252      |
| 10  | HQ Firewall to DMZ                 | 10.20.20.0/27        | 255.255.255.224      |

---


## 🧑‍🤝‍🧑 Team Members

- Ashbal Shaikh 
- Hiba Imran  
- Rahul Kumar  
- Altaf Samejo  
- M. Raza Abbas  

---



## 🙏 Acknowledgment

Special thanks to our instructor for insightful guidance and practical lab support in designing this network infrastructure.

---


