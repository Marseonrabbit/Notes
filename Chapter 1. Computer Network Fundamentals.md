

## 1.1 Introduction

The basic ideas in all types of communication are that there must be three ingredients for the communication to be effective. First, there must be two entities, dubbed a sender and a receiver. These two must have something they need to share. Second, there must be a medium through which the sharable item is channeled. This is the transmission medium. Finally, there must be an agreed-on set of communication rules or protocols. These three apply to every category or structure of communication.

In this chapter, we will focus on these three components in a computer network. But what is a computer network? A computer network is a distributed system consisting of loosely coupled computers and other devices. Any two of these devices, which we will from now on refer to as network elements or transmitting elements without loss of generality, can communicate with each other through a communication medium. In order for these connected devices to be considered a communicating network, there must be a set of communicating rules or protocols each device in the network must follow to communicate with another device in the network. The resulting combination consisting of hardware and software is a computer communication network or computer network in short.

![Computer Network](attachment:computer_network.png)

*Fig. 1.1 A Computer Network*

The hardware component is made of network elements consisting of a collection of nodes that include the end systems commonly called hosts and intermediate switching elements that include hubs, bridges, routers, and gateways that, without loss of generality, we will call network elements.

Network elements may own resources individually, that is locally or globally. Network software consists of all application programs and network protocols that are used to synchronize, coordinate, and bring about the sharing and exchange of data among the network elements. Network software also makes the sharing of expensive resources in the network possible. Network elements, network software, and users all work together so that individual users can exchange messages and share resources on other systems that are not readily available locally. The network elements, together with their resources, may be of diverse hardware technologies and the software may be as different as possible, but the whole combination must work together in unison.

Internetworking technology enables multiple, diverse underlying hardware technologies and different software regimes to interconnect heterogeneous networks and bring them to communicate smoothly. The smooth working of any computer communication network is achieved through the low-level mechanisms provided by the network elements and high-level communication facilities provided by the software running on the communicating elements. Before we discuss the working of these networks, let us first look at the different types of networks.

## 1.2 Computer Network Models

There are several configuration models that form a computer network. The most common of these are the centralized and distributed models. In a centralized model, several computers and devices are interconnected, and can talk to each other. However, there is only one central computer, called the master, through which all correspondence must take place. Dependent computers, called surrogates, may have reduced local resources, such as memory, and sharable global resources are controlled by the master at the center. Unlike the centralized model, however, the distributed network consists of loosely coupled computers interconnected by a communication network consisting of connecting elements and communication channels. The computers themselves may own their resources locally or may request resources from a remote computer. These computers are known by a string of names, including host, client, or node. If a host has resources that other hosts need, then that host is known as a server. Communication and sharing of resources are not controlled by the central computer but are arranged between any two communicating elements in the network.

![Centralized Network Model](attachment:centralized_network.png)

*Fig. 1.2 A Centralized network model*

![Distributed Network Model](attachment:distributed_network.png)

*Fig. 1.3 A Distributed network model*

## 1.3 Computer Network Types

Computer networks come in different sizes. Each network is a cluster of network elements and their resources. The size of the cluster determines the network type. There are, in general, two main network types: the local area network (LAN) and wide area network (WAN).

### 1.3.1 Local Area Networks (LANs)

A computer network with two or more computers or clusters of network and their resources connected by a communication medium sharing communication protocols and confined in a small geographical area, such as a building floor, a building, or a few adjacent buildings, is called a local area network (LAN). The advantage of a LAN is that all network elements are close together so the communication links maintain a higher speed of data movement. Also, because of the proximity of the communicating elements, high-cost and high quality communicating elements can be used to deliver better service and high reliability.

![LAN Network](attachment:lan_network.png)

*Fig. 1.4 A LAN Network*

### 1.3.2 Wide Area Networks (WANs)

A wide area network (WAN), on the other hand, is a network made up of one or more clusters of network elements and their resources but instead of being confined to a small area, the elements of the clusters or the clusters themselves are scattered over a wide geographical area as in a region of a country or across the whole country, several countries, or the entire globe like the Internet for example. Some advantages of a WAN include distributing services to a wider community and availability of a wide array of both hardware and software resources that may not be available in a LAN. However, because of the large geographical areas covered by WANs, communication media are slow and often unreliable.

![WAN Network](attachment:wan_network.png)

*Fig. 1.5 A WAN Network*

### 1.3.3 Metropolitan Area Networks (MANs)

Between the LAN and WAN, there is also a middle network called the metropolitan area network (MAN) because it covers a slightly wider area than the LAN but not so wide as to be considered a WAN. Civic networks that cover a city or part of a city are a good example of a MAN. MANs are rarely talked about because they are quiet often overshadowed by cousin LAN to the left and cousin WAN to the right.

## 1.4 Data Communication Media Technology

The performance of a network type depends greatly on the transmission technology and media used in the network. Let us look at these two.

### 1.4.1 Transmission Technology

The media through which information has to be transmitted determine the signal to be used. Some media permit only analog signals. Some allow both analog and digital. Therefore, depending on the media type involved and other considerations, the input data can be represented as either digital or analog signal. In an analog format, data is sent as continuous electromagnetic waves on an interval representing things such as voice and video and propagated over a variety of media that may include copper wires, twisted coaxial pair or cable, fiber optics, or wireless. We will discuss these media soon. In a digital format, on the other hand, data is sent as a digital signal, a sequence of voltage pulses that can be represented as a stream of binary bits. Both analog and digital data can be propagated and many times represented as either analog or digital.

Transmission itself is the propagation and processing of data signals between network elements. The concept of representation of data for transmission, either as analog or digital signal, is called an encoding scheme. Encoded data is then transmitted over a suitable transmission medium that connects all network elements. There are two encoding schemes, analog and digital. Analog encoding propagates analog signals representing analog data such as sound waves and voice data. Digital encoding, on the other hand, propagates digital signals representing either an analog or a digital signal representing digital data of binary streams by two voltage levels.

Since our interest in this book is in digital networks, we will focus on the encoding of digital data.

#### 1.4.1.1 Analog Encoding of Digital Data

Recall that digital information is in the form of 1s or 0s. To send this information over some analog medium such as the telephone line, for example, which has limited bandwidth, digital data needs to be encoded using modulation and demodulation to produce analog signals. The encoding uses a continuous oscillating wave, usually a sine wave, with a constant frequency signal called a carrier signal. The carrier has three modulation characteristics: amplitude, frequency, and phase shift. The scheme then uses a modem, a modulation-demodulation pair, to modulate and demodulate the data signal based on any one of the three carrier characteristics or a combination. The resulting wave is between a range of frequencies on both sides of the carrier as shown below:

- **Amplitude modulation** represents each binary value by a different amplitude of the carrier frequency. The absence of or low carrier frequency may represent a 0 and any other frequency then represents a 1. But this is a rather inefficient modulation technique and is therefore used only at low frequencies up to 1200 bps in voice grade lines.
- **Frequency modulation** also represents the two binary values by two different frequencies close to the frequency of the underlying carrier. Higher frequencies represent a 1 and low frequencies represent a 0. The scheme is less susceptible to errors.
- **Phase shift modulation** changes the timing of the carrier wave, shifting the carrier phase to encode the data. A 1 is encoded as a change in phase by 180 degrees and a 0 may be encoded as a 0 change in phase of a carrier signal. This is the most efficient scheme of the three and it can reach a transmission rate of up to 9600 bps.

#### 1.4.1.2 Digital Encoding of Digital Data

In this encoding scheme, which offers the most common and easiest way to transmit digital signals, two binary digits are used to represent two different voltages. Within a computer, these voltages are commonly 0 volt and 5 volts. Another procedure uses two representation codes: nonreturn to zero level (NRZ-L), in which negative voltage represents binary one and positive voltage represents binary zero, and nonreturn to zero, invert on ones (NRZ-I).

![NRZ-L Representation Code](attachment:nrz_l.png)

*Fig. 1.6 NRZ-L N Nonreturn to zero level representation code*

![NRZ-I Representation Code](attachment:nrz_i.png)

*Fig. 1.7 NRZI Nonreturn to zero Invert on ones representation code*

One may wonder why go through the hassle of digital encoding and transmission. There are several advantages over its cousin, analog encoding. These include the following:

- Plummeting costs of digital circuitry
- More efficient integration of voice, video, text, and image
- Reduction of noise and other signal impairment because of use of repeaters
- Capacity of channels is utilized best with digital techniques
- Better encryption and hence better security than in analog transmission

#### 1.4.1.3 Multiplexing of Transmission Signals

Quite often during the transmission of data over a network medium, the volume of transmitted data may far exceed the capacity of the medium. Whenever this happens, it may be possible to make multiple signal carriers share a transmission medium. This is referred to as multiplexing. There are two ways in which multiplexing can be achieved: time-division multiplexing (TMD) and frequency-division multiplexing (FDM).

In FDM, all data channels are first converted to analog form. Since a number of signals can be carried on a carrier, each analog signal is then modulated by a separate and different carrier frequency, and this makes it possible to recover during the demultiplexing process. The frequencies are then bundled on the carrier. At the receiving end, the demultiplexer can select the desired carrier signal and use it to extract the data signal for that channel in such a way that the bandwidths do not overlap. FDM has an advantage of supporting full-duplex communication.

TDM, on the other hand, works by dividing the channel into time slots that are allocated to the data streams before they are transmitted. At both ends of the transmission, if the sender and receiver agree on the time-slot assignments, then the receiver can easily recover and reconstruct the original data streams. So multiple digital signals can be carried on one carrier by interleaving portions of each signal in time.

### 1.4.2 Transmission Media

As we have observed above, in any form of communication, there must be a medium through which the communication can take place. So network elements in a network need a medium in order to communicate. No network can function without a transmission medium because there would be no connection between the transmitting elements. The transmission medium plays a vital role in the performance of the network. In total, characteristic quality, dependability, and overall performance of a network depend heavily on its transmission medium. The transmission medium also determines a network's capacity in realizing the expected network traffic, reliability for the network's availability, size of the network in terms of the distance covered, and the transmission rate. Network transmission media can be either wired or wireless.

#### 1.4.2.1 Wired Transmission Media

Wired transmission media are used in fixed networks physically connecting every network element. There are different types of physical media, the most common of which are copper wires, twisted pair, coaxial cables, and optical fibers.

- **Copper wires** have been traditionally used in communication because of their low resistance to electrical currents that allows signals to travel even further. But copper wires suffer interference from electromagnetic energy in the environment, and because of this, they must always be insulated.

- **Twisted pair** is a pair of wires consisting of insulated copper wire each wrapped around the other, forming frequent and numerous twists. Together, the twisted, insulated copper wires act as a full-duplex communication link. The twisting of the wires reduces the sensitivity of the cable to electromagnetic interference and also reduces the radiation of radio frequency noises that may interfere with nearby cables and electronic components. To increase the capacity of the transmitting medium, more than one pair of the twisted wires may be bundled together in a protective coating. Because twisted pairs were far less expensive, easy to install, and had a high quality of voice data, they were widely used in telephone networks. However, because they are poor in upward scalability in transmission rate, distance, and bandwidth in LANs, twisted pair technology has been abandoned in favor of other technologies.

![Twisted Pair](attachment:twisted_pair.png)

*Fig. 1.8 Twisted Pair*

- **Coaxial cables** are dual-conductor cables with a shared inner conductor in the core of the cable protected by an insulation layer and the outer conductor surrounding the insulation. These cables are called coaxial because they share the inner conductor. The inner core conductor is usually made of solid copper wire, but at times can also be made up of stranded wire. The outer conductor commonly made of braided wires, but sometimes made of metallic foil or both, forms a protective tube around the inner conductor. This outer conductor is also further protected by another outer coating called the sheath. Coaxial cables are commonly used in television transmissions. Unlike twisted pairs, coaxial cables can be used over long distances. There are two types of coaxial cables: thinnet, a light and flexible cabling medium that is inexpensive and easy to install; and the thickent, which is thicker and harder to break and can carry more signals through a longer distance than thinnet.

![Coaxial Cable](attachment:coaxial_cable.png)

*Fig. 1.9 Coaxial Cable*

- **Optical fiber** is a small medium made up of glass and plastics and conducts an optical ray. This is the most ideal cable for data transmission because it can accommodate extremely high bandwidths and has few problems with electromagnetic interference that coaxial cables suffer from. It can also support cabling for several kilometers. The two disadvantages of fiber-optic cables, however, are cost and installation difficulty. As shown in Fig. 1.10, a simple optical fiber has a central core made up of thin fibers of glass or plastics. The fibers are protected by a glass or plastic coating called a cladding. The cladding, though made up of the same materials as the core, has different properties that give it the capacity to reflect back the core rays that tangentially hit on it. The cladding itself is encased in a plastic jacket. The jacket protects the inner fiber from external abuses such as bending and abrasions. Optical fiber cables transmit data signals by first converting them into light signals. The transmitted light is emitted at the source from either a light emitting diode (LED) or an injection laser diode (ILD). At the receiving end, the emitted rays are received by a photo detector that converts them back to the original form.

![Optical Fiber](attachment:optical_fiber.png)

*Fig. 1.10 Optical Fiber*

#### 1.4.2.2 Wireless Communication

Wireless communication and wireless networks have evolved as a result of rapid development in communication technologies, computing, and people's need for mobility. Wireless networks fall in one of the following three categories depending on distance as follows:

- **Restricted Proximity Network**: This network involves local area networks (LANs) with a mixture of fixed and wireless devices.
- **Intermediate/Extended Network**: This wireless network is actually made up of two fixed LAN components joined together by a wireless component. The bridge may be connecting LANs in two nearby buildings or even further.
- **Mobile Network**: This is a fully wireless network connecting two network elements. One of these elements is usually a mobile unit that connects to the home network (fixed) using cellular or satellite technology.

These three types of wireless networks are connected using basic media such as infrared, laser beam, narrow-band and spread-spectrum radio, microwave, and satellite communication.

- **Infrared**: During an infrared transmission, one network element remotely emits and transmits pulses of infrared light that carry coded instructions to the receiving network element. As long as there is no object to stop the transmitted light, the receiver gets the instruction. Infrared is best used effectively in a small confined area, within 100 feet, for example, a television remote communicating with the television set. In a confined area such as this, infrared is relatively fast and can support high bandwidths of up to 10 Mbps.

- **High-Frequency Radio**: During a radio communication, high-frequency electromagnetic radio waves or radio frequency commonly referred to as RF transmissions are generated by the transmitter and are picked up by the receiver. Because the range of radio frequency band is greater than that of infrared, mobile computing elements can communicate over a limited area without both transmitter and receiver being placed along a direct line of sight; the signal can bounce off light walls, buildings, and atmospheric objects. RF transmissions are very good for long distances when combined with satellites to refract the radio waves.

- **Microwave**: Microwaves are a higher-frequency version of radio waves but whose transmissions, unlike those of the radio, can be focused in a single direction. Microwave transmissions use a pair of parabolic antennas that produce and receive narrow, but highly directional signals. To be sensitive to signals, both the transmitting and receiving antennas must focus within a narrow area. Because of this, both the transmitting and receiving antennas must be carefully adjusted to align the transmitted signal to the receiver. Microwave communication has two forms: terrestrial, when it is near ground, and satellite microwave. The frequencies and technologies employed by these two forms are similar but with notably distinct differences.

- **Laser**: Laser light can be used to carry data for several thousand yards through air and optical fibers. But this is possible only if there are no obstacles in the line of sight. Lasers can be used in many of the same situations as microwaves, and like microwaves, laser beams must be refracted when used over long distances.

## 1.5 Network Topology

Computer networks, whether LANs, MANs, or WANs, are constructed based on a topology. The are several topologies including the following popular ones.

### 1.5.1 Mesh

A mesh topology allows multiple access links between network elements, unlike other types of topologies. The multiplicity of access links between the network elements offers an advantage in network reliability because whenever one network element fails, the network does not cease operations; it simply finds a bypass to the failed element and the network continues to function. Mesh topology is most often applied in MAN networks.

![Mesh Network](attachment:mesh_network.png)

*Fig. 1.11 Mesh Network*

### 1.5.2 Tree

A more common type of network topology is the tree topology. In the tree topology, network elements are put in a hierarchical structure in which the most predominant element is called the root of the tree and all other elements in the network share a child-parent relationship. As in ordinary, though inverted trees, there are no closed loops. So dealing with failures of network elements presents complications depending on the position of the failed element in the structure. For example, in a deeply rooted tree, if the root element fails, the network automatically ruptures and splits into two parts. The two parts cannot communicate with each other. The functioning of the network as a unit is, therefore, fatally curtailed.

![Tree Topology](attachment:tree_topology.png)

*Fig. 1.12 Tree Topology*

### 1.5.3 Bus

A more popular topology, especially for LANs, is the bus topology. Elements in a network using a bus topology always share a bus and, therefore, have equal access to all LAN resources. Every network element has full-duplex connections to the transmitting medium which allows every element on the bus to send and receive data. Because each computing element is directly attached to the transmitting medium, a transmission from any one element propagates through the entire length of the medium in either direction and therefore can be received by all elements in the network. Because of this, precautions need to be taken to make sure that transmissions intended for one element can be received by that element and no other element. The network must also use a mechanism that handles disputes in case two or more elements try to transmit at the same time. The mechanism deals with the likely collision of signals and brings a quick recovery from such a collision. It is also necessary to create fairness in the network so that all other elements can transmit when they need to do so.

![Bus Topology](attachment:bus_topology.png)

*Fig. 1.13 Bus topology*

A collision control mechanism must also improve efficiency in the network using a bus topology by allowing only one element in the network to have control of the bus at any one time. This network element is then called the bus master and other elements are considered to be its slaves. This requirement prevents collision from occurring in the network as elements in the network try to seize the bus at the same time. A bus topology is commonly used by LANs.

### 1.5.4 Star

Another very popular topology, especially in LAN network technologies, is a star topology. A star topology is characterized by a central prominent node that connects to every other element in the network. So, all the elements in the network are connected to a central element. Every network element in a star topology is connected pairwise in a point-to-point manner through the central element, and communication between any pair of elements must go through this central element. The central element or node can either operate in a broadcast fashion, in which case information from one element is broadcast to all connected elements, or transmit as a switching device in which the incoming data is transmitted only to one element, the nearest element enroute to the destination. The biggest disadvantage to the star topology in networks is that the failure of the central element results in the failure of the entire network.

![Star Topology](attachment:star_topology.png)

*Fig. 1.14 Star topology*

### 1.5.5 Ring

Finally another popular network topology is the ring topology. In this topology, each computing element in a network using a ring topology is directly connected to the transmitting medium via a unidirectional connection so that information put on the transmission medium can reach all computing elements in the network through a mechanism of taking turns in sending information around the ring.

![Ring Topology](attachment:ring_topology.png)

*Fig. 1.15 Ring topology network*

The taking of turns in passing information is managed through a token system. A token is a system-wide piece of information that guarantees the current owner to be the bus master. As long as it owns the token, no other network element is allowed to transmit on the bus. When an element currently sending information and holding the token has finished, it passes the token downstream to its nearest neighbor. The token system is a good management system of collision and fairness.

There are variants of a ring topology collectively called hub hybrids combining either a star with a bus or a stretched star as shown in Fig. 1.16.

![Token Ring Hub](attachment:token_ring_hub.png)

*Fig. 1.16 Token ring hub*

Although network topologies are important in LANs, the choice of a topology depends on a number of other factors, including the type of transmission medium, reliability of the network, the size of the network, and its anticipated future growth. Recently the most popular LAN topologies have been the bus, star, and ring topologies. The most popular bus- and star-based LAN topology is the Ethernet, and the most popular ring-based LAN topology is the token ring.

## 1.6 Network Connectivity and Protocols

In the early days of computing, computers were used as stand-alone machines, and all work that needed cross-computing was done manually. Files were moved on disks from computer to computer. There was, therefore, a need for cross-computing where more than one computer should talk to others and vice versa.

A new movement was, therefore, born. It was called the open system movement, which called for computer hardware and software manufacturers to come up with a way for this to happen. But to make this possible, standardization of equipment and software was needed. To help in this effort and streamline computer communication, the International Standards Organization (ISO) developed the Open System Interconnection (OSI) model. The OSI is an open architecture model that functions as the network communication protocol standard, although it is not the most widely used one. The Transport Control Protocol/Internet Protocol (TCP/IP) model, a rival model to OSI, is the most widely used. Both OSI and TCP/IP models use two protocol stacks, one at the source element and the other at the destination element.

### 1.6.1 Open System Interconnection (OSI) Protocol Suite

The development of the OSI model was based on the secure premise that a communication task over a network can be broken into seven layers, where each layer represents a different portion of the task. Different layers of the protocol provide different services and ensure that each layer can communicate only with its own neighboring layers. That is, the protocols in each layer are based on the protocols of the previous layers.

Starting from the top of the protocol stack, tasks and information move down from the top layers until they reach the bottom layer where they are sent out over the network media from the source system to the destination. At the destination, the task or information rises back up through the layers until it reaches the top. Each layer is designed to accept work from the layer above it and to pass work down to the layer below it, and vice versa. To ease interlayer communication, the interfaces between the layers are standardized. However, each layer remains independent and can be designed independently and each layer's functionality should not affect the functionalities of other layers above and below it.

![ISO Logical Peer Communication Model](attachment:iso_logical_peer_communication.png)

*Fig. 1.17 ISO logical peer communication model*

Table 1.1 shows an OSI model consisting of seven layers and the descriptions of the services provided in each layer.

| Layer Number | Protocol |
| :-- | :-- |
| 7 | Application |
| 6 | Presentation |
| 5 | Session |
| 4 | Transport |
| 3 | Network |
| 2 | Data Link |
| 1 | Physical |

*Table 1.1 ISO protocol layers and corresponding services*

In peer-to-peer communication, the two communicating computers can initiate and receive tasks and data. The task and data initiated from each computer starts from the top in the application layer of the protocol stack on each computer. The tasks and data then move down from the top layers until they reach the bottom layer, where they are sent out over the network media from the source system to the destination. At the destination, the task and data rise back up through the layers until the top. Each layer is designed to accept work from the layer above it and pass work down to the layer below it. As data passes from layer to layer of the sender machine, layer headers are appended to the data, causing the datagram to grow larger. Each layer header contains information for that layer's peer on the remote system. That information may indicate how to route the packet through the network or what should be done to the packet as it is handed back up the layers on the recipient computer.

Table 1.2 shows the datagram with added header information as it moves through the layers.

| No header | Data | Application |
| :-- | :-- | :-- |
| H1 | Data | Presentation |
| H2 | Data | Session |
| H3 | Data | Transport |
| H4 | Data | Network |
| H5 | Data | Data Link |
| No header | Data | Physical |

*Table 1.2 OSI datagrams seen in each layer with header added*

Although the development of the OSI model was intended to offer a standard for all other proprietary models, and it was as encompassing of all existing models as possible, it never really replaced many of those rival models it was intended to replace. In fact it is this "all in one" concept that led to market failure because it became too complex. Its late arrival on the market also prevented its much anticipated interoperability across networks.

### 1.6.2 Transport Control Protocol/Internet Protocol (TCP/IP) Model

Among the OSI rivals was the TCP/IP, which was far less complex and more historically established by the time the OSI came on the market. The TCP/IP model does not exactly match the OSI model. For example, it has two to three fewer levels than the seven layers of the OSI model. It was developed for the US Department of Defense Advanced Research Project Agency (DARPA); but over the years, it has seen a phenomenal growth in popularity and it is now the de facto standard for the Internet and many intranets. It consists of two major protocols: the transmission control protocol (TCP) and the Internet protocol (IP), hence the TCP/IP designation. Table 1.3 shows the layers and protocols in each layer.

| Layer | Delivery Unit | Protocols |
| :--: | :--: | :--: |
| Application | Message | - Handles all higher level protocols including File Transfer Protocol (FTP), Name Server Protocol (NSP), Simple Mail Transfer Protocol (SMTP), Simple Network Management Protocol (SNMP), HTTP, Remote file access (telnet), Remote file server (NFS), Name Resolution (DNS), HTTP,- TFTP, SNMP, DHCP, DNS, BOOTP <br> - Combines Application, Session and Presentation Layers of the OSI model. <br> - Handles all high-level protocols |
| Transport | Segment | - Handles transport protocols including Transmission Control Protocol (TCP), User Datagram Protocol (UDP). |
| Network | Datagram | - Contains the following protocols: Internet Protocol (IP), Internet Control Message Protocol (ICMP), Internet Group Management Protocol (IGMP). <br> - Supports transmitting source packets from any network on the internetwork and makes sure they arrive at the destination independent of the path and networks they took to reach there. <br> - Best path determination and packet switching occur at this layer. |
| Data Link | Frame | Contains protocols that require IP packet to cross a physical link from one device to another directly connected device. <br> - It included the following networks: <br> - WAN - Wide Area Network <br> - LAN - Local Area Network |
| Physical | Bit stream | All network card drivers. |

*Table 1.3 TCP/IP protocol layers*

Since TCP/IP is the most widely used in most network protocol suites by the Internet and many intranets, let us focus on its layers here.

#### 1.6.2.1 Application Layer

This layer, very similar to the application layer in the OSI model, provides the user interface with resources rich in application functions. It supports all network applications and includes many protocols on a data structure consisting of bit streams as shown in Fig. 1.18.

![Application Layer Data Frame](attachment:application_layer_data_frame.png)

*Fig. 1.18 Application layer data frame*

#### 1.6.2.2 Transport Layer

This layer, again similar to the OSI model session layer, is a slightly removed from the user and is hidden from the user. Its main purpose is to transport application layer messages that include application layer protocols in their headers between the host and the server. For the Internet network, the transport layer has two standard protocols: transport control protocol (TCP) and user datagram protocol (UDP). TCP provides a connection-oriented service, and it guarantees the delivery of all application layer packets to their destination. This guarantee is based on two mechanisms: congestion control that throttles the transmission rate of the source element when there is traffic congestion in the network and the flow control mechanism that tries to match sender and receiver speeds to synchronize the flow rate and reduce the packet drop rate. While TCP offers guarantees of delivery of the application layer packets, UDP, on the other hand, offers no such guarantees. It provides a nofrills connectionless service with just delivery and no acknowledgements. But it is much more efficient and a protocol of choice for real-time data such as streaming video and music. Transport layer delivers transport layer packets and protocols to the network layer. Figure 1.19 shows the TCP data structure, and Fig. 1.20 shows the UDP data structure.

![TCP Data Structure](attachment:tcp_data_structure.png)

*Fig. 1.19 A T
