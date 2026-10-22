# Layer 3 Switch with Router – Point-to-Point Connection

## 📌 Project Overview

This project demonstrates a **point-to-point connection between a Layer 3 Switch and a Router** using **Cisco Packet Tracer**.

The main purpose of this lab is to understand how a Layer 3 switch can perform routing functions and communicate with a router through a point-to-point network connection.

## 🎯 Objectives

- Understand Layer 3 Switch configuration
- Configure a point-to-point connection between a Layer 3 Switch and Router
- Configure IP addresses on Layer 3 interfaces
- Enable routing on the Layer 3 Switch
- Configure routing between network devices
- Verify connectivity using `ping`
- Understand the difference between Layer 2 and Layer 3 switching

## 🖥️ Network Topology

**Layer 3 Switch ↔ Router**

The Layer 3 switch is connected directly to the router using a point-to-point connection.

```text
+------------------+          Point-to-Point          +------------------+
|                  |                                  |                  |
|   Layer 3 Switch |==================================|      Router      |
|                  |                                  |                  |
+------------------+                                  +------------------+
```

## ⚙️ Technologies Used

- Cisco Packet Tracer
- Layer 3 Switch
- Cisco Router
- IPv4 Addressing
- Static Routing / Layer 3 Routing
- Point-to-Point Networking
- ICMP / Ping

## 🔧 Key Configuration Concepts

### Layer 3 Switch

The Layer 3 switch is configured to operate at the network layer and provide routing functionality.

Example:

```bash
enable
configure terminal

ip routing
```

An IP address can then be configured on the Layer 3 interface:

```bash
interface <interface-id>
ip address <IP-address> <subnet-mask>
no shutdown
```

### Router

The router interface connected to the Layer 3 switch is configured with an IP address from the same point-to-point network.

```bash
enable
configure terminal

interface <interface-id>
ip address <IP-address> <subnet-mask>
no shutdown
```

## 🔍 Verification Commands

The following commands can be used to verify the configuration:

```bash
show ip interface brief
```

```bash
show ip route
```

```bash
ping <destination-ip>
```

These commands help verify interface status, routing information, and end-to-end connectivity.

## 📚 Key Learnings

- A **Layer 3 switch** can perform routing using `ip routing`.
- A router and Layer 3 switch can communicate through a point-to-point Layer 3 connection.
- Both sides of the connection need appropriate IP addresses.
- Interfaces must be enabled using `no shutdown`.
- Routing tables determine how packets reach their destination.
- `ping` can be used to test connectivity between devices.

## 🧪 Lab Practice

This Packet Tracer file was created as part of my **CCNA networking hands-on practice**.

The lab focuses on understanding:

**Layer 3 Switching → IP Addressing → Routing → Router Connectivity → Network Verification**

## 📁 File

- `layer 3 switch with router point-to-point connection.pkt` — Cisco Packet Tracer project file

## 🚀 Skills Practiced

- Cisco IOS CLI
- IPv4 Addressing
- Layer 3 Switching
- Routing
- Router Configuration
- Network Troubleshooting
- Connectivity Testing
- Cisco Packet Tracer

## 👨‍💻 Learning Journey

This project is part of my **CCNA Journey** and hands-on networking practice.

> Learning networking one lab at a time. 🌐
