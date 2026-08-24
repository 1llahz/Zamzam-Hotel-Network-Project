🏨 Zamzam Hotel Network Project



A complete multi-floor hotel network design and simulation, built using Cisco Packet Tracer . This project demonstrates a scalable, secure, and well-segmented network infrastructure covering all major hotel departments across 3 floors.



\---



&#x20;📌 Project Overview



This project simulates the full network infrastructure of a hotel, covering departments such as Sales, HR, Finance, IT, Admin, Reception, Logistics, and Store, spread across 1st, 2nd, and 3rd floors . It demonstrates core networking concepts including VLAN segmentation, inter-VLAN routing, subnetting, wireless connectivity, and end-device configuration.



\---

&#x20;🖥️ Tools Used



\- Cisco Packet Tracer – Network design and simulation

\- Cisco 2911 Routers, 2960-24TT Switches

\- PCs, Printers, Laptops, Tablets, Smartphones, Wireless Access Points



\---



🏗️ Network Architecture



The hotel network is split across 3 floors , each connected to a router (F1.Router, F2.Router, F3.Router) and interconnected via serial WAN links. Each department sits on its own VLAN for traffic segmentation and security.



Floor Layout:

\- \*\*2nd Floor (F2.Router)\*\* – Sales, HR, Finance departments

\- \*\*3rd Floor (F3.Switch)\*\* – IT, Admin departments

\- \*\*1st Floor (F1.Router)\*\* – Reception, Logistic, Store departments



Router Interconnection (Serial WAN Links):

| Link | Subnet |

|---|---|

| F2.Router ↔ F3 side | 10.10.10.0/30 |

| F2.Router ↔ F1 side | 10.10.10.4/30 |

| F1.Router ↔ F2.Router (Se0/1/0 – Se0/2/0) | 10.10.10.8/30 |



\---



🔑 Key Features



\- ✅ VLAN segmentation for every department (8 VLANs)

\- ✅ Inter-VLAN and inter-floor routing

\- ✅ Wireless Access Points for Sales, Admin, and Logistic areas

\- ✅ Mixed end-device types: PCs, Printers, Laptop, Tablet, Smartphone

\- ✅ Serial WAN links connecting the 3 floor routers

\- ✅ Scalable design for future department/floor expansion



\---



\## 🗺️ Network Topology



!\[Network Topology](screenshots/hotel-topology.png)



\---



&#x20;📸 Screenshots



&#x20;Full Network Topology

!\[Topology](screenshots/hotel-topology.png)



&#x20;VLAN Configuration

!\[VLAN Configuration](screenshots/vlan-configuration.png)



&#x20;Device/Router Configuration

!\[Configuration](screenshots/configuration.png)



\---



🌐 VLAN \& IP Addressing Scheme



| Department | VLAN ID | Subnet | Floor |

|---|---|---|---|

| IT | 10 | 192.168.1.0/24 | 3rd Floor |

| Admin | 20 | 192.168.2.0/24 | 3rd Floor |

| Finance | 30 \*(port Fa0/8)\* | 192.168.4.0/24 | 2nd Floor |

| HR | 30 | 192.168.4.0/24 | 2nd Floor |

| Finance | 40 | 192.168.3.0/24 | 2nd Floor |

| Sales | 50 | 192.168.5.0/24 | 2nd Floor |

| Logistic | 60 | 192.168.6.0/24 | 1st Floor |

| Store | 70 | 192.168.7.0/24 | 1st Floor |

| Reception | 80 | 192.168.8.0/24 | 1st Floor |





\---

⚙️ How to Run This Project



1\. Download and install \[Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer).

2\. Clone or download this repository.

3\. Open `HOTEL PROJECT.pkt` (included in this repository).

4\. Explore the topology, check device/VLAN configurations, and test connectivity using `ping` or `traceroute` between departments.



\---



📁 Repository Structure



```

HOTEL MNG/

│

├── HOTEL PROJECT.pkt               # Main Packet Tracer project file

├── screenshots/                    # Screenshots folder

│   ├── hotel-topology.png

│   ├── vlan-configuration.png

│   └── configuration.png

└── README.md                       # Project documentation

```



\---



👤 Author



Aisha Hassan

Networking Student | Cisco Packet Tracer Enthusiast



\---



&#x20;📄 License



This project is for educational purposes.

