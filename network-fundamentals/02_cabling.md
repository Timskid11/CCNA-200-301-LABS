

# Lab Title: Cabling in Cisco Packet Tracer

# Date: 27th Feb, 2026

# Topic: Network Cabling & Connection Types

# Objective:

Understand different cable types and manually connect devices using the correct cable in Cisco Packet Tracer.

# Tools Used:

* Cisco Packet Tracer
* PC

---

# Cable Types in Packet Tracer

## 1️⃣ Copper Straight-Through Cable

### Used For:

* PC → Switch
* Switch → Router
* PC → Router (sometimes)

### Why?

Used to connect **different types of devices**.

---

## 2️⃣ Copper Cross-Over Cable

### Used For:

* PC → PC
* Switch → Switch
* Router → Router

### Why?

Used to connect **same type of devices** (though modern devices support Auto-MDIX).

---

## 3️⃣ Fiber Optic Cable

### Used For:

* Switch → Switch (long distance)
* High-speed backbone connections

### Why?

* Faster
* Longer distance
* Immune to electromagnetic interference

---

# Network Topology (Day 2)

Devices:

* 2 PCs
* 1 Switch
* 1 Router

---

# Configuration Steps (Manual Cabling)

1. Opened Cisco Packet Tracer.
2. Dragged:

   * 1 Router
   * 1 Switch
   * 2 PCs
3. Selected **Copper Straight-Through** manually (instead of automatic).
4. Connected:

   * PC0 → Switch (FastEthernet0 to FastEthernet0/1)
   * PC1 → Switch (FastEthernet0 to FastEthernet0/2)
   * Switch → Router (GigabitEthernet or FastEthernet ports)
5. Waited for link lights to turn green.

---

# Verification

* Checked physical connection indicators (green lights).
* Verified correct port types.
* Used:

```
ping 192.168.1.X
```

(after assigning IP addresses if required)

---

# Problems Faced

* Used crossover cable instead of straight-through initially.
* Connected to wrong router interface.
* Forgot that router interfaces must be enabled (`no shutdown`).

---

# What I Learned

* Straight-through = different device types
* Crossover = same device types
* Fiber = long distance/high speed
* Correct port selection matters
* Cabling mistakes cause Layer 1 issues

---

# Real-World Application

* Offices use straight-through cables to connect PCs to switches.
* Data centers use fiber for backbone connections.
* Network engineers must understand Layer 1 before IP configuration.

---

# Security Insight (Thinking Like a Security Engineer 🔐)

* Unused switch ports should be disabled.
* Patch panels should be secured physically.
* Fiber tapping is harder but still possible.

