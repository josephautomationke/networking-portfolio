# 🌐 ISP Customer Network Deployment & Troubleshooting

## 🚀 Project Overview

This project simulates a real-world Internet Service Provider (ISP) deployment for a small business customer. It demonstrates end-to-end network setup, service configuration, and structured troubleshooting of multiple network failures.

The goal was to design a functional network, deliver connectivity, and resolve issues affecting internal communication and internet access.

---

## 📌 Scenario

A business customer reported multiple network issues:

* Some devices were not receiving IP addresses
* Departments could not communicate
* Internet access was unavailable

As the network engineer, I was responsible for:

* Building the network infrastructure
* Configuring core services
* Diagnosing and resolving connectivity issues

---

## 🧱 Network Architecture

### 🔹 Internal Network

* VLAN 10 — HR Department
* VLAN 20 — Sales Department
* Layer 2 Switch (access + trunk ports)

### 🔹 Routing Layer

* Router-on-a-Stick for Inter-VLAN routing
* Subinterfaces for VLAN segmentation

### 🔹 ISP Simulation

* EDGE Router (customer-facing)
* CORE Router (ISP backbone)
* INTERNET Router (external network simulation)

---

## ⚙️ Technologies Implemented

* VLAN segmentation
* Inter-VLAN Routing
* DHCP (Dynamic Host Configuration Protocol)
* OSPF (Open Shortest Path First)
* NAT (PAT - Port Address Translation)
* Static Routing
* Basic Network Troubleshooting

---

## 🔧 Key Configuration Highlights

### VLAN Configuration

* Created VLAN 10 (HR) and VLAN 20 (Sales)
* Assigned switch ports to appropriate VLANs
* Configured trunk link to router

---

### Inter-VLAN Routing

* Implemented Router-on-a-Stick using subinterfaces
* Enabled communication between VLANs

---

### DHCP Configuration

* Configured DHCP pools per VLAN
* Automatically assigned IP addresses, gateway, and DNS

---

### OSPF Routing

* Established adjacency between EDGE and CORE routers
* Enabled dynamic route exchange

---

### NAT (Internet Access)

* Configured PAT on EDGE router
* Translated private IP addresses to public IP for internet access

---

## 🛠 Troubleshooting Process

A structured troubleshooting approach was used to identify and resolve multiple issues:

---

### 🔴 Issue 1 — Devices Receiving 169.x.x.x Addresses

**Cause:** DHCP requests not reaching the router
**Diagnosis:** Verified VLANs and trunk configuration
**Resolution:** Corrected trunk link between switch and router

---

### 🔴 Issue 2 — “Destination Host Unreachable”

**Cause:** Missing routing path to external network
**Diagnosis:** Checked routing table using `show ip route`
**Resolution:** Configured default route toward CORE router

---

### 🔴 Issue 3 — No Internet Connectivity

**Cause:** CORE router lacked upstream path
**Diagnosis:** Traced packet flow hop-by-hop
**Resolution:** Added INTERNET router and configured routing

---

### 🔴 Issue 4 — Network Still Not Responding

**Cause:** Interface administratively down
**Diagnosis:** Used `show ip interface brief`
**Resolution:** Enabled interface using `no shutdown`

---

## ✅ Final Results

* All devices successfully received IP addresses via DHCP
* VLAN segmentation worked as expected
* Inter-VLAN communication was fully functional
* Internet simulation was successfully achieved
* Network remained stable after fault resolution

---

## 📸 Project Evidence

The following screenshots are included in this project:

* Network topology
* DHCP address assignment
* OSPF neighbor relationship
* Successful connectivity tests (ping)
* Troubleshooting steps and error outputs

---

## 🧠 Key Skills Demonstrated

* Network design and segmentation
* Routing (Static + OSPF fundamentals)
* NAT configuration (PAT)
* DHCP deployment and verification
* Systematic troubleshooting methodology
* Real-world problem analysis and resolution

---

## 🎯 Key Takeaway

This project goes beyond configuration by focusing on **real-world troubleshooting scenarios**, simulating the type of issues commonly handled in ISP and network support roles.

---

## 📬 Contact

* Email: [your-email@example.com](mailto:your-email@example.com)
* GitHub: your-profile-link

---
