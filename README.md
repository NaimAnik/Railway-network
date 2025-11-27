## Railway Networking System Simulation

### Course & Context
* Project Goal: To design a reliable, secure, and efficient computer network simulation for a modern railway platform and its administrative zones.
* Simulation Tool: Cisco Packet Tracer.

---

### Implemented Features

* **Network Segmentation:** Logically divided the entire network into distinct operational zones (Authority, Passenger, VIP Zone, Platform).
* **IP Management (VLSM):** Used Variable Length Subnet Masking (VLSM) for efficient network segmentation and IP address optimization (e.g., 192.168.10.0/24, 192.168.20.0/24).
* **DHCP:** Automatically assigns IP addresses to devices across multiple subnets.
* **DNS Service:** Enables domain resolution for internal services (e.g., www.railwayportal.com).
* **HTTP Service:** Hosts simulated internal web applications (Daily Train Schedule, Ticket Booking System interface).
* **Routing:** Static Routes were configured between routers for secure and documented connectivity.
* **Security:** Wireless access points (for Passenger and VIP zones) are secured with WPA2 encryption.

---

### Network Zone Overview

1.  **Authority (192.168.20.0/24):** High security, hosts DNS and HTTP servers.
2.  **Passenger (192.168.10.0/24):** General public access, DHCP enabled.
3.  **Platform/Ticket Gate (192.168.30.0/24):** Designated for information displays and gate control.
4.  **VIP Zone (192.168.40.0/24):** Higher privilege access, secured wireless.

---

### Future Enhancements

* **VLAN Implementation:** For stronger broadcast domain separation and granular traffic control.
* **External Threat Protection:** Introduce dedicated **Firewalls**.
* **Redundancy Protocols:** Implement **HSRP (Hot Standby Router Protocol)**.
* **Advanced Monitoring:** Integrate **SNMP (Simple Network Management Protocol)**.
* **Expanded Functionality:** Deploy **IP cameras** and **VoIP** services.
