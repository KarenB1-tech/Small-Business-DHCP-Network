# 🌐 Network Topology

<p align="center">
  <img src="01-Small-Business-Topology.jpg" width="900">
</p>

This topology demonstrates a centralized LAN where every client connects to a Cisco switch, which connects to the Cisco router acting as both the default gateway and DHCP server.

---

# 🖥️ Devices Used

| Device | Quantity |
|---------|---------:|
| Cisco 1941 Router | 1 |
| Cisco 2960-24TT Switch | 1 |
| Cloud-PT (Internet) | 1 |
| Desktop PCs | 12 |

---

# 🌍 Network Configuration

| Setting | Value |
|---------|-------|
| Network Address | 192.168.10.0/24 |
| Router IP | 192.168.10.1 |
| Default Gateway | 192.168.10.1 |
| DHCP Pool | 192.168.10.10 - 192.168.10.254 |
| DNS Server | 8.8.8.8 |

---

# ⚙️ Router Configuration

The Cisco router was configured to:

- Configure the hostname.
- Configure the LAN interface.
- Assign the gateway IP address.
- Configure DHCP excluded addresses.
- Create the DHCP pool.
- Configure the default gateway.
- Configure the DNS server.
- Save the running configuration.

<p align="center">
  <img src="02-Router-DHCP-Configuration.jpg" width="900">
</p>

---

# 💻 DHCP Client Configuration

Every workstation was configured to automatically obtain its network settings.

Each client successfully received:

- IPv4 Address
- Subnet Mask
- Default Gateway
- DNS Server

<p align="center">
  <img src="03-PC-DHCP-Configuration.jpg" width="850">
</p>

---

# ✅ Network Verification

The following Cisco IOS commands were used to verify the network:

```text
show ip interface brief
show ip dhcp pool
show ip dhcp binding
```

These commands verified:

- Interface status
- DHCP pool configuration
- DHCP leases
- Router operational status

<p align="center">
  <img src="04-Router-Verification-Commands.jpg" width="900">
</p>

---

# 📡 Connectivity Testing

## Ping Test to Router

The client computer successfully communicated with the default gateway.

<p align="center">
  <img src="05-Ping-Router-Success.jpg" width="850">
</p>

---

## PC-to-PC Communication

Successful communication between client devices confirmed proper DHCP operation and Layer 3 connectivity.

<p align="center">
  <img src="06-PC-to-PC-Success.jpg" width="850">
</p>

---

# 🧠 Skills Demonstrated

This project strengthened my experience with:

- Cisco Packet Tracer
- Cisco IOS CLI
- Router Configuration
- DHCP Configuration
- IPv4 Addressing
- LAN Design
- Switch Configuration
- Network Verification
- Connectivity Testing
- Basic Network Troubleshooting
- Technical Documentation
- GitHub Portfolio Development

---

# 📚 What I Learned

Completing this project improved my understanding of how a real small business network operates.

Key concepts I practiced include:

- Designing a LAN topology.
- Configuring Cisco routers using the IOS CLI.
- Configuring DHCP services.
- Understanding how DHCP automatically assigns IP addresses.
- Configuring clients to obtain IP addresses dynamically.
- Verifying DHCP leases and interface status.
- Testing connectivity using the `ping` command.
- Understanding IPv4 addressing and default gateways.
- Practicing network troubleshooting.
- Creating professional technical documentation for GitHub.

This project strengthened concepts covered in Cisco Networking, CompTIA Network+, and the WGU Cybersecurity program.

---

# 📁 Repository Contents

```text
Small-Business-DHCP-Network
│
├── README.md
├── Small-Business-DHCP-Network.pkt
├── 00-Project-Overview.png
├── 01-Small-Business-Topology.jpg
├── 02-Router-DHCP-Configuration.jpg
├── 03-PC-DHCP-Configuration.jpg
├── 04-Router-Verification-Commands.jpg
├── 05-Ping-Router-Success.jpg
└── 06-PC-to-PC-Success.jpg
```

---

# 🚀 Future Improvements

Future versions of this network will include:

- VLANs
- Router-on-a-Stick
- Inter-VLAN Routing
- Multiple DHCP Scopes
- Access Control Lists (ACLs)
- Wireless Networking
- Basic Network Security

These enhancements will continue expanding my networking and cybersecurity skills through hands-on projects.

---

# 👩‍💻 Author

## Karen Batres

Bachelor of Science in Cybersecurity and Information Assurance  
**Western Governors University (WGU)**

🔗 **GitHub**  
https://github.com/KarenB1-tech

🔗 **LinkedIn**  
https://www.linkedin.com/in/karen-batres-umana-a31245358/

---

## ⭐ Thank You

Thank you for taking the time to review my project.

I am continuously building hands-on networking and cybersecurity projects while expanding my technical skills through Cisco Packet Tracer, WGU, CompTIA certifications, and practical lab environments.

Feedback and suggestions are always appreciated!
