# University Network Design: Backbone & Departmental Implementation

This project outlines the design and implementation of a robust and scalable network infrastructure for the University of Moratuwa (UOM) and, specifically, the Electronic and Telecommunication Engineering (ENTC) Department. Leveraging Cisco Packet Tracer, this solution focuses on high availability, efficient routing, and simplified device management.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Network Design Principles](#network-design-principles)
- [Implementation Details](#implementation-details)
- [Project Files & Structure](#project-files--structure)
- [Network Topologies](#network-topologies)
- [How to Open and Run](#how-to-open-and-run)
- [Acknowledgements](#acknowledgements)

---

## Project Overview

This project simulates the network infrastructure of the University of Moratuwa, distinguishing between a university-wide backbone and a detailed departmental network for the ENTC faculty. The design prioritizes **redundancy**, **efficient routing**, and **ease of management** to ensure continuous and reliable connectivity for all users and services.

The entire implementation is carried out using **Cisco Packet Tracer**, providing a practical and verifiable simulation environment for the proposed network architecture.

## Key Features

- **Hybrid Network Topology**: Implemented a combination of **star and mesh topologies** to ensure high availability and prevent single points of failure, crucial for a critical network like a university backbone.
- **OSPF Routing Protocol**: Utilized **Open Shortest Path First (OSPF)** for dynamic and efficient packet routing within and between network segments, enabling fast convergence and load balancing.
- **DHCP for IP Address Management**: Configured **Dynamic Host Configuration Protocol (DHCP)** to automatically assign IP addresses to devices, simplifying network administration and reducing manual configuration errors.
- **Scalable Design**: The architecture is designed to be scalable, allowing for future expansion and integration of additional departments or services without major re-designs.

---

## Network Design Principles

The network design adheres to modern best practices, focusing on:

-   **High Availability**: Through redundant links and a mix of topologies, connectivity is maintained even in the event of component failures.
-   **Performance**: OSPF ensures optimal path selection and fast routing decisions, minimizing latency.
-   **Manageability**: DHCP simplifies IP management, while structured segmentation aids troubleshooting.
-   **Security**: While not the primary focus, the layered design provides a foundation for future security enhancements.

## Implementation Details

### University Backbone Network
The university backbone serves as the core interconnecting various faculties, administrative blocks, and key services. Its design emphasizes high bandwidth and redundancy to handle aggregated traffic effectively.

### ENTC Department Network
The ENTC department network is designed to cater to the specific needs of students and staff, including labs, lecture halls, and offices. It integrates seamlessly with the university backbone while providing localized services and efficient internal communication.

## Project Files & Structure
```
Network-Design-UOM/
├── Backbone_of_the_University/
│ └── backbone.pkt # Cisco Packet Tracer file for the UOM backbone network
│
├── Department_Network/
│ └── ENTCdepartment.pkt # Cisco Packet Tracer file for the ENTC department network (assuming this name)
│
├── Images/
│ ├── university_backbone_topology.png # Image of the University Backbone topology
│ ├── entc_department_topology.png # Image of the ENTC Department network topology
│ ├── ospf_configuration_example.png # Screenshot of OSPF configuration (optional)
│ └── dhcp_configuration_example.png # Screenshot of DHCP configuration (optional)
│
└── README.md # This documentation file
```
**Note:** I've assumed the ENTC departmental file is named `entc_department.pkt`. Please adjust the name in the file structure and the guide below if it's different.

---

## Network Topologies

### University Backbone Network Topology

This diagram illustrates the robust and redundant backbone network of the University of Moratuwa, designed to connect all major faculties and administrative units.

![University Backbone Network Topology](./Images/university_backbone_topology.png)
*Figure 1: High-level view of the University of Moratuwa's backbone network in Cisco Packet Tracer.*

### ENTC Department Network Topology

This diagram provides a detailed view of the Electronic and Telecommunication Engineering (ENTC) Department's network, showcasing its internal structure and connection points to the university backbone.

![ENTC Department Network Topology](./Images/entc_department_topology.png)
*Figure 2: Detailed topology of the ENTC Department's network, highlighting internal device connections.*

### Configuration Examples (Optional - Add if you have screenshots)

To further illustrate the implementation, here are examples of key configurations:

#### OSPF Configuration Example
![OSPF Configuration Snippet](./Images/ospf_configuration_example.png)
*Figure 3: Snippet from a router's OSPF configuration in Cisco Packet Tracer.*

#### DHCP Configuration Example
![DHCP Configuration Snippet](./Images/dhcp_configuration_example.png)
*Figure 4: Example of DHCP server configuration for automated IP assignment.*

---

## How to Open and Run

1.  **Install Cisco Packet Tracer**: Ensure you have Cisco Packet Tracer (version 7.x or later recommended) installed on your system. You can download it from the Cisco Networking Academy website.
2.  **Clone or Download Repository**: Clone this GitHub repository to your local machine.
3.  **Open .pkt Files**:
    *   Navigate to the `Backbone_of_the_University` folder and open `backbone.pkt` with Cisco Packet Tracer.
    *   Navigate to the `Department_Network` folder and open `entc_department.pkt` with Cisco Packet Tracer.
4.  **Explore and Simulate**: Once opened, you can:
    *   Inspect device configurations (CLI, GUI).
    *   Run Pings and Traceroutes to verify connectivity and routing paths.
    *   Switch to Simulation Mode to observe packet flow.

---

## Acknowledgements

This project was developed as part of a network design course/module at the University of Moratuwa.

---

*Designed and Implemented by [Your Name/Team Name]*

