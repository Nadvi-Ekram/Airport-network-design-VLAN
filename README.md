# ✈️ Airport Network Design Using VLANs

A segmented airport network built in **Cisco Packet Tracer** using **VLANs** and **Router-on-a-Stick inter-VLAN routing**, with centralised DHCP, DNS and Web services and wireless access for passengers.

![Cisco Packet Tracer](https://img.shields.io/badge/Cisco-Packet%20Tracer-1BA0D7?logo=cisco&logoColor=white)
![Networking](https://img.shields.io/badge/Topic-VLAN%20%7C%20Inter--VLAN%20Routing-informational)

---

## 🗺️ Topology

![Full topology](Full%20topology.png)

## 📌 Project summary

| | |
|---|---|
| **Topic** | Airport network segmentation using VLANs |
| **Technique** | Router-on-a-Stick inter-VLAN routing (802.1Q sub-interfaces) |
| **Tool** | Cisco Packet Tracer |
| **VLANs** | 7: Admin, Check-In, Security, Baggage, ATC, Server, WiFi |
| **Devices** | 1 Router, 2 Switches, 10 PCs, 3 Servers, 1 Access Point |

## 🔧 What's configured

- **VLAN segmentation** so that each airport department is isolated in its own broadcast domain
- **802.1Q trunking** between the switches and the router
- **Router-on-a-Stick**, where one physical router interface is split into sub-interfaces to route between VLANs
- **Centralised DHCP server** handing out addresses to every VLAN (with DHCP relay / helper addresses)
- **DNS and Web servers** in a dedicated Server VLAN
- **Wireless access point** on a separate WiFi VLAN for passengers

## ✅ Testing

- Ping tests within and between VLANs
- DHCP address assignment verified on every end device
- Web page access by domain name through the DNS server

Full test results are in the lab report.

## 📁 Files

| File | Contents |
|---|---|
| `Airport Network Design.pkt` | Packet Tracer project file |
| `Full topology.png` | Topology screenshot |
| `Airport_Network_Lab_Report_GitHub.pdf` | Full lab report (design, implementation, testing) |

## ▶️ How to open

1. Install [Cisco Packet Tracer](https://www.netacad.com/cisco-packet-tracer) (free with a NetAcad account)
2. Download `Airport Network Design.pkt`
3. Open it in Packet Tracer and explore the devices, VLANs and configurations

---

📍 CSE342.2 Computer Networking Lab, **Southeast University**
