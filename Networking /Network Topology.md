A **network topology** refers to how devices (like computers, servers, and routers) are connected in a network. The choice of topology affects the performance, reliability, and scalability of the network. Here are the most common types of network topologies:

---
### 1. **Mesh Topology**

- **How It Works** : Every device is connected to every other device directly or indirectly.
- **Key Features** :
    - Multiple paths between devices.
    - If one connection fails, data can take an alternate route.
- **Pros** :
    - Highly reliable because the network continues to work even if one device fails.
    - No single point of failure.
- **Cons** :
    - Expensive due to the large number of connections.
    - Complex to set up and maintain.
- **Best For** : Large networks like MANs (Metropolitan Area Networks).
![[Pasted image 20250220195342.png]]
---

### 2. **Tree Topology**

- **How It Works** : Devices are arranged in a hierarchical structure, like an upside-down tree.
    - The **root** is the main device, and other devices branch out from it.
- **Key Features** :
    - Devices have a parent-child relationship.
    - No loops in the structure.
- **Pros** :
    - Easy to expand by adding branches.
    - Suitable for large networks.
- **Cons** :
    - If the root device fails, the entire network splits or stops working.
    - Troubleshooting can be difficult.
- **Best For** : Hierarchical networks like corporate systems.
![[Pasted image 20250220195359.png]]
---

### 3. **Bus Topology**

- **How It Works** : All devices share a single communication line called a **bus** .
- **Key Features** :
    - Data travels along the bus and can be received by all devices.
    - A mechanism is needed to prevent collisions when multiple devices try to send data at the same time.
- **Pros** :
    - Simple and cost-effective to set up.
    - Easy to add new devices.
- **Cons** :
    - Performance decreases as more devices are added.
    - If the bus fails, the entire network goes down.
- **Collision Control** :
    - Uses a **collision detection system** (e.g., Ethernet).
    - Only one device can transmit at a time (called the "bus master").
- **Best For** : Small LANs (Local Area Networks).
![[Pasted image 20250220195416.png]]
---

### 4. **Star Topology**

- **How It Works** : All devices are connected to a central hub or switch.
- **Key Features** :
    - Communication between devices must pass through the central hub.
    - The hub can broadcast data to all devices or send it only to the intended recipient.
- **Pros** :
    - Easy to manage and troubleshoot.
    - Adding or removing devices doesn’t affect the rest of the network.
- **Cons** :
    - If the central hub fails, the entire network stops working.
    - Requires more cables than other topologies.
- **Best For** : LANs in homes, offices, and small businesses.
![[Pasted image 20250220195440.png]]
---

### 5. **Ring Topology**

- **How It Works** : Devices are connected in a circular loop, and data travels in one direction around the ring.
- **Key Features** :
    - Uses a **token system** to manage data transmission.
    - The token ensures only one device can send data at a time.
- **Token System** :
    - A device must hold the token to transmit data.
    - After transmitting, the token is passed to the next device.
- **Pros** :
    - Prevents data collisions.
    - Ensures fair access to the network.
- **Cons** :
    - If one device or connection fails, the entire ring can stop working.
    - Adding or removing devices disrupts the network.
- **Best For** : Token Ring networks.
![[Pasted image 20250220195537.png]]![[Pasted image 20250220195501.png]]
---

### 6. **Hybrid Topologies**

- **How It Works** : Combines two or more topologies (e.g., star + bus, star + ring).
- **Examples** :
    - **Star-Bus** : A star network where each hub is connected via a bus.
    - **Stretched Star** : A star network extended over a larger area.
- **Pros** :
    - Flexible and scalable.
    - Can combine the strengths of different topologies.
- **Cons** :
    - More complex to design and manage.

---

### Popular LAN Topologies

- **Bus Topology** : Commonly used in older Ethernet networks.
- **Star Topology** : Most popular in modern Ethernet networks.
- **Ring Topology** : Used in Token Ring networks.

---

### Factors Influencing Topology Choice

The choice of topology depends on:

1. **Type of Transmission Medium** : Wired or wireless.
2. **Reliability** : How critical uptime is for the network.
3. **Size of the Network** : Number of devices and coverage area.
4. **Future Growth** : Scalability for adding more devices.

---

### Summary

| Topology | How It Works                               | Pros                                        | Cons                                | Best For               |
| -------- | ------------------------------------------ | ------------------------------------------- | ----------------------------------- | ---------------------- |
| **Mesh** | Every device connects to every other.      | Highly reliable, no single point of failure | Expensive, complex setup            | Large networks (MANs). |
| **Tree** | Hierarchical structure like a tree.        | Easy to expand, scalable                    | Root failure crashes the network    | Corporate networks.    |
| **Bus**  | Devices share a single communication line. | Simple, cost-effective                      | Performance drops with more devices | Small LANs.            |
| **Star** | All devices connect to a central hub.      | Easy to manage, scalable                    | Hub failure crashes the network     | Home/office LANs.      |
| **Ring** | Devices form a circular loop.              | Prevents collisions, fair access            | Single failure disrupts the network | Token Ring networks.   |

Each topology has its strengths and weaknesses, so the choice depends on the specific needs of the network!