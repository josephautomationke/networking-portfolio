# ISP Appointment Booking & Technician Assignment System

## Overview

The ISP Appointment Booking & Technician Assignment System is a workflow automation project designed to streamline the process of handling ISP service appointments.

The system uses n8n to process appointment and technician information, evaluate technician skills and availability, make a conditional assignment decision, update booking information, and send an automated Gmail notification.

This project demonstrates the practical use of workflow automation to reduce repetitive operational tasks in an ISP environment.

---

## Business Problem

ISP appointment management can require several manual steps.

A typical process may involve:

1. Receiving an appointment request.
2. Reviewing technician information.
3. Checking technician skills.
4. Checking availability.
5. Selecting a suitable technician.
6. Updating the appointment record.
7. Informing the relevant person about the booking.

Performing these tasks manually can become repetitive and time-consuming.

The goal of this project was to demonstrate how these steps can be connected into an automated workflow.

---

## Solution

The workflow uses n8n to connect the different stages of the appointment process.

The main workflow is:

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
