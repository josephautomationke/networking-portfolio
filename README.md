# 🌐 Networking & Automation Portfolio

## Joseph Automation

> **Building practical technology solutions across networking, ISP infrastructure, and business process automation.**

This repository is a showcase of practical projects combining **computer networking, ISP infrastructure, troubleshooting, workflow automation, and operational technology solutions**.

Rather than focusing only on individual technologies, these projects demonstrate how technology can be applied to solve real operational problems.

---

## 🚀 What This Portfolio Demonstrates

This portfolio currently covers two different technical areas:

| Project | Focus | Main Technologies |
|---|---|---|
| 🌐 **ISP Customer Network Deployment & Troubleshooting** | Network infrastructure | Cisco Packet Tracer, VLANs, OSPF, DHCP, NAT/PAT |
| 🤖 **ISP Appointment Booking & Technician Assignment Automation** | Business process automation | n8n, Google Sheets, Gmail, conditional logic |

### The difference is simple:

**Project 01 = I build and troubleshoot the network.**

**Project 02 = I automate the business processes that operate around the network.**

Together, they demonstrate a broader understanding of how an ISP can use technology for both **infrastructure and operational efficiency**.

---

# 🌐 Project 01 — ISP Customer Network Deployment & Troubleshooting

### Network Infrastructure & Troubleshooting

This project simulates the deployment and troubleshooting of a structured ISP/customer network environment using Cisco Packet Tracer.

The objective was to design a working network infrastructure and demonstrate the ability to configure, test, diagnose, and resolve common networking problems.

### 🔧 Key Areas

- VLAN configuration
- Inter-VLAN routing
- OSPF routing
- DHCP
- NAT/PAT
- Router configuration
- Switch configuration
- Network segmentation
- Connectivity testing
- Troubleshooting
- Fault identification and resolution

### 🎯 What This Project Demonstrates

The project demonstrates practical understanding of:

- Network design
- Routing and switching
- IP addressing
- Network segmentation
- Dynamic routing
- DHCP services
- NAT configuration
- Connectivity troubleshooting
- Diagnosing configuration problems

### 📂 Project Files

[**→ Open the Full Networking Project**](projects/isp-customer-network/index.html)

[**→ Read the Networking Documentation**](projects/isp-customer-network/README.md)

---

# 🤖 Project 02 — ISP Appointment Booking & Technician Assignment Automation

### Business Process Automation

This project focuses on a completely different problem.

Instead of building the network itself, the goal is to **automate an ISP operational process**.

The system processes appointment information, evaluates technician information, applies assignment logic, updates booking information, and sends automated communication.

The workflow is built using **n8n**, with Google Sheets and Gmail used as supporting services.

---

## ⚙️ Automation Workflow

```text
                    CUSTOMER / BOOKING DATA
                              │
                              ▼
                    ┌─────────────────────┐
                    │   Google Sheets     │
                    │      Trigger        │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Technician Data     │
                    │ Collection          │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Skills & Availability│
                    │ Matching             │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    IF / Decision    │
                    │       Logic         │
                    └──────────┬──────────┘
                               │
                       ┌───────┴───────┐
                       ▼               ▼
                  MATCH FOUND      NO MATCH
                       │               │
                       ▼               ▼
                Update Booking    Handle Result
                       │
                       ▼
                Gmail Notification
