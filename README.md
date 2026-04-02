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
