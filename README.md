# 🖧 Small Business DHCP Network
### Cisco Packet Tracer | Cisco IOS | DHCP | IPv4 Networking

---

# 📌 Project Overview

![Project Overview](images/00-Project-Overview.png)

This project demonstrates the design, configuration, and verification of a **Small Business Local Area Network (LAN)** using **Cisco Packet Tracer**.

The network simulates a small office environment consisting of one Cisco router, one Cisco switch, an Internet cloud for topology representation, and twelve client computers representing multiple business departments.

The Cisco router was configured as a **DHCP server**, allowing all client devices to automatically obtain their IPv4 configuration instead of requiring manual static addressing.

This project was completed as part of my hands-on networking practice while preparing for the **Bachelor of Science in Cybersecurity and Information Assurance at Western Governors University (WGU)** and the **CompTIA Network+ certification**.

---

# 📑 Table of Contents

- [Project Overview](#-project-overview)
- [Project Objectives](#-project-objectives)
- [Business Scenario](#-business-scenario)
- [Network Topology](#-network-topology)
- [Devices Used](#-devices-used)
- [Network Information](#-network-information)
- [Router Configuration](#️-router-configuration)
- [DHCP Client Configuration](#-dhcp-client-configuration)
- [Network Verification](#-network-verification)
- [Connectivity Testing](#-connectivity-testing)
- [Skills Demonstrated](#-skills-demonstrated)
- [What I Learned](#-what-i-learned)
- [Repository Contents](#-repository-contents)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---

# 🎯 Project Objectives

The objectives of this lab were to:

- Design a small business LAN.
- Configure a Cisco router using the Cisco IOS Command-Line Interface (CLI).
- Configure the router as a DHCP server.
- Automatically assign IPv4 addresses to client devices.
- Verify DHCP functionality.
- Test end-to-end network connectivity.
- Practice documenting a networking project using GitHub.

---

# 🏢 Business Scenario

**Company:** BlueWave Consulting

BlueWave Consulting is a small business with twelve employees distributed across multiple departments.

Departments included in this project:

- Reception
- Management
- Accounting
- Sales
- Human Resources
- IT
- Shared Devices

The goal was to create a network where every workstation automatically receives its IP configuration through DHCP while allowing all devices to communicate successfully.

---

# 🌐 Network Topology

![Network Topology](images/01-Small-Business-Topology.png)

---

# 🖥️ Devices Used

| Device | Quantity |
|---------|---------:|
| Cisco 1941 Router | 1 |
| Cisco 2960-24TT Switch | 1 |
| Cloud-PT (Internet) | 1 |
| Desktop PCs | 12 |

---

# 🌍 Network Information

| Configuration | Value |
|--------------|-------|
| Network Address | 192.168.10.0/24 |
| Router IP Address | 192.168.10.1 |
| Default Gateway | 192.168.10.1 |
| DHCP Scope | 192.168.10.10 – 192.168.10.254 |
| DNS Server | 8.8.8.8 |

---

# ⚙️ Router Configuration

The Cisco 1941 router was configured to:

- Assign a hostname
- Configure the GigabitEthernet interface
- Assign the LAN IP address
- Exclude reserved IP addresses
- Create a DHCP pool
- Configure the default gateway
- Configure the DNS server
- Save the running configuration

### Router Configuration

![Router Configuration](images/02-Router-DHCP-Configuration.png)

---

# 💻 DHCP Client Configuration

Each workstation was configured to automatically obtain an IP address from the DHCP server.

Each client successfully received:

- IP Address
- Subnet Mask
- Default Gateway
- DNS Server

![PC DHCP Configuration](images/03-PC-DHCP-Configuration.png)

---

# ✅ Network Verification

The following Cisco IOS commands were used to verify the network configuration:

```text
show ip interface brief
show ip dhcp pool
show ip dhcp binding
```

These commands verified:

- Router interface status
- Active DHCP pool
- DHCP address assignments
- Operational network interfaces

![Router Verification](images/04-Router-Verification-Commands.png)

---

# 📡 Connectivity Testing

### Ping Test to the Router

The client computer successfully communicated with the default gateway.

![Ping Router](images/05-Ping-Router-Success.png)

---

### End-to-End Device Communication

Client devices successfully communicated with each other, confirming proper DHCP configuration and Layer 3 connectivity.

![PC to PC Communication](images/06-PC-to-PC-Success.png)

---

# 🧠 Skills Demonstrated

This project allowed me to practice and strengthen the following networking skills:

- Cisco Packet Tracer
- Cisco IOS Command-Line Interface (CLI)
- Router Configuration
- DHCP Configuration
- IPv4 Addressing
- LAN Design
- Switch Connectivity
- DHCP Verification
- Connectivity Testing
- Basic Network Troubleshooting
- Technical Documentation
- GitHub Project Organization

---

# 📚 What I Learned

Completing this project helped me better understand how a small business network operates and how DHCP simplifies network administration.

Key takeaways include:

- Designed and documented a small business LAN topology.
- Configured a Cisco router using the Cisco IOS CLI.
- Configured the router to function as a DHCP server.
- Learned how DHCP automatically assigns IP addresses, subnet masks, default gateways, and DNS settings to client devices.
- Configured twelve computers to receive network settings dynamically.
- Verified router interfaces and DHCP leases using Cisco verification commands.
- Confirmed successful communication between devices using the `ping` command.
- Strengthened my understanding of IPv4 addressing, subnet masks, default gateways, and DNS configuration.
- Practiced basic troubleshooting by verifying interface status and testing network connectivity.
- Improved my technical documentation skills by organizing and presenting the project on GitHub.

This project strengthened my understanding of networking concepts covered in Cisco networking courses, CompTIA Network+, and the WGU Cybersecurity and Information Assurance program.

---

# 📁 Repository Contents

```text
Small-Business-DHCP-Network/
│
├── README.md
├── Small-Business-DHCP-Network.pkt
│
└── images/
    ├── 00-Project-Overview.png
    ├── 01-Small-Business-Topology.png
    ├── 02-Router-DHCP-Configuration.png
    ├── 03-PC-DHCP-Configuration.png
    ├── 04-Router-Verification-Commands.png
    ├── 05-Ping-Router-Success.png
    └── 06-PC-to-PC-Success.png
```

---

# 🚀 Future Improvements

The next version of this project will expand the network by implementing:

- VLAN Configuration
- Router-on-a-Stick
- Inter-VLAN Routing
- Multiple DHCP Scopes
- Access Control Lists (ACLs)
- Wireless Networking
- Basic Network Security

These enhancements will further strengthen my understanding of enterprise networking concepts while continuing to build my cybersecurity portfolio.

---

# 👩‍💻 Author

**Karen Batres**

Bachelor of Science in Cybersecurity and Information Assurance  
Western Governors University (WGU)

**GitHub:** https://github.com/KarenB1-tech

**LinkedIn:** *(Add your LinkedIn profile URL here.)*

---

⭐ **Thank you for taking the time to review this project. Feedback and suggestions are always welcome!**
