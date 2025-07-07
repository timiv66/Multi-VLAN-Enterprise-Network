# Multi-VLAN-Enterprise-Network

## Project Overview
In this project I have set up a small network with 3 separate Virtual Local Area Networks (VLANs) in a corporate environment. Each VLAN will be given its own pool of IP addresses from an router with DHCP enabled.

## Network Topology

- **1 Router**
- **1 Layer 3 Switch**
- **1 Layer 2 Switch**
- **1 DNS Server**
- **12 Personal Computers** (4 for each VLAN)
- **Copper straight through and trunk cables**

## Learning Objectives
- ✅ Configure and segment a network using **VLANs**
- ✅ Enable **inter-VLAN routing** on a Layer 3 switch
- ✅ Use a **DHCP server** to assign IPs dynamically per VLAN
- ✅ Implement a **DNS server** for domain name resolution
- ✅ Apply **ACLs (Access Control Lists)** to restrict network access between VLANs

## IP Addressing Scheme
For my IP selection, I used addresses from the private Class C range (192.168.0.0/16), which is commonly reserved for internal addressing in small office and home networks. I chose a subnet mask of /24 (255.255.255.0), which provides 256 total IP addresses per subnet, including 254 usable host addresses. This allows each VLAN to support a large number of devices, with sufficient room to scale and accommodate future infrastructure.<br>
<br>

| Department | VLAN ID | Subnet            | Default Gateway  | DHCP IP Range         |
|------------|---------|-------------------|------------------|------------------------|
| HR         | 10      | 192.168.10.0/24   | 192.168.10.1     | 192.168.10.100–192.168.10.200 |
| IT         | 20      | 192.168.20.0/24   | 192.168.20.1     | 192.168.20.100–192.168.20.200 |
| Sales      | 30      | 192.168.30.0/24   | 192.168.30.1     | 192.168.30.100–192.168.30.200 |


This project is part of my journey to become a network engineer. It replicates real-world enterprise networking principles using Cisco Packet Tracer. Feedback and collaboration welcome!
