# Multisite Networks Configuration Lab

**Date:** 17/05/2025  
**Toolchain:** Cisco Packet Tracer  
**Status:** ✅ Completed and Verified  
**Documentation:** 📎 Full configuration steps and interface details included

---

## 📘 Overview

This project demonstrates the full configuration and validation of a **multisite enterprise network** using **Cisco Packet Tracer**. The lab simulates real-world scenarios including:

- Subnetting for scalable design
- Static and dynamic routing (RIPv2)
- Deployment of network services (DNS, HTTP, FTP, DHCP)
- End-to-end connectivity validation and service testing

All configurations were performed strictly through CLI and desktop interfaces—no reliance on Packet Tracer’s GUI config tab.

---

## 🧭 Network Architecture

The network is composed of the following core segments:

- **ISP Network**: `209.165.200.224/27`
- **Headquarter Network**: Subnetted from `192.168.2.0/24`
- **Branch Network**: Subnetted from `192.168.2.0/24`
- **WAN Links**: `209.165.201.0/30` and `192.168.2.128/26`

The network is designed to scale while supporting services across distributed LANs.

---

## 🔧 Key Features

### 📌 Subnetting & IP Planning
- 4 subnets derived from `192.168.2.0/24` using `/26` mask
- Minimum 60 usable hosts per subnet
- Clear allocation for LANs and WAN links

### 🛠 Static Routing
- Manual configuration across all routers
- Interface-level addressing with full command documentation
- Static routes for all inter-site paths

### 🔁 Dynamic Routing (RIPv2)
- RIP enabled across ISP, HQ, and Branch routers
- No auto-summary to preserve classless routes
- Fully functional route propagation and convergence

### 🌐 Services Configured
- **HTTP (Web)**: Internal and external sites hosted
- **DNS**: Internal resolution for `www.mycompany.fr`, `ftpmyfiles.fr`
- **FTP**: Upload/download verified with user authentication
- **DHCP**: Dynamic address allocation with gateway and DNS

---

## 📂 Repository Contents

| File/Folder                  | Description                                           |
|-----------------------------|-------------------------------------------------------|
| `README.md`                 | Project overview and usage instructions               |
| `PacketTracer_Config.pkt`   | Final Packet Tracer file (not included here)          |
| `config/`                   | CLI commands and screenshots for all configurations   |
| `docs/`                     | Lab report and supporting documentation               |
| `screenshots/`              | Visual verification for each stage                    |

---

## 🚦 Simulation & Verification

### ✅ Ping Tests
- Verified from both ends of LANs and WANs
- Confirmed reachability to external ISP services

### ✅ DNS & HTTP
- Successfully resolved domain names
- Reached internal/external web servers

### ✅ FTP Transfers
- Uploads and downloads verified
- Captured and analyzed TCP ports (20/21)

### ✅ DHCP
- Auto-assignment of IPs with correct DNS/gateway
- Verified via release/renew cycles

---

## 🧪 Lab Execution Policy

- No GUI-based configuration: Only CLI and Desktop tabs used
- Every device configured manually, replicating real-world constraints
- All configurations verified through live simulation and test commands

---

## 🧠 Learning Objectives Achieved

✔ Efficient subnet planning and allocation  
✔ End-to-end static and dynamic routing  
✔ Service-layer configuration and testing  
✔ Hands-on experience with Cisco CLI  
✔ Network troubleshooting and simulation analysis

---

## 📌 How to Reuse

1. Clone this repo.
2. Open the `.pkt` file in Cisco Packet Tracer.
3. Follow the instructions in the `config/` folder to reconfigure the network.
4. Use simulation mode to inspect traffic flows and service interactions.

---

## 🤝 Contribution

This project is closed for contributions as it represents a finalized lab submission. However, forks are welcome for educational use or derivative work.

---

## 📜 License

All content is © Rayan EL IDRISSI DAFALI.  
For academic or educational reuse only. Commercial usage is prohibited.

---

## 🏁 Final Notes

This project encapsulates critical foundational skills in enterprise network design and Cisco configuration. It serves as a complete reference for:

- Manual IP address planning
- Hybrid routing strategies
- Service integration (HTTP, DNS, FTP, DHCP)
- Network validation via simulation

Feel free to explore the configuration scripts and adapt the design for more complex topologies.
