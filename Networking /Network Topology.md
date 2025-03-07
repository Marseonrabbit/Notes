Computer networks, whether LANs, MANs, or WANs, are constructed based on a topology. The are several topologies including the following popular ones.

---
## Mesh Topology  
---
A mesh topology allows multiple access links between network elements, unlike other types of topologies. The multiplicity of access links between the network elements offers an advantage in network reliability because whenever one network element fails, the network does not cease operations; it simply finds a bypass to the failed element and the network continues to function. Mesh topology is most often applied in MAN networks. Figure 1.11 shows a mesh network.

![[Pasted image 20250227171645.png]]  
*Fig. 1.11: Full mesh topology with redundant paths.*  

---

## Tree Topology  

A more common type of network topology is the tree topology. In the tree topology, network elements are put in a hierarchical structure in which the most predomi- nant element is called the root of the tree and all other elements in the network share a child–parent relationship. As in ordinary, though inverted trees, there are no closed loops. So dealing with failures of network elements presents complications depending on the position of the failed element in the structure. For example, in a deeply rooted tree, if the root element fails, the network automatically ruptures and splits into two parts. The two parts cannot communicate with each other. The func- tioning of the network as a unit is, therefore, fatally curtailed. Figure 1.12 shows a network using a tree topology
![[Pasted image 20250227171719.png]]  
*Fig. 1.12: Tree topology with root-server dependency.*  

---
## Bus Topology  

A more popular topology, especially for LANs, is the bus topology. Elements in a net- work using a bus topology always share a bus and, therefore, have equal access to all LAN resources. Every network element has full-duplex connections to the transmit- ting medium which allows every element on the bus to send and receive data. Because each computing element is directly attached to the transmitting medium, a transmis- sion from any one element propagates through the entire length of the medium in either direction and therefore can be received by all elements in the network. Because of this, precautions need to be taken to make sure that transmissions intended for one element can be received by that element and no other element. The network must also use a mechanism that handles disputes in case two or more elements try to transmit at the same time. The mechanism deals with the likely collision of signals and brings auick recovery from such a collision. It is also necessary to create fairness in the net- work so that all other elements can transmit when they need to do so. See Fig. 1.13. A collision control mechanism must also improve efficiency in the network using a bus topology by allowing only one element in the network to have control of the bus at any one time. This network element is then called the bus master and other elements are considered to be its slaves. This requirement prevents collision from occurring in the network as elements in the network try to seize the bus at the same time. A bus topology is commonly used by LANs.

![[Pasted image 20250227171741.png]]  
*Fig. 1.13: Bus topology with collision domains.*  

---

## Star Topology  

Another very popular topology, especially in LAN network technologies, is a star topol- ogy. A star topology is characterized by a central prominent node that connects to every other element in the network. So, all the elements in the network are connected to a cen- tral element. Every network element in a star topology is connected pairwise in a point- to-point manner through the central element, and communication between any pair of elements must go through this central element. The central element or node can either operate in a broadcast fashion, in which case information from one element is broadcast to all connected elements, or transmit as a switching device in which the incoming data is transmitted only to one element, the nearest element enroute to the destination. The biggest disadvantage to the star topology in networks is that the failure of the central element results in the failure of the entire network. Figure 1.14 shows a star topology.
![[Pasted image 20250227171757.png]]  
*Fig. 1.14: Star topology with central switch.*  

---
## Ring Topology  

- Finally another popular network topology is the ring topology. In this topology, each computing element in a network using a ring topology is directly connected to the transmitting medium via a unidirectional connection so that information put on the transmission medium can reach all computing elements in the network through a mechanism of taking turns in sending information around the ring. Figure 1.15 shows a ring topology network. The taking of turns in passing information is man- aged through a token system. A token is a system-wide piece of information that guarantees the current owner to be the bus master. As long as it owns the token, no other network element is allowed to transmit on the bus. When an element currently sending information and holding the token has finished, it passes the token down- stream to its nearest neighbor. The token system is a good management system of collision and fairness. 
- There are variants of a ring topology collectively called hub hybrids combining either a star with a bus or a stretched star as shown in Fig. 1.16. Although network topologies are important in LANs, the choice of a topology depends on a number of other factors, including the type of transmission medium, reliability of the network, the size of the network, and its anticipated future growth. Recently the most popular LAN topologies have been the bus, star, and ring topolo- gies. The most popular bus- and star-based LAN topology is the Ethernet, and the most popular ring-based LAN topology is the token ring.
![[Pasted image 20250227171814.png]]  
*Fig. 1.15: Unidirectional ring with token circulation.*  
![[Pasted image 20250308022730.png]]