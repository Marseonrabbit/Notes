For a communication network to work effectively, data in the network must be able to move from one network element to another. This can only happen if the network services to move such data work. For data networks, these services fall into two categories:

- Connection services to facilitate the exchange of data between the two network• communicating end-systems with as little data loss as possible and in as little time as possible
- Switching services to facilitate the movement of data from host to host across• the length and width of the network mesh of hosts, hubs, bridges, routers, and gateways

## Connection Services

How do we get the network transmitting elements to exchange data over the network? Two types of connection services are used: the connected-oriented and connectionless services.

### Connected-Oriented Services

With a connection-oriented service, before a client can send packets with real data to the server, there must be a three-way handshake. We will define this three-way handshake in later chapters. But the purpose of a three-way handshake is to estab- lish a session before the actual communication can begin. Establishing a session before data is moved creates a path of virtual links between the end systems through a network and therefore, guarantees the reservation and establishment of fixed com- munication channels and other resources needed for the exchange of data before any data is exchanged and as long as the channels are needed. For example, this happens whenever we place telephone calls; before we exchange words, the channels are reserved and established for the duration. Because this technique guarantees that data will arrive in the same order it was sent in, it is considered to be reliable. In short the service offers the following:

- Acknowledgments of all data exchanges between the end-systems,
- Flow control in the network during the exchange, and
- Congestion control in the network during the exchange

 Depending on the type of physical connections in place and the services required by the systems that are communicating, connection-oriented methods may be implemented in the data link layers or in the transport layers of the protocol stack, although the trend now is to implement it more at the transport layer. For example, TCP is a connection-oriented transport protocol in the transport layer. Other network technologies that are connection-oriented include the frame relay and ATMs.

### Connectionless Service

In a connectionless service, there is no handshaking to establish a session between the communicating end-systems, no flow control, and no congestion control in the network. This means that a client can start communicating with a server without warning or inquiry for readiness; it simply sends streams of packets, called data- grams, from its sending port to the server’s connection port in single point-to-point transmissions with no relationship established between the packets and between the end-systems. There are advantages and of course disadvantages to this type of con- nection service. In brief, the connection is faster because there is no handshaking which can sometimes be time consuming, and it offers periodic burst transfers with large quantities of data and, in addition, it has simple protocol. However, this service offers minimum services, no safeguards and guarantees to the sender since there is no prior control information and no acknowledgment. In addition, the service does not have the reliability of the connection-oriented method, and offers no error han- dling and no packets ordering; in addition, each packet self-identifies that leads to long headers, and finally, there is no predefined order in the arrival of packets.

Like the connection-oriented method, this service can operate both at the data link and transport layers. For example, UDP, a connectionless service, operates at the transport layer




## Network Switching Services

Before we discuss communication protocols, let us take a detour and briefly discuss data transfer by a switching element. This is a technique by which data is moved from host to host across the length and width of the network mesh of hosts, hubs, bridges, routers, and gateways. This technique is referred to as data switching. The type of data switching technique used by a network determines how messages are transmitted between the two communicating elements and across that network. There are two types of data switching techniques: circuit switching and packet switching.

### Circuit Switching

In circuit switching networks, one must reserve all the resources before setting up a physical communication channel needed for communication. The physical con- nection, once established, is then used exclusively by the two end-systems, usually subscribers, for the duration of the communication. The main feature of such a con- nection is that it provides a fixed data rate channel, and both subscribers must oper- ate at this rate. For example, in a telephone communication network, a connected line is reserved between the two points before the users can start using the service. One issue of debate on circuit switching is the perceived waste of resources during the so-called silent periods when the connection is fully in force but not being used by the parties. This situation occurs when, for example, during a telephone network session, a telephone receiver is not hung up after use, leaving the connection still established. During this period, while no one is utilizing the session, the session line is still open.

### Packet Switching

Packet switching networks, on the other hand, do not require any resources to be reserved before a communication session begins. These networks, however, require the sending host to assemble all data streams to be transmitted into packets. If a message is large, it is broken into several packets. Packet headers contain the source and the destination network addresses of the two communicating end-systems. Then, each of the packets is sent on the communication links and across packet switches (routers). On receipt of each packet, the router inspects the destination address contained in the packet. Using its own routing table, each router then for- wards the packet on the appropriate link at the maximum available bit rate. As each Packet is received at each intermediate router, it is forwarded on the appropriate link interspersed with other packets being forwarded on that link. Each router checks the destination address, if it is the owner of the packet; it then reassembles the packets into the final message. Figure 1.22 shows the role of routers in packet switching networks.

Packet switches are considered to be store-and-forward transmitters, mean- ing that they must receive the entire packet before the packet is retransmitted or switched on to the next switch

Because there is no predefined route for these packets, there can be unpredictably long delays before the full message can be re-assembled. In addition, the network may not dependably deliver all the packets to the intended destination. To ensure that the network has a reliably fast transit time, a fixed maximum length of time is allowed for each packet. Packet switching networks suffer from a few problems, including the following

