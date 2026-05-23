# Computer Networks Lab Portfolio (Cisco Packet Tracer)

Welcome to the **Networks** repository. This project contains a comprehensive suite of network simulation blueprints built using **Cisco Packet Tracer**. It documents practical implementations of key networking concepts, routing protocols, switching standards, and infrastructure services studied as part of Computer Engineering coursework.

The repository spans 8 progressive labs (`ayhamlab1.pkt` through `ayhamlab8.pkt`), moving from basic local area network setups to complex, multi-router topologies featuring dynamic routing, Access Control Lists (ACLs), and automated network services.

---

## 🛠️ Technology Stack & Tools
* **Simulation Environment:** Cisco Packet Tracer (v8.x recommended)
* **Core Protocols:** IPv4 Addressing, VLSM, Static Routing, RIPv2, OSPF, EIGRP, NAT/PAT, DHCP, DNS, HTTP, Telnet/SSH, VLANs, Inter-VLAN Routing (Router-on-a-Stick).
* **Hardware Simulated:** Cisco ISR 2911 Routers, Catalyst 2960 Switches, Generic Servers, and End-Devices (PCs, Laptops).

---

## 📂 Laboratory Breakdown

### 🔹 Lab 1: Foundational LAN Setup (`ayhamlab1.pkt`)
* **Objective:** Design a baseline Local Area Network (LAN) using a centralized switch to connect multiple host devices.
* **Key Implementations:**
  * Baseline host configurations (IPv4 Static Subnets, Subnet Masks).
  * Layer 2 switching discovery and verification of the MAC Address Table.
  * Local connectivity validation using `ping` and `traceroute`.

### 🔹 Lab 2 & 3: Advanced LAN Topology & Basic Routing (`ayhamlab2.pkt` / `ayhamlab3.pkt`)
* **Objective:** Scale host environments and introduce Layer 3 routing to interconnect distinct broadcast domains.
* **Key Implementations:**
  * Router interface configuring (FastEthernet/GigabitEthernet assigning).
  * Building a default gateway architecture for cross-subnet traffic communication.
  * Introductory Static Routing paths to tell the router how to reach remote networks.

### 🔹 Lab 4: Variable Length Subnet Masking (VLSM) Design (`ayhamlab4.pkt`)
* **Objective:** Optimize IP address allocation to eliminate wastage based on variable host requirements per department.
* **Key Implementations:**
  * Subnetting a core block (e.g., /24) into tailored subnets matching unique host capacities.
  * Configuration of networks with precise default gateways.
  * Validation of structural multi-subnet connectivity via a single routing point.

### 🔹 Lab 5: Dynamic Routing Implementation - RIPv2 & OSPF (`ayhamlab5.pkt`)
* **Objective:** Transition from administrative static paths to automated dynamic routing protocols across multi-router meshes.
* **Key Implementations:**
  * **RIPv2 Configuration:** Enabling classless dynamic updates with `version 2` and `no auto-summary`.
  * **OSPF Convergence:** Setting up Single-Area OSPF (Area 0), declaring explicit network wildcard masks, and evaluating shortest path first (SPF) metrics.
  * Analyzing and reading routing tables (`show ip route`) to verify optimal route selection.

### 🔹 Lab 6: Enterprise Infrastructure Services - DHCP, DNS, & Web HTTP (`ayhamlab6.pkt`)
* **Objective:** Centralize network operations by deploying automated application-layer infrastructure services.
* **Key Implementations:**
  * **DHCP Server Setup:** Constructing automated IP exclusion ranges and dynamic network distribution pools.
  * **DNS Mapping:** Creating visual Domain Name System records mapping customized web names to static target IPs.
  * **HTTP Web Server:** Deploying functional web server targets inside Packet Tracer and verifying end-user access using the built-in desktop Web Browser utility.

### 🔹 Lab 7: Virtual LANs (VLANs) & Inter-VLAN Routing (`ayhamlab7 (1).pkt`)
* **Objective:** Segment a single physical switch into logical independent broadcast domains to enhance network security and efficiency.
* **Key Implementations:**
  * Creating and labeling specific VLANs (e.g., Management, HR, Engineering) on Catalyst switches.
  * Configuring Access Ports for end-nodes and IEEE 802.1Q Trunk links for inter-switch connectivity.
  * **Router-on-a-Stick (RoaS):** Creating sub-interfaces on a single router link (`Router(config-subif)#`) paired with encapsulation tags to facilitate communication between isolated VLANs.

### 🔹 Lab 8: Network Security & Edge Services - ACLs & NAT/PAT (`ayhamlab8.pkt`)
* **Objective:** Harden the internal network perimeter and implement translation mechanisms required for public Internet traversal.
* **Key Implementations:**
  * **Access Control Lists (ACLs):** Developing Standard and Extended ACL traffic filters to restrict access to sensitive servers or block traffic from specific subnets.
  * **Network Address Translation (NAT/PAT):** Building Port Address Translation maps to convert private RFC 1918 addresses into routeable public IP interfaces.
  * Securing edge router access lines via VTY password controls and privilege levels.

---

## 🚀 How to Run the Labs

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/Ayhamtawara/Networks.git](https://github.com/Ayhamtawara/Networks.git)
   cd Networks
