# Lab Title: Packet Tracer Introduction

# Date: 26th Feb, 2026

# Topic: Network and Network Devices

# Objective:
Connect network devices together using Packet Tracer's "Automatically Choose Connection Type" function and understand basic device roles.

# Tools Used:
- Cisco Packet Tracer
- PC

# Network Topology:
A simple topology consisting of:
- 2 PCs
- 1 Switch
- 1 Router

(Insert topology screenshot below)
![Day 01 Topology](images/day01_topology.png)

# Configuration Steps:

1. Opened Cisco Packet Tracer.
2. Dragged and dropped:
   - 1 Router
   - 1 Switch
   - 2 PCs
3. Selected the "Automatically Choose Connection Type" (lightning icon).
4. Connected:
   - PC0 to Switch
   - PC1 to Switch
   - Switch to Router
5. Powered on all devices (if necessary).
6. Assigned IP addresses to PCs (if required for testing).

# Verification:

- Checked physical connections (green indicator lights).
- Used Command Prompt on PC:
  
  ping 192.168.1.X

- Confirmed successful communication between connected devices (if IPs were configured).

# Problems Faced:

- Initially connected wrong ports.
- Forgot that end devices must connect to switch ports (FastEthernet).
- Confused router interface naming (GigabitEthernet vs FastEthernet).

# What I Learned:

- The role of basic network devices:
  - Router connects different networks.
  - Switch connects devices within the same network.
  - PCs act as end devices.
- How to use the automatic connection tool.
- Basic physical topology setup.
- Importance of correct port selection.

# Real-World Application:

In real-world networks:
- Switches connect office computers.
- Routers connect the office network to the internet.
- Proper cabling and device placement are critical for communication.
- Network engineers must understand physical and logical topology before configuration.

# Security Insight (Extra - Thinking Like a Future Security Engineer):

- Physical access to network devices must be restricted.
- Unused switch ports should be disabled.
- Router interfaces should be secured with passwords.
- Default configurations should always be hardened.