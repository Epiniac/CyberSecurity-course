# CompTIA Network+ – Networking Devices

## 1. Router

### What it is

A **router** is a networking device designed to **connect multiple distinct networks** and intelligently forward data between them. Its primary responsibility is to determine the **best possible path** for data to travel from a source network to a destination network using **IP addressing and routing logic**.

Unlike devices that operate only within a single network, a router sits at the **boundary between networks** (for example, between a private LAN and the public Internet). Every device that wants to communicate outside its local network sends traffic to the router, which is why the router is known as the **default gateway**.

At its core, a router analyzes the **destination IP address** of each packet, consults its **routing table**, and forwards the packet to the appropriate next hop. By doing this, routers control traffic flow, prevent unnecessary broadcasts from spreading, and enable global connectivity.

### Key characteristics

* Uses **IP addresses** to make forwarding decisions
* Separates **broadcast domains**
* Acts as the **default gateway** for devices
* Connects **LAN to WAN** (ex: home network to the Internet)

### Common router features

* Routing (static or dynamic)
* NAT / PAT
* DHCP service (optional)
* Basic firewall functionality

### Exam keywords

**IP address, default gateway, routing, Layer 3**

---

## 2. Switch

### What it is

A **switch** is a networking device that connects multiple devices **within the same local network** and enables them to communicate efficiently. Its main function is to forward data only to the **intended destination device**, rather than broadcasting it to all devices.

A switch operates by learning the **MAC addresses** of connected devices and building a **MAC address table**. When a frame arrives, the switch checks this table and forwards the frame only to the correct port. This dramatically reduces unnecessary traffic and collisions compared to older technologies like hubs.

Switches form the backbone of modern LANs and are essential for performance, scalability, and network segmentation.

### Key characteristics

* Uses **MAC addresses**
* One collision domain per port
* Full-duplex communication
* Forwards **frames**, not packets

### Advanced switch features

* VLANs
* Trunking
* Port security
* Some switches can operate at Layer 3 (Layer 3 switches)

### Exam keywords

**MAC address, frames, VLAN, Layer 2**

---

## 3. Firewall

### What it is

A **firewall** is a security device or software solution that acts as a **control point between trusted and untrusted networks**. Its purpose is to inspect network traffic and decide whether to **allow or block** that traffic based on predefined security rules.

Firewalls analyze traffic using information such as IP addresses, port numbers, protocols, and connection state. By enforcing these rules, a firewall protects internal systems from unauthorized access, malware, and external attacks while still allowing legitimate communication.

Firewalls are commonly deployed at network perimeters, between internal network segments, or directly on individual hosts.

### Types of firewalls

* **Stateless** – checks individual packets
* **Stateful** – tracks active connections (most common)
* **Next-Generation Firewall (NGFW)** – includes deep packet inspection, application awareness

### Purpose

* Allow or block traffic
* Protect internal networks from unauthorized access

### Exam keywords

**Allow/deny rules, stateful inspection, security**

---

## 4. IDS and IPS

### What it is

**IDS (Intrusion Detection System)** and **IPS (Intrusion Prevention System)** are security technologies designed to **monitor network traffic for malicious activity, policy violations, or suspicious behavior**.

Both systems analyze traffic patterns, signatures, and anomalies to identify potential threats such as attacks, exploits, or unauthorized access attempts. The key difference lies in how they respond once a threat is detected.

An IDS focuses on **visibility and alerting**, while an IPS actively takes action to **stop threats in real time**.

### IDS – Intrusion Detection System

* Monitors traffic
* **Detects and alerts** on suspicious activity
* Does NOT block traffic

### IPS – Intrusion Prevention System

* Monitors traffic
* **Detects and blocks** malicious activity
* Placed inline with traffic flow

### Memory trick

* **IDS = Detect**
* **IPS = Prevent**

### Exam keywords

**Alert vs block, intrusion detection/prevention**

---

## 5. Load Balancing (Concept)

### What it means

**Load balancing** is the practice of distributing network or application traffic across multiple resources to improve:

* Performance
* Availability
* Fault tolerance

### Why it matters

* Prevents server overload
* Ensures high availability

---

## 6. Load Balancer

### What it is

A **load balancer** is a device or software solution that sits in front of multiple servers and **distributes incoming client requests across them**. Its goal is to ensure that no single server becomes overwhelmed while others sit idle.

By intelligently spreading traffic, load balancers improve **performance, reliability, and availability** of applications and services. If one server fails, the load balancer can automatically redirect traffic to healthy servers, enabling high availability.

Load balancers are commonly used in web services, cloud environments, and enterprise data centers.

### Load balancing methods

* Round robin
* Least connections
* Weighted distribution

### OSI layers

* Layer 4 (TCP/UDP)
* Layer 7 (Application-aware load balancing)

### Exam keywords

**Traffic distribution, high availability**

---

## 7. Proxy Server

### What it is

A **proxy server** is an intermediary system that **handles client requests on their behalf**. Instead of clients communicating directly with a destination server, they send their requests to the proxy, which then forwards them.

Proxies are commonly used to improve security, control access to resources, enhance performance through caching, and provide anonymity by hiding internal client IP addresses from external servers.

Depending on placement and configuration, proxies can protect clients, servers, or both.

### Functions

* Content filtering
* Caching
* Hiding internal IP addresses
* Access control

### Types

* Forward proxy
* Reverse proxy
* Transparent proxy

### Exam keywords

**Acts on behalf of client, caching, anonymity**

---

## 8. NAS vs SAN

### NAS – Network Attached Storage

* File-level storage
* Uses standard network protocols (SMB, NFS)
* Easy to deploy
* Lower cost

### SAN – Storage Area Network

* Block-level storage
* High performance
* Uses Fibre Channel or iSCSI
* More complex and expensive

### Comparison table

| Feature      | NAS        | SAN         |
| ------------ | ---------- | ----------- |
| Storage type | File-level | Block-level |
| Performance  | Moderate   | Very high   |
| Complexity   | Low        | High        |
| Cost         | Lower      | Higher      |

---

## 9. Access Point (AP)

### What it is

An **Access Point (AP)** is a networking device that allows **wireless devices** such as laptops, smartphones, and tablets to connect to a **wired Ethernet network**.

An AP acts as a **bridge between wireless and wired networks**, converting radio signals into wired Ethernet frames and vice versa. It extends network access without requiring physical cables for each device, enabling mobility and flexibility.

Access Points are commonly deployed in homes, offices, campuses, and public spaces, often in groups to provide seamless wireless coverage.

### Key points

* Operates at **Layer 2**
* Does NOT assign IP addresses by default
* Bridges wireless and wired networks

### Exam keywords

**Wireless to wired bridge, Layer 2**

---

## 10. Wireless Networking

### What it is

**Wireless networking** is a method of connecting devices to a network using **radio frequency (RF) signals** instead of physical cables. It enables mobility, flexibility, and ease of deployment while maintaining network connectivity.

Wireless networks rely on **access points** and standardized communication protocols defined by IEEE 802.11. Devices authenticate, associate with an AP, and then transmit data over shared radio channels.

Because wireless signals travel through the air, security and interference management are critical considerations in wireless network design.

### Wireless security

* WPA2
* WPA3 (preferred)

### Exam keywords

**SSID, encryption, wireless standards**

---
