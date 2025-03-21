Earlier in this chapter, we indicated that computer networks are basically classi- fied according to their sizes with the local area networks (LANs) covering smaller areas, and the bigger ones covering wider areas (WANs). In this last section of the chapter, let us look at a few network technologies in each one of these categories.

## LAN Technologies

Recall our definition of a LAN at the beginning of this chapter. We defined a LAN to be a small data communication network that consists of a variety of machines that are all part of the network and cover a geographically small area such as one build- ing or one floor. Also, a LAN is usually owned by an individual or a single entity such as an organization. According to IEEE 802.3 Committee on LAN Standard- ization, a LAN must be a moderately sized and geographically shared peer-to-peer communication network broadcasting information for all on the network to hear via a common physical medium on a point-to-point basis with no intermediate switch- ing element required. Many common network technologies today fall into this cat- egory including the popular Ethernet, the widely used token ring/IEEE 805.2, and the fiber distributed data interface (FDDI).

### Star-Based Ethernet (IEEE 802.3) LAN

Ethernet technology is the most widely used of all LAN technologies and it has been standardized by the IEEE 802.3 Committee on Standards. The IEEE 802.3 standards define the medium access control (MAC) layer and the physical layer. The Ethernet MAC is a carrier sense multiple access with collision detection (CSMA/CD) sys- tem. With CSMA, any network node that wants to transmit must listen first to the medium to make sure that there is no other node already transmitting. This is called the carrier sensing of the medium. If there is already a node using the medium, then the element that was intending to transmit waits; otherwise it transmits. In case, two or more elements are trying to transmit at the same time, a collision will occur and the integrity of the data for all is compromised. However, the element may not know this. So it waits for an acknowledgment from the receiving node. The waiting period varies, taking into account maximum round-trip propagation delay and other unexpected delays. If no acknowledgment is received during that time, the element then assumes that a collision has occurred and the transmission was unsuccessful and therefore it must retransmit. If more collisions were to happen, then the element must now double the delay time and so on. After a collision, when the two elements are in delay period, the medium may be idle and this may lead to inefficiency. To correct this situation, the elements, instead of just going into the delay mode, must continue to listen onto the medium as they transmit. In this case, they will not only be doing carrier sensing but also detecting a collision that leads to CSMA/CD. According to Stallings, the CSMA/CD scheme follows the following algorithm.

- If the medium is idle, transmit.
- If the medium busy, continue to listen until idle, then transmit immediately.
- If collision is detected, transmit jamming signal for “collision warning” to all• other network elements.
- After jamming the signal, wait random time units and attempt to transmit
![[Pasted image 20250321113313.png]]
A number of Ethernet LANs are based on the IEEE 802.3 standards, including

- 10 BASE-X (where X = 2, 5, T and F; T = twisted pair and F = fiber optics)
- 100 BASE-T (where the T options include T4, TX, and FX)
- 1000 BASE-T (where T options include LX, SX, T, and CX)

The basic Ethernet transmission structure is a frame and it is shown in Fig. 1.32.

The source and destination fields contain 6-byte LAN addresses of the form xx-xx- xx-xx-xx-xx, where x is a hexadecimal integer. The error detection field is 4 bytes of bits used for error detection, usually using the cyclic redundancy check (CRC) algo- rithm, in which the source and destination elements synchronize the values of these bits.

### Token Ring/IEEE 805.2

Token ring LANs based on IEEE 805.2 are also used widely in commercial and small industrial networks, although not as popular as Ethernet. The standard uses a frame called a token that circulates around the network so that all network nodes have equal access to it. As we have seen previously, token ring technology employs a mechanism that involves passing the token around the network so that all network elements have equal access to it.

Whenever a network element wants to transmit, it waits for the token on the ring to make its way to the element’s connection point on the ring. When the token arrives at this point, the element grabs it and changes one bit of the token that becomes the start bit in the data frame the element will be transmitting. The ele- ment then inserts data, addressing information and other fields and then releases the payload onto the ring. It then waits for the token to make a round and come back. The receiving host must recognize the destination MAC address within the frame as its own. Upon receipt, the host identifies the last field indicating the recognition of the MAC address as its own. The frame contents are then copied by the host, and the frame is put back in circulation. On reaching the network ele- ment that still owns the token, the element withdraws the token and a new to transmit.

Because of its round-robin nature, the token ring technique gives each network element a fair chance of transmitting if it wants to. However, if the token ever gets lost, the network business is halted. Figure 1.33 shows the structure of a token data frame, and Fig. 1.16 shows the token ring structure.

Because of its round-robin nature, the token ring technique gives each network element a fair chance of transmitting if it wants to. However, if the token ever gets lost, the network business is halted. Figure 1.33 shows the structure of a token data frame, and Fig. 1.16 shows the token ring structure.

Like Ethernet, the token ring has a variety of technologies based on the transmission rates
![[Pasted image 20250321113702.png]]
### Other LAN Technologies

In addition to those we have discussed earlier, several other LAN technologies are in use, including the following:

- Asynchronous transfer mode (ATM) with the goal of transporting real-time• voice, video, text, e-mail, and graphic data. ATM offers a full array of network services that make it a rival of the Internet network.
- Fiber distributed data interface (FDDI) is a dual-ring network that uses a token• ring scheme with many similarities to the original token ring technology.
- AppleTalk, the popular Mac users’ LAN.


## WAN Technologies

As we defined it earlier, WANs are data networks like LANs but they cover a wider geographical area. Because of their sizes, WANs traditionally provide fewer services to customers than LANs. Several networks fall into this category, including the inte- grated services digital network (ISDN), X.25, frame relay, and the popular Internet

### integrated Services Digital Network (ISDN)

ISDN is a system of digital phone connections that allows data to be transmitted simultaneously across the world using end-to-end digital connectivity. It is a net- work that supports the transmission of video, voice, and data. Because the trans- mission of these varieties of data, including graphics, usually puts widely differing demands on the communication network, service integration for these networks is an important advantage to make them more appealing. The ISDN standards specify that subscribers must be provided with

- **Basic rate interface (BRI) services of two full-duplex 64-kbps B channels – the bearer channels, and one full-duplex 16-kbps D channel – the data channel. One B channel is used for digital voice and the other for applications such as data transmission. The D channel is used for telemetry and for exchanging network control information. This rate is for individual users.