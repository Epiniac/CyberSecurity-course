# OSI Model (Open Systems Interconnection)

The **OSI model** is a conceptual framework used to understand and describe how data moves through a network. It divides network communication into **7 distinct layers**, each with a specific role. This separation helps engineers design, implement, and troubleshoot network systems more easily.

---

## Why the OSI Model Matters

* Standardizes network communication
* Helps isolate and diagnose network problems
* Makes learning networking more structured
* Allows interoperability between different vendors

---

## The 7 OSI Layers (Top to Bottom)

```
7. Application
6. Presentation
5. Session
4. Transport
3. Network
2. Data Link
1. Physical
```

A common mnemonic:
**"All People Seem To Need Data Processing"**

---

## 7. Application Layer

**Purpose:**
Provides network services directly to end-user applications.

**Examples:**

* HTTP / HTTPS (web)
* FTP (file transfer)
* SMTP (email)
* DNS (name resolution)

**Key Point:**
This is what the user interacts with.

---

## 6. Presentation Layer

**Purpose:**
Ensures data is in a readable format for the application layer.

**Responsibilities:**

* Data formatting
* Encryption / Decryption
* Compression

**Example:**

* SSL/TLS encryption

---

## 5. Session Layer

**Purpose:**
Manages sessions (connections) between two devices.

**Responsibilities:**

* Session establishment
* Session maintenance
* Session termination
* Synchronization (checkpoints)

**Example:**

* Maintaining a logged-in session

---

## 4. Transport Layer

**Purpose:**
Ensures reliable or fast data delivery between hosts.

**Responsibilities:**

* Segmentation & reassembly
* Error detection
* Flow control

**Protocols:**

* TCP (reliable, ordered)
* UDP (fast, connectionless)

---

## 3. Network Layer

**Purpose:**
Handles routing and logical addressing.

**Responsibilities:**

* Path selection
* Packet forwarding
* IP addressing

**Protocols & Devices:**

* IP
* ICMP
* Routers

---

## 2. Data Link Layer

**Purpose:**
Provides node-to-node data transfer and error detection.

**Responsibilities:**

* MAC addressing
* Framing
* Error detection

**Protocols & Devices:**

* Ethernet
* ARP
* Switches

---

## 1. Physical Layer

**Purpose:**
Transmits raw bits over a physical medium.

**Responsibilities:**

* Voltage levels
* Cables and connectors
* Data rates

**Examples:**

* Ethernet cables
* Fiber optics
* Wi-Fi signals

---

## OSI vs TCP/IP Model

| OSI Layer | TCP/IP Equivalent |
| --------- | ----------------- |
| 7–5       | Application       |
| 4         | Transport         |
| 3         | Internet          |
| 2–1       | Network Access    |

---

## Summary

* The OSI model has **7 layers**
* Each layer has a clear responsibility
* Used mainly for **learning and troubleshooting**
* Real-world networks often follow the **TCP/IP model**, but OSI remains a key reference

---