# Enhancing Fault Tolerance and Network Efficiency through Advanced HSRP and OSPF Integration

## Overview
This project aims to improve network fault tolerance and routing efficiency by integrating **Hot Standby Router Protocol (HSRP)** and **Open Shortest Path First (OSPF)**. Using **GNS3**, the network comprises three routers: two configured with HSRP for redundancy and one using OSPF for dynamic routing. The objective is to ensure network availability and efficient routing, even in the event of router failure.

## Key Features
- **HSRP for Redundancy**: HSRP provides seamless failover between two routers (R1 and R2), ensuring continuous data flow even if one router fails.
- **OSPF for Dynamic Routing**: OSPF intelligently routes traffic based on the most efficient path, adjusting dynamically to network changes.
- **Failover Testing**: Multiple failover scenarios were tested, demonstrating the resilience of the network in real-time.

## Network Topology
- **Routers**: 
  - R1 and R2 are configured with HSRP, where one acts as a backup for the other.
  - R3 connects to an external network via OSPF.
- **Clients**: Simulated PCs connect to the network, routing through Virtual IPs managed by HSRP.
- **Failover Handling**: R1 is the active router, with R2 as standby. If R1 fails, R2 automatically takes over without interruption.

## Objectives
- Achieve **100% uptime** through redundancy with HSRP.
- Ensure **optimal routing** and traffic efficiency using OSPF.
- Seamlessly handle failovers with no manual intervention.

## Future Enhancements
- **Expand Network Scalability**: Test HSRP and OSPF in larger, more complex topologies.
- **Automate Network Management**: Integrate security protocols such as IPsec and ACLs for enhanced network protection.
- **Performance Monitoring**: Utilize advanced tools for real-time traffic analysis and optimization.

## Conclusion
This project demonstrates the successful integration of HSRP and OSPF to create a robust, fault-tolerant network capable of handling real-world traffic demands with minimal downtime.

---

### References:
- [How to Configure OSPF in GNS3 - OSPF Routing Configuration Step by Step](https://youtu.be/Iib20MF8y-c?si=eKBCga6e_pJDl5_y)
- [How to configure Hot Standby Router Protocol (HSRP) in GNS3](https://www.youtube.com/watch?v=TnoOAps8pM0)
- [Hot Standby Router Protocol (HSRP) - GeeksforGeeks](https://www.geeksforgeeks.org/hot-standby-router-protocol-hsrp/)

---
