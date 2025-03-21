Before we discuss network connecting devices, let us revisit the network infra- structure. We have defined a network as a mesh of network elements, commonly referred to as network nodes, connected together by conducting media. These network nodes can be either at the ends of the mesh, in which case they are com- monly known as clients or in the middle of the network as transmitting elements. In a small network such as a LAN, the nodes are connected together via special connecting and conducting devices that take network traffic from one node and pass it on to the next node. If the network is big Internetwork (large networks of networks like WANs and LANs), these networks are connected to other special intermediate networking devices so that the Internet functions as a single large network. Now let us look at network connecting devices and focus on two types of devices: those used in networks (small networks such as LANs) and those used in internet- works.


## LAN Connecting Devices

Because LANs are small networks, connecting devices in LANs are less powerful with limited capabilities. There are hubs, repeaters, bridges, and switches.

### A Hub

This is the simplest in the family of network connecting devices since it connects the LAN components with identical protocols. It takes in imports and re-transmits them verbatim. It can be used to switch both digital and analog data. In each node, pre-setting must be done to prepare for the formatting of the incoming data. For example, if the incoming data is in digital format, the hub must pass it on as pack- ets; however, if the incoming data is analog, then the hub passes as a signal. There are two types of hubs: simple and multiple port hubs, as shown in Figs. 1.23 and 1.24. Multiple ports hubs may support more than one computer up to its number of ports and may be used to plan for the network expansion as more computers are added at a later time.

![[Pasted image 20250321104700.png]]

Network hubs are designed to work with network adapters and cables and can typically run at either 10 Mbps or 100 Mbps; some hubs can run at both speeds. To connect computers with differing speeds, it is better to use hubs that run at both speeds 10/100 Mbps.

### A Repeater

A network repeater is a low-level local communication device at the physical layer of the network that receives network signals, amplifies them to restore them to full strength, and then re-transmits them to another node in the network. Repeaters are used in a network for several purposes including countering the attenuation that occurs when signals travel long distances, and extending the length of the LAN above the specified maximum. Since they work at the low- est network stack layer, they are less intelligent than their counterparts such as bridges, switches, routers, and gateways in the upper layers of the network stack. See Fig. 1.25.
![[Pasted image 20250321104821.png]]
### A Bridge

A bridge is like a repeater but differs in that a repeater amplifies electrical signals because it is deployed at the physical layer; a bridge is deployed at the datalink and therefore amplifies digital signals. It digitally copies frames. It permits frames from one part of a LAN or a different LAN with different technology to move to another part or another LAN. However, in filtering and isolating a frame from one network to another or another part of the same network, the bridge will not move a dam- aged frame from one end of the network to the other. As it filters the data packets, the bridge makes no modifications to the format and content of the incoming data. A bridge filters the frames to determine whether a frame should be forwarded or dropped. All “noise” (collisions, faulty wiring, power surges, etc.) packets are not transmitted. The bridge filters and forwards frames on the network using a dynamic bridge table. The bridge table, which is initially empty, maintains the LAN addresses for each computer in the LAN and the addresses of each bridge inter- face that connects the LAN to other LANs. Bridges, like hubs, can be either simple or multi-ported. Figure 1.26 shows a simple bridge, Fig. 1.27 shows a multi-ported bridge, and Fig. 1.28 shows the position of the bridge in an OSI protocol stack.

![[Pasted image 20250321104942.png]]
### A Switch

A switch is a network device that connects segments of a network or two small networks such as Ethernet or token ring LANs. Like the bridge, it also filters and forwards frames on the network with the help of a dynamic table. This point-to-point approach allows the switch to connect multiple pairs of segments at a time, allowing more than one computer to transmit data at a time, thus giving them a high performance over their cousins, the bridges.
![[Pasted image 20250321105044.png]]
## Internet working Devices

### Routers

Routers are general purpose devices that interconnect two or more heterogeneous networks represented by IP subnets or unnumbered point to point lines. They are usually dedicated special-purpose computers with separate input and output inter- faces for each connected network. They are implemented at the network layer in the protocol stack. Figure 1.29 shows the position of the router in the OSI protocol stack.

According to RFC 1812, a router performs the following functions:

- Conforms to specific Internet protocols specified in the 1812 document, including• the Internet protocol (IP), Internet control message protocol (ICMP), and others as necessary.
- Connects to two or more packet networks. For each connected network, the• router must implement the functions required by that network because it is a member of that network. These functions typically include the following:
	- Encapsulating and decapsulating the IP datagrams with the connected• network framing. For example, if the connected network is an Ethernet LAN, an Ethernet header and checksum must be attached.
- Sending and receiving IP datagrams up to the maximum size supported by• that network; this size is the network’s maximum transmission unit or MTU.
- Translating the IP destination address into an appropriate network-level• address for the connected network. These are the Ethernet hardware address on the NIC, for Ethernet cards, if needed. Each network addresses the router as a member computer of its own network. This means that each router is a member of each network it connects to. It, therefore, has a network host address for that network and an interface address for each network it is connected to. Because of this rather strange characteristic, each router interface has its own address resolution protocol (ARP) module, its LAN address (network card address), and its own Internet protocol (IP) address.
- Responding to network flow control and error indications, if any