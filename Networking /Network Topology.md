Network structure determines communication patterns, fault tolerance, and scalability. Key topologies include:

---
## Mesh Topology  
**Structure**:  
- **Full Mesh**: Every node connected to every other node  
- **Partial Mesh**: Selective node interconnections  

**Advantages**:  
- **Fault Tolerance**: Automatic rerouting via alternative paths  
- **High Reliability**: No single point of failure  
- **Optimized for MANs**: Common in metropolitan area networks  

**Disadvantages**:  
- **Cost**: High cabling complexity (N*(N-1)/2 connections)  
- **Scalability**: Impractical for >100 nodes  

**Use Case**:  
- Military networks, financial backbone systems  
![[Pasted image 20250227171645.png]]  
*Fig. 1.11: Full mesh topology with redundant paths.*  

---

## Tree Topology  
**Hierarchical Structure**:  
- **Root Node**: Central authority (e.g., core router)  
- **Parent-Child Links**: Strict hierarchy without loops  

**Failure Impact**:  
- **Root Failure**: Network splits into isolated segments  
- **Leaf Failure**: Minimal disruption  

**Applications**:  
- Corporate intranets, hierarchical database systems  
![[Pasted image 20250227171719.png]]  
*Fig. 1.12: Tree topology with root-server dependency.*  

---

## Bus Topology  
**Key Features**:  
- **Shared Medium**: All nodes connect to a single backbone (bus)  
- **Collision Handling**:  
  - **CSMA/CD**: Carrier-sense multiple access with collision detection  
  - **Bus Master**: Controls transmission rights (prevents collisions)  

**Limitations**:  
- **Bandwidth Contention**: Performance degrades with >20 nodes  
- **Single Point of Failure**: Bus cable failure disables entire network  

**Protocols**:  
- **Ethernet (IEEE 802.3)**: Dominant standard for wired LANs  

![[Pasted image 20250227171741.png]]  
*Fig. 1.13: Bus topology with collision domains.*  

---

## Star Topology  
**Centralized Architecture**:  
- **Hub/Switch**: Central node managing all traffic  
- **Point-to-Point Links**: Dedicated connections from devices to hub  

**Advantages**:  
- **Ease of Management**: Centralized monitoring  
- **Scalability**: Add/remove nodes without disrupting network  

**Disadvantages**:  
- **Hub Dependency**: Central node failure = network outage  
- **Latency**: All traffic passes through central node  

**Modern Implementations**:  
- Wi-Fi access points (logical star topology)  
![[Pasted image 20250227171757.png]]  
*Fig. 1.14: Star topology with central switch.*  

---

## Ring Topology  
**Token-Passing Mechanism**:  
- **Token Frame**: Special 3-byte packet (IEEE 802.5 standard)  
- **Deterministic Access**: Nodes transmit only when holding token  

**Performance**:  
- **Throughput**: 4-16 Mbps (traditional Token Ring)  
- **Latency**: Predictable due to ordered token circulation  

**Fault Tolerance**:  
- **Dual Ring**: Redundant counter-rotating rings (FDDI standard)  

**Legacy Use**:  
- IBM Token Ring (displaced by Ethernet)  
![[Pasted image 20250227171814.png]]  
*Fig. 1.15: Unidirectional ring with token circulation.*  

---

## Hybrid Topologies  
**Common Combinations**:  
- **Star-Wired Bus**: Ethernet with hierarchical switches  
- **Star-Ring**: Token Ring networks using MAUs (Multistation Access Units)  

**Modern Evolution**:  
- **Spine-Leaf**: Data center hybrid (tree + mesh principles)  
![[Pasted image 20250227171832.png]]  
*Fig. 1.16: Star-bus hybrid topology example.*  

---

## Topology Comparison Matrix  
| Factor          | Mesh      | Tree      | Bus       | Star      | Ring      |
|-----------------|-----------|-----------|-----------|-----------|-----------|
| **Fault Tolerance** | Excellent | Low       | Poor      | Moderate  | High      |
| **Scalability** | Limited   | Moderate  | Low       | High      | Low       |
| **Cost**        | Very High | Moderate  | Low       | Moderate  | High      |
| **Latency**     | Low       | Variable  | High      | Moderate  | Predictable |
| **Use Case**    | WAN backbones | Hierarchical systems | Small LANs | Enterprise LANs | Legacy systems |

