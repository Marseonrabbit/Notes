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
![[Pasted image 20250321105950.png]]

According to RFC 1812, a router performs the following functions:

- Conforms to specific Internet protocols specified in the 1812 document, including• the Internet protocol (IP), Internet control message protocol (ICMP), and others as necessary.
- Connects to two or more packet networks. For each connected network, the• router must implement the functions required by that network because it is a member of that network. These functions typically include the following:
	- Encapsulating and decapsulating the IP datagrams with the connected• network framing. For example, if the connected network is an Ethernet LAN, an Ethernet header and checksum must be attached.
	- Sending and receiving IP datagrams up to the maximum size supported by• that network; this size is the network’s maximum transmission unit or MTU.
	- Translating the IP destination address into an appropriate network-level• address for the connected network. These are the Ethernet hardware address on the NIC, for Ethernet cards, if needed. Each network addresses the router as a member computer of its own network. This means that each router is a member of each network it connects to. It, therefore, has a network host address for that network and an interface address for each network it is connected to. Because of this rather strange characteristic, each router interface has its own address resolution protocol (ARP) module, its LAN address (network card address), and its own Internet protocol (IP) address.
	- Responding to network flow control and error indications, if any.
- Receives and forwards Internet datagrams. Important issues in this process are• buffer management, congestion control, and fairness. To do this the router must.
	- Recognize error conditions and generate ICMP error and information• messages as required.
	- Drop datagrams whose time-to-live fields have reached zero.
	- Fragment datagrams when necessary to fit into the maximum transmission• unit (MTU) of the next network.
- Chooses a next-hop destination for each IP datagram based on the information• in its routing database.
- Usually supports an interior gateway protocol (IGP) to carry out distributed• routing and reachability algorithms with the other routers in the same autonomous system. In addition, some routers will need to support an exterior gateway protocol (EGP) to exchange topological information with other autonomous systems.
- Usually supports an interior gateway protocol (IGP) to carry out distributed• routing and reachability algorithms with the other routers in the same autonomous system. In addition, some routers will need to support an exterior gateway protocol (EGP) to exchange topological information with other autonomous systems.
- Provides network management and system support facilities, including loading,• debugging, status reporting, exception reporting, and control.

Forwarding an IP datagram from one network across a router requires the router to choose the address and relevant interface of the next-hop router or for the final hop if it is the destination host. The next-hop router is always in the next network of which the router is also a member. The choice of the next-hop router, called for- warding, depends on the entries in the routing table within the router.

Routers are smarter than bridges in that the router with the use of a router table has some knowledge of possible routes a packet could take from its source to its destination. Once it finds the destination, it determines the best, fastest, and most efficient way of routing the package. The routing table, like in the bridge and switch, grows dynamically as activities in the network develop. On receipt of a packet, the router removes the packet headers and trailers and analyzes the IP header by deter- mining the source and destination addresses and data type and noting the arrival time. It also updates the router table with new addresses if not already in the table. The IP header and arrival time information is entered in the routing table. If a router encounters an address it cannot understand, it drops the package. Let us explain the working of a router by an example using Fig. 1.30

In Fig. 1.30, suppose host A in LAN1 tries to send a packet to host B in LAN2. Both host A and host B have two addresses: the LAN (host) address and the IP address. The translation between host LAN addresses and IP addresses is done by the ARP, and data is retrieved or built into the ARP table, similar to Table 1.4. Notice also that the router has two network interfaces: interface 1 for LAN1 and interface 2 for LAN2 for the connection to a larger network such as the Internet. Each inter- face has a LAN (host) address for the network the interface connects on and a cor- responding IP address. As we will see later in the chapter, host A sends a packet to router 1 at time 10:01 that includes, among other things, both its addresses, message type, and destination IP address of host B. The packet is received at interface 1 of the router; the router reads the packet and builds row 1 of the routing table as shown in Table 1.5.

The router notices that the packet has to go to network 193.55.1.***, where *** are digits 0–9, and it has knowledge that this network is connected on interface It forwards the packet to interface 2. Now, interface 2 with its own ARP may know host B. If it does, then it forwards the packet and updates the routing table with the inclusion of row 2. What happens when the ARP at the router interface 1 cannot determine the next network? That is, if it has no knowledge of the pres- ence of network 193.55.1.***, it will then ask for help from a gateway. Let us now discuss how IP chooses a gateway to use when delivering a datagram to a remote network

![[Pasted image 20250321110034.png]]
![[Pasted image 20250321110225.png]]

### Gateways

Gateways are more versatile devices than routers. They perform protocol conver- sion between different types of networks, architectures, or applications and serve as translators and interpreters for network computers that communicate in differ- ent protocols and operate in dissimilar networks, for example, OSI and TCP/IP. Because the networks are different with different technologies, each network has its own routing algorithms, protocols, domain names servers, and network administra- tion procedures and policies. Gateways perform all of the functions of a router and more. The gateway functionality that does the translation between different network technologies and algorithms is called a protocol converter. Figure 1.31 shows the position of a gateway in a network.

Gateways services include packet format and/or size conversion, protocol con- version, data translation, terminal emulation, and multiplexing. Since gateways per- form a more complicated task of protocol conversion, they operate more slowly and handle fewer devices.

Let us now see how a packet can be routed through a gateway or several gate- ways before it reaches its destination. We have seen that if a router gets a datagram, it checks the destination address and finds that it is not on the local network. It, therefore, sends it to the default gateway. The default gateway now searches its table for the destination address. In case the default gateway recognizes that the destination address is not on any of the networks it is connected to directly, it has to find yet another gateway to forward it through.

![[Pasted image 20250321112900.png]]

The routing information the server uses for this is in a gateway routing table link- ing networks to gateways that reach them. The table starts with the network entry 0.0.0.0, a catch-all entry, for default routes. All packets to an unknown network are sent through the default route. Table 1.6 shows the gateway routing table. The choice between a router, a bridge, and a gateway is a balance between func- tionality and speed. Gateways, as we have indicated, perform a variety of functions; however, because of this variety of functions, gateways may become bottlenecks within a network because they are slow. Routing tables may be built either manually for small LANs or by using software called routing daemons for larger networks.