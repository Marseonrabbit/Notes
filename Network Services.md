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