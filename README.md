# Networking & Automation Portfolio

## Joseph Automation

A practical portfolio showcasing networking infrastructure, ISP environments, troubleshooting, workflow automation and technology solutions.

---

## About

This repository contains practical projects demonstrating my development across networking and automation.

My focus is on building systems that solve practical operational problems rather than only demonstrating theoretical concepts.

The portfolio currently combines:

- Computer networking
- ISP network infrastructure
- Network troubleshooting
- Cisco Packet Tracer
- n8n workflow automation
- Google Sheets integration
- Gmail automation
- Conditional workflow logic
- Technician assignment processes

---

# Featured Projects

## 1. ISP Customer Network Deployment & Troubleshooting

A simulated ISP network environment developed using Cisco Packet Tracer.

### Technologies & Concepts

- Cisco Packet Tracer
- VLANs
- Inter-VLAN Routing
- OSPF
- DHCP
- NAT/PAT
- Network Troubleshooting
- Routing & Switching

### Project Demonstrates

- Network segmentation
- Router configuration
- Switch configuration
- VLAN implementation
- Inter-VLAN communication
- Dynamic routing
- DHCP configuration
- NAT configuration
- Troubleshooting network connectivity
- Diagnosing configuration problems

### Project

[View ISP Customer Network Project](projects/isp-customer-network/index.html)

[View ISP Network Documentation](projects/isp-customer-network/README.md)

---

# 2. ISP Appointment Booking & Technician Assignment System

An n8n workflow automation project designed to streamline ISP appointment processing and technician assignment.

The workflow connects appointment information with technician data and uses workflow logic to process the assignment.

### Workflow

```text
Google Sheets Trigger
        ↓
Collect Technician Data
        ↓
Match Skills & Availability
        ↓
IF Condition
        ↓
Update Booking
        ↓
Gmail Notification
