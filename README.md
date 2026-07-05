# Enterprise Network Design using Cisco Packet Tracer

## Overview
This project demonstrates the design and implementation of a small enterprise network using Cisco Packet Tracer. The network is divided into multiple departments using VLANs, with inter-VLAN communication enabled through Router-on-a-Stick. Automatic IP address allocation is provided using DHCP, and a web server is hosted within a dedicated server VLAN.

## Features
- VLAN Segmentation
  - VLAN 10 – IT Department
  - VLAN 20 – Admin Department
  - VLAN 50 – Server Network
- Router-on-a-Stick for Inter-VLAN Routing
- DHCP for Automatic IP Address Assignment
- DNS for Hostname Resolution
- HTTP Web Server Hosting
- End-to-End Network Connectivity Testing

## Network Topology

```
                  Router (Cisco 2901)
                        |
                     Trunk Link
                        |
                  Core Switch (2960)
              _________|___________
             |                     |
         IT Switch            Admin Switch
             |                     |
        IT PCs                Admin PCs
             |
          Web Server
```

## IP Addressing Scheme

| VLAN | Department | Network |
|------|------------|----------------|
| 10 | IT | 192.168.10.0/24 |
| 20 | Admin | 192.168.20.0/24 |
| 50 | Server | 192.168.50.0/24 |

## Technologies Used

- Cisco Packet Tracer
- Cisco 2901 Router
- Cisco 2960 Switches
- VLAN
- Router-on-a-Stick
- DHCP
- DNS
- HTTP

## Implementation

### VLAN Configuration
Configured VLANs to logically separate the IT, Admin, and Server networks.

### Trunk Links
Configured trunk ports between the core switch, access switches, and router to carry multiple VLANs.

### Inter-VLAN Routing
Implemented Router-on-a-Stick using router subinterfaces to enable communication between VLANs.

### DHCP
Configured DHCP pools to automatically assign IP addresses to devices in each VLAN.

### DNS
Configured DNS to allow access to the web server using a hostname instead of an IP address.

### Web Server
Hosted a basic HTML webpage on the server using the HTTP service available in Cisco Packet Tracer.

## Testing Performed

- DHCP IP allocation verified
- Inter-VLAN communication verified using Ping
- Web server accessibility verified using a web browser
- DNS hostname resolution verified

## Learning Outcomes

Through this project, I gained hands-on experience in:

- VLAN configuration
- Switch trunking
- Router-on-a-Stick
- DHCP configuration
- DNS configuration
- HTTP server deployment
- Enterprise network design
- Cisco IOS CLI troubleshooting

## Future Enhancements

- Implement Access Control Lists (ACLs)
- Configure SSH for secure remote management
- Add Network Address Translation (NAT)
- Expand topology with additional departments
- Implement Dynamic Routing Protocols (OSPF)


**Mo**
