# 🌐 ISP Customer Network Deployment & Troubleshooting

## 🚀 Project Overview

This project simulates a real-world Internet Service Provider (ISP) deployment for a small business. It demonstrates full network setup, service configuration, and structured troubleshooting of connectivity issues from internal users to a simulated internet.

---

## 📌 Scenario

A business network experienced multiple issues:

* Devices were not receiving IP addresses
* Departments could not communicate
* Internet access was unavailable

As the network engineer, I:

* Designed and deployed the network
* Configured routing and services
* Diagnosed and resolved all failures

---

## 🧱 Network Architecture

### 🔹 Internal Network

* VLAN 10 — HR
* VLAN 20 — Sales
* Layer 2 Switch (access + trunk)

### 🔹 Routing Layer

* Router-on-a-Stick (Inter-VLAN routing)
* Subinterfaces for VLAN segmentation

### 🔹 ISP Simulation

* EDGE Router (customer gateway)
* CORE Router (ISP backbone)
* INTERNET Router (external simulation)

---

## ⚙️ Technologies Used

* VLAN Segmentation
* Inter-VLAN Routing
* DHCP
* OSPF
* NAT (PAT)
* Static Routing
* Network Troubleshooting

---

## 🔧 Key Configurations

### VLANs

* Created VLAN 10 and VLAN 20
* Assigned switch ports
* Configured trunk link

### Routing

* Configured subinterfaces for inter-VLAN routing

### DHCP

* Configured pools for automatic IP assignment

### OSPF

* Established neighbor adjacency between routers

### NAT

* Configured PAT for internet access

---

## 📸 Network Implementation & Results

### 🔹 VLAN Configuration

![VLAN](screenshots/Vlan%20configurationf.png)

---

### 🔹 DHCP Configuration

![DHCP Config](screenshots/Configure%20DHCP%20.png)

---

### 🔹 DHCP Working

![DHCP Working](screenshots/dhcp%20working.png)

---

### 🔹 Inter-VLAN Routing

![Inter-VLAN](screenshots/inter%20vlan%20routing%20router.png)

---

### 🔹 OSPF Configuration

![OSPF](screenshots/ospf%20in%20router.png)

---

### 🔹 Routing Verification

![Routing](screenshots/routing%20confirmed.png)

---

### 🔹 NAT Configuration

![NAT](screenshots/NAT%20configuration.png)

---

### 🔹 NAT Fixed

![NAT Fixed](screenshots/fixed%20nat.png)

---

## 🛠 Troubleshooting Evidence

### 🔴 DHCP Failure (169.x.x.x)

![DHCP Error](screenshots/dhcp%20not%20worrking%20fix.png)

**Cause:** DHCP not reachable
**Fix:** Corrected trunk and routing configuration

---

### 🔴 ACL / Connectivity Issue

![ACL](screenshots/ACL%20troubleshoot.png)

**Cause:** Traffic blocked / misconfiguration
**Fix:** Adjusted rules and verified routing

---

## ✅ Final Results

* All devices received IP addresses
* VLAN segmentation worked correctly
* Inter-VLAN communication successful
* OSPF routing stable
* Internet simulation achieved
* Network fully operational

---

## 🧠 What I Learned

* How to design and segment enterprise networks
* How to configure routing and NAT for real-world scenarios
* How to troubleshoot using a step-by-step method
* How to identify issues using CLI tools (`show`, `ping`, `traceroute`)
* How to resolve Layer 1–Layer 3 network failures

---

## 🎯 Key Skills Demonstrated

* Network Design
* Routing (Static + OSPF)
* NAT (PAT)
* DHCP Deployment
* VLAN Configuration
* Troubleshooting Methodology

---


```

---

## 📬 Contact

* Email: josephnjuguna.automation@gmail.com


---
