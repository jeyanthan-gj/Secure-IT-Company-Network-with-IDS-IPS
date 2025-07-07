# Secure IT Company Network Design (IDS & IPS)

A mini project report for **19EC651 – Computer Communication Networks Laboratory**

## Authors
- **Jeyanthan GJ** (Roll No. 22BEC170)
- **Selvaraj RS** (Roll No. 22BEC181)
- **III Year B.E ECE C (VI Semester)**

**Department of Electronics and Communication Engineering**  
**Academic Year 2025**  
**Mepco Schlenk Engineering College (Autonomous, Affiliated to Anna University, Chennai)**  
Sivakasi – 626 005, Virudhunagar (District), Tamil Nadu  
**February 2025**

---

## Table of Contents

1. [Introduction](#introduction)
2. [Case Study and Requirements](#case-study-and-requirements)
3. [Network Devices Description](#network-devices-description)
4. [Technologies Implemented](#technologies-implemented)
5. [Device Settings and Configuration](#device-settings-and-configuration)
6. [Implementation and Progress](#implementation-and-progress)
7. [Conclusion](#conclusion)

---

## Introduction

This project presents a secure, scalable, and robust company network design featuring Intrusion Detection (IDS) and Intrusion Prevention Systems (IPS). The design leverages enterprise-grade Cisco network devices, layered security, and best practices for access control and redundancy.

---

## Case Study and Requirements

- Secure web filtering and malware defense
- Strong access control and user authentication
- High availability and redundancy
- Segregation of network traffic (VLANs)
- Efficient IP management
- Centralized wireless and VoIP integration

---

## Network Devices Description

### Cisco Catalyst Switches (3850 & 2960)
- **3850:** Stackable, Layer 3 routing, integrated wireless controller, high bandwidth (up to 480 Gbps stacking).
- **2960:** Layer 2, suitable for access layer, supports VLANs, STP, port security, and energy efficiency.

### DHCP Server
- Assigns dynamic IP addresses and parameters (subnet mask, gateway) to clients.
- Reduces manual IP configuration, manages IP leases, DNS, and gateway info.

### DNS Server
- Resolves domain names to IP addresses, critical for network and internet operations.
- Caches lookups for faster response.

### FTP Server
- Facilitates file sharing between clients and servers.
- Features authentication, user access control, and optionally secure FTP (SFTP).

### Web Server
- Hosts and delivers web pages/applications over HTTP/HTTPS.
- Supports SSL/TLS encryption and load balancing.

### Email Server
- Manages sending/receiving emails using SMTP, IMAP, POP3.
- Implements spam filtering and virus scanning.

### VoIP Gateway
- Converts voice between PSTN and IP networks.
- Handles call routing, codec conversion, and supports fax/SMS integration.

### Wireless LAN Controller (WLC)
- Centralizes management of wireless access points.
- Provides wireless security, load balancing, and seamless roaming.

### NAS Storage Server
- Centralized file storage and sharing with data redundancy (RAID).
- Manages user access, permissions, and backups.

---

## Technologies Implemented

- **Design Tool:** Cisco Packet Tracer for simulation and configuration testing.
- **Hierarchical Network Model:** Core, Distribution, and Access layers for scalability and redundancy.
- **Wireless LAN Controller:** Centralized management of departmental WiFi.
- **VoIP:** Integration of IP phones for unified communications.
- **VLANs:** Departmental traffic segregation (Management, LAN, WLAN, VoIP, Blackhole).
- **EtherChannel (LACP):** Link aggregation for increased bandwidth and redundancy.
- **Spanning Tree Protocol (STP):** Prevents network loops, with PortFast and BPDUguard on access ports.
- **Subnetting:** Logical network divisions for efficient IP usage and security.
- **Device Security:** Hostname configuration, password encryption, banners, and secure logging.
- **Inter-VLAN Routing:** Multilayer switches enable communication between VLANs.
- **HSRP:** High availability routing using Hot Standby Router Protocol.
- **Static Addressing:** Critical devices assigned static IPs for reliability.
- **OSPF:** Dynamic routing protocol for efficient route advertisement and path selection.

---

## Device Settings and Configuration

- **Password Encryption:** Using `service password-encryption` for device security.
- **Banner Messages:** Legal and informational banners on login.
- **IP Addressing:** Static for core devices, DHCP for end users, with proper subnetting.
- **Routing:** OSPF for dynamic routing, static routes where required, inter-VLAN routing on multilayer switches.
- **Access Control Lists (ACLs):** Restrict/allow traffic as needed.
- **SSH:** Secure remote device management.
- **Port Security:** Restricts access to switch ports.

---

## Implementation and Progress

- **Simulation:** All network topologies and configurations tested in Cisco Packet Tracer.
- **Progress:** Step-by-step configuration of each component, validation of connectivity, redundancy, and security.

---

## Conclusion

The designed network delivers:
- High security using IDS & IPS measures.
- Redundancy and high availability for mission-critical services.
- Segregation and control of traffic using VLANs and ACLs.
- Efficient management and scalability using hierarchical architecture and automation tools.

---

## References

- Cisco Official Documentation
- [Cisco Packet Tracer Tutorials](https://www.netacad.com/courses/packet-tracer)
- Network Security Fundamentals, Anna University Syllabus

---

*For any queries, contact the project authors via the Department of Electronics and Communication Engineering, Mepco Schlenk Engineering College.*
