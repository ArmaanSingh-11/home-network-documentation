# Home Network Documentation  
**Author:** Armaanjot Singh  
**Location:** Winnipeg, Manitoba  
**Date:** March 2026  

---

# 1. Physical Network Topology

The home network is deployed in a two-room apartment consisting of a living room and bedroom. The main networking devices are located in the living room, where the internet connection enters the apartment.

## Living Room Layout

| Device | Interface | Cable Type | Connected To | Location |
|-------|-----------|-----------|--------------|----------|
| ISP Fiber Modem | WAN Port | Fiber line | ISP Network | Living Room wall panel |
| Wireless Router | WAN Port | Cat6 Ethernet | ISP Modem | TV stand |
| Desktop PC | Ethernet (RJ-45) | Cat6 Ethernet | Router LAN Port 1 | Computer desk |

Router LAN Port Usage:

- LAN1 → Desktop PC  
- LAN2 → Available  
- LAN3 → Available  
- LAN4 → Available  

## Bedroom Layout

| Device | Interface | Frequency Band | Connected To |
|-------|-----------|---------------|--------------|
| Laptop | WiFi Adapter | 5 GHz | Wireless Router |
| Smartphone | WiFi Adapter | 5 GHz | Wireless Router |
| Smart TV | WiFi Adapter | 2.4 GHz | Wireless Router |

## Physical Topology Diagram

```text
Fiber ISP Line
      │
      ▼
ISP Modem
      │ (Cat6)
      ▼
Wireless Router
   │        │        │
Desktop   Laptop   Smart TV / Phone
(Cat6)    (WiFi)      (WiFi)

---

# 2. Logical Network Topology

The logical topology of the home network follows a star topology where all devices connect through a central wireless router. The router acts as the default gateway and manages communication between internal devices and the internet.

Logical flow:

Internet → ISP Modem → Wireless Router → Connected Devices

The router provides the following services:

- DHCP (automatic IP address assignment)
- NAT (Network Address Translation)
- Firewall protection
- DNS forwarding
- Wireless access control

## Network Topology Diagram

![Home Network Topology](Downloads/topology.drawio.png)

---

# 3. Addressing Documentation

Private IP addressing scheme:

Network Range: 192.168.1.0/24

Default Gateway: 192.168.1.1

DHCP Range: 192.168.1.100 – 192.168.1.200

Device Address Table:

| Device | IP Address | Connection Type |
|--------|------------|----------------|
| Router | 192.168.1.1 | Ethernet |
| Desktop | 192.168.1.10 | Ethernet |
| Laptop | 192.168.1.20 | WiFi |
| Smartphone | 192.168.1.30 | WiFi |
| Smart TV | 192.168.1.40 | WiFi |

---

# 4. Network Devices and Services

The following devices are connected in the home network:

ISP Modem

Provides internet connectivity from the service provider.

Wireless Router

Acts as the central networking device and provides:

- DHCP
- NAT
- Firewall protection
- Wireless connectivity

Desktop Computer

Connected using Ethernet cable and used for coursework and documentation.

Laptop

Connected using WiFi for assignments and online learning.

Smartphone

Connected wirelessly for communication and internet browsing.

Smart TV

Connected wirelessly for streaming services.

---

# 5. Device Configurations

Router configuration:

Router IP address: 192.168.0.1  
DHCP enabled: Yes  
Firewall enabled: Yes  
Wireless security: WPA2/WPA3  

Desktop configuration:

Connection type: Ethernet  
IP assignment: Automatic (DHCP)

Laptop configuration:

Connection type: WiFi  
Frequency band: 5 GHz

---

# 6. Secure Storage of Login Credentials

All network login credentials are securely stored using Microsoft Edge Password Manager.

Additional protection methods:

- Strong passwords enabled
- Two-factor authentication enabled
- Router admin password changed from default
- WiFi password secured using WPA2 encryption
