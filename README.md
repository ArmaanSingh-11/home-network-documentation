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

---

# 3. Addressing Documentation

Network address range:

192.168.0.0/24

Subnet mask:

255.255.255.0

Default gateway:

192.168.0.1

DNS servers:

8.8.8.8
8.8.4.4

DHCP range:

192.168.0.10 – 192.168.0.100

Device address table:

| Device | IP Address | Interface | Assignment |
|--------|------------|-----------|------------|
| Router | 192.168.0.1 | LAN | Static |
| Desktop PC | 192.168.0.10 | Ethernet | DHCP |
| Laptop | 192.168.0.11 | WiFi | DHCP |
| Smartphone | 192.168.0.12 | WiFi | DHCP |
| Smart TV | 192.168.0.13 | WiFi | DHCP |

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

Login credentials for the router and wireless network are stored securely using an encrypted password manager.

Security measures implemented include:

- Router default password changed
- Strong passwords used
- WPA2/WPA3 wireless encryption enabled
- Credentials not stored in plain text
- Remote management disabled

