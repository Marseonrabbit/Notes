
# A Guide to Computer Network Security

## Joseph Migga Kizza

---

# Computer Communications and Networks

The Computer Communications and Networks series is a range of textbooks, monographs, and handbooks. It sets out to provide students, researchers, and nonspecialists alike with a sure grounding in current knowledge, together with comprehensible access to the latest developments in computer communications and networking. Emphasis is placed on clear and explanatory styles that support a tutorial approach so that even the most complex of topics is presented in a lucid and intelligible manner.

For other titles published in this series, go to [Springer](http://www.springer.com/).

---

# Joseph Migga Kizza

## A Guide to Computer Network Security

**Springer**

**Joseph Migga Kizza, PhD**
University of Tennessee-Chattanooga
Department of Computer Science
615 McCallie Ave.
Chattanooga, TN 37403
326 Grote Hall
USA
[joseph-kizza@utc.edu](mailto:joseph-kizza@utc.edu)

**Series Editor**
Professor A.J. Sammes, BSc, MPhil, PhD, FBCS, CEng
CISM Group, Cranfield University,
RMCS, Shrivenham, Swindon SN6 8LA, UK

**CCN Series ISSN** 1617-7975
**ISBN** 978-1-84800-916-5
**e-ISBN** 978-1-84800-917-2
**DOI** [10.1007/978-1-84800-917-2](https://doi.org/10.1007/978-1-84800-917-2)
**Library of Congress Control Number:** 2008942999

© Springer-Verlag London Limited 2009

All rights reserved. This work may not be translated or copied in whole or in part without the written permission of the publisher (Springer Science + Business Media, LLC, 233 Spring Street, New York, NY 10013, USA), except for brief excerpts in connection with reviews or scholarly analysis. Use in connection with any form of information storage and retrieval, electronic adaptation, computer software, or by similar or dissimilar methodology now known or hereafter developed is forbidden.

The use in this publication of trade names, trademarks, service marks, and similar terms, even if they are not identified as such, is not to be taken as an expression of opinion as to whether or not they are subject to proprietary rights.

Printed on acid-free paper
[springer.com](http://www.springer.com)

To the Trio: Immaculate, Josephine, and Florence

---

# Preface

If we are to believe in Moore's law, then every passing day brings new and advanced changes to the technology arena. We are as amazed by the miniaturization of computing devices as we are amused by their speed of computation. Everything seems to be in flux and moving fast. We are also fast moving towards ubiquitous computing. To achieve this kind of computing landscape, new ease and seamless computing user interfaces have to be developed. Believe me, if you mature and have ever programmed any digital device, you are, like me, looking forward to this brave new computing landscape with anticipation.

However, if history is any guide to us, we in information security, and indeed every computing device user young and old, must brace ourselves for a future full of problems. As we enter into this world of fast, small, and concealable ubiquitous computing devices, we are entering fertile territory for dubious, mischievous, and malicious people. We need to be on guard because, as expected, help will be slow coming because first, well-trained and experienced personnel will still be difficult to get and those that will be found will likely be very expensive as the case is today. Secondly, the security protocols and best practices will, as it is today, keep changing at a first rate which may warrant network administrators to constantly changing them. Thirdly, as the case is today, it will be extremely difficult to keep abreast of the many new vulnerabilities and patches to them. In other words, the computing landscape will change for sure on one side and remain the same on the other.

For these reasons, we need to remain vigilant with better, if not advanced computer and information security protocols and best practices because the frequency of computer network attacks and the vulnerability of computer network systems will likely not abet, rather they are likely to increase as before.

More efforts in developing adaptive and scalable security protocols and best practices and massive awareness, therefore, are needed to meet this growing challenge and bring the public to a level where they can be active and safe participants in the brave new worlds of computing.

This guide is a comprehensive volume touching not only on every major topic in computing and information security and assurance but it also introduces new computing technologies like wireless sensor networks, a wave of the future, where security is likely to be a major issue. It is intended to bring massive education and awareness of security issues and concerns in cyberspace in general and the computing world in particular, their benefits to society, the security problems and the dangers likely to be encountered by the users, and be a pathfinder as it initiates a dialog towards developing better algorithms, protocols, and best practices that will enhance security of computing systems in the anticipated brave new world. It does this comprehensively in four parts and twenty-two chapters. Part I gives the reader an understanding of the working of and the security situation of computer networks. Part II builds on this knowledge and exposes the reader to the prevailing security situation based on a constant security threat. It surveys several security threats. Part III, the largest, forms the core of the guide and presents to the reader most of the best practices and solutions that are currently in use. Part IV is for projects. In addition to the algorithms, protocols, and solutions, several products and services are given for each security item under discussion.

In summary, the guide attempts to achieve the following objectives:
1. Educate the public about cyberspace security in general terms and computer systems security in particular, with reference to the Internet.
2. Alert the public to the magnitude of computer network vulnerabilities, weaknesses, and loopholes inherent in the computer network infrastructure.
3. Bring to the public attention effective security solutions and best practices, expert opinions on those solutions, and the possibility of ad-hoc solutions.
4. Look at the roles legislation, regulation, and enforcement play in computer network security efforts.
5. Finally, initiate a debate on developing effective and comprehensive algorithms, protocols, and best practices for information security.

Since the guide covers a wide variety of security topics, algorithms, solutions, and best practices, it is intended to be both a teaching and a reference tool for all interested in learning about computer network security issues and available techniques to prevent information systems attacks. The depth and thorough discussion and analysis of most of the computer network security issues, together with the discussion of security algorithms, and solutions given, makes the guide a unique reference source of ideas for computer network security personnel, network security policy makers, and those reading for leisure. In addition, the guide provokes the reader by raising valid legislative, legal, social, and ethical security issues, including the increasingly diminishing line between individual privacy and the need for collective and individual security.

The guide targets college students in computer science, information science, technology studies, library sciences, engineering, and to a lesser extent students in the arts and sciences who are interested in information technology. In addition, students in information management sciences will find the guide particularly helpful. Practitioners, especially those working in information-intensive areas, will likewise find the guide a good reference source. It will also be valuable to those interested in any aspect of information security and assurance and those simply wanting to become cyberspace literates.

---

# Book Resources

There are two types of exercises at the end of each chapter: easy and quickly workable exercises whose responses can be easily spotted from the preceding text; and more thought-provoking advanced exercises whose responses may require research outside the content of this book. Also, Chapter 22 is devoted to lab exercises. There are three types of lab exercises: weekly or bi-weekly assignments that can be done easily with either reading or using readily available software and hardware tools; slightly harder semester-long projects that may require extensive time, collaboration, and some research to finish them successfully; and hard open research projects that require a lot of thinking, take a lot of time, and require extensive research.

We have tried as much as possible, throughout the guide, to use open-source software tools. This has two consequences to it: one, it makes the guide affordable keeping in mind the escalating proprietary software prices; and two, it makes the content and related software tools last longer because the content and corresponding exercises and labs are not based on one particular proprietary software tool that can go out anytime.

---

## Instructor Support Materials

As you consider using this book, you may need to know that we have developed materials to help you with your course. The help materials for both instructors and students cover the following areas:

- **Syllabus:** There is a suggested syllabus for the instructor.
- **Instructor PowerPoint slides:** These are detailed enough to help the instructor, especially those teaching the course for the first time.
- **Answers to selected exercises at the end of each chapter.**
- **Laboratory:** Since network security is a hands-on course, students need to spend a considerable amount of time on scheduled laboratory exercises. The last chapter of the book contains several laboratory exercises and projects. The book resource center contains several more and updates.
- **Instructor manual:** These will guide the instructor in the day-to-day job of getting materials ready for the class.
- **Student laboratory materials:** Under this section, we will be continuously posting the latest laboratory exercises, software, and challenge projects.

These materials can be found at the publisher's website at [Springer Online](http://www.springeronline.com) and at the author's site at [UTC Faculty](http://www.utc.edu/Faculty/Joseph-Kizza/).

Chattanooga, Tennessee, USA
Joseph Migga Kizza
October, 2008.

---

# Contents

## Part I: Understanding Computer Network Security

1. [Computer Network Fundamentals](#chapter-1)
2. [Understanding Computer Network Security](#chapter-2)

## Part II: Security Challenges to Computer Networks

1. [Security Threats to Computer Networks](#chapter-3)
2. [Computer Network Vulnerabilities](#chapter-4)
3. [Cyber Crimes and Hackers](#chapter-5)
4. [Hostile Scripts](#chapter-6)
5. [Security Assessment, Analysis, and Assurance](#chapter-7)

## Part III: Dealing with Network Security Challenges

1. [Disaster Management](#chapter-8)
2. [Access Control and Authorization](#chapter-9)
3. [Authentication](#chapter-10)
4. [Cryptography](#chapter-11)
5. [Firewalls](#chapter-12)
6. [System Intrusion Detection and Prevention](#chapter-13)
7. [Computer and Network Forensics](#chapter-14)
8. [Virus and Content Filtering](#chapter-15)
9. [Standardization and Security Criteria: Security Evaluation of Computer Products](#chapter-16)
10. [Computer Network Security Protocols](#chapter-17)
11. [Security in Wireless Networks and Devices](#chapter-18)
12. [Security in Sensor Networks](#chapter-19)
13. [Other Efforts to Secure Information and Computer Networks](#chapter-20)

## Part IV: Projects

1. [Security Beyond Computer Networks: Information Assurance](#chapter-21)
2. [Projects](#chapter-22)

---

# Chapter 1: Computer Network Fundamentals

## 1.1 Introduction

The basic ideas in all types of communication are that there must be three ingredients for the communication to be effective. First, there must be two entities, dubbed a sender and a receiver. These two must have something they need to share. Second, there must be a medium through which the sharable item is channeled. This is the transmission medium. Finally, there must be an agreed-on set of communication rules or protocols. These three apply to every category or structure of communication.

In this chapter, we will focus on these three components in a computer network. But what is a computer network? A computer network is a distributed system consisting of loosely coupled computers and other devices. Any two of these devices, which we will from now on refer to as network elements or transmitting elements without loss of generality, can communicate with each other through a communication medium. In order for these connected devices to be considered a communicating network, there must be a set of communicating rules or protocols each device in the network must follow to communicate with another device in the network. The resulting combination consisting of hardware and software is a computer communication network or computer network in short.

![Computer Network](attachment:computer_network.png)

*Fig. 1.1 A Computer Network*

The hardware component is made of network elements consisting of a collection of nodes that include the end systems commonly called hosts and intermediate switching elements that include hubs, bridges, routers, and gateways that, without loss of generality, we will call network elements.

Network elements may own resources individually, that is locally or globally. Network software consists of all application programs and network protocols that are used to synchronize, coordinate, and bring about the sharing and exchange of data among the network elements. Network software also makes the sharing of expensive resources in the network possible. Network elements, network software, and users all work together so that individual users can exchange messages and share resources on other systems that are not readily available locally. The network elements, together with their resources, may be of diverse hardware technologies and the software may be as different as possible, but the whole combination must work together in unison.

Internetworking technology enables multiple, diverse underlying hardware technologies and different software regimes to interconnect heterogeneous networks and bring them to communicate smoothly. The smooth working of any computer communication network is achieved through the low-level mechanisms provided by the network elements and high-level communication facilities provided by the software running on the communicating elements. Before we discuss the working of these networks, let us first look at the different types of networks.

---

## 1.2 Computer Network Models

There are several configuration models that form a computer network. The most common of these are the centralized and distributed models. In a centralized model, several computers and devices are interconnected, and can talk to each other. However, there is only one central computer, called the master, through which all correspondence must take place. Dependent computers, called surrogates, may have reduced local resources, such as memory, and sharable global resources are controlled by the master at the center. Unlike the centralized model, however, the distributed network consists of loosely coupled computers interconnected by a communication network consisting of connecting elements and communication channels. The computers themselves may own their resources locally or may request resources from a remote computer. These computers are known by a string of names, including host, client, or node. If a host has resources that other hosts need, then that host is known as a server. Communication and sharing of resources are not controlled by the central computer but are arranged between any two communicating elements in the network.

![Centralized Network Model](attachment:centralized_network.png)

*Fig. 1.2 A Centralized Network Model*

![Distributed Network Model](attachment:distributed_network.png)

*Fig. 1.3 A Distributed Network Model*

---

## 1.3 Computer Network Types

Computer networks come in different sizes. Each network is a cluster of network elements and their resources. The size of the cluster determines the network type. There are, in general, two main network types: the local area network (LAN) and wide area network (WAN).

### 1.3.1 Local Area Networks (LANs)

A computer network with two or more computers or clusters of networks and their resources connected by a communication medium sharing communication protocols and confined in a small geographical area, such as a building floor, a building, or a few adjacent buildings, is called a local area network (LAN). The advantage of a LAN is that all network elements are close together so the communication links maintain a higher speed of data movement. Also, because of the proximity of the communicating elements, high-cost and high-quality communicating elements can be used to deliver better service and high reliability.

![LAN Network](attachment:lan_network.png)

*Fig. 1.4 A LAN Network*

### 1.3.2 Wide Area Networks (WANs)

A wide area network (WAN), on the other hand, is a network made up of one or more clusters of network elements and their resources but instead of being confined to a small area, the elements of the clusters or the clusters themselves are scattered over a wide geographical area as in a region of a country or across the whole country, several countries, or the entire globe like the Internet for example. Some advantages of a WAN include distributing services to a wider community and availability of a wide array of both hardware and software resources that may not be available in a LAN. However, because of the large geographical areas covered by WANs, communication media are slow and often unreliable.

![WAN Network](attachment:wan_network.png)

*Fig. 1.5 A WAN Network*

### 1.3.3 Metropolitan Area Networks (MANs)

Between the LAN and WAN, there is also a middle network called the metropolitan area network (MAN) because it covers a slightly wider area than the LAN but not so wide as to be considered a WAN. Civic networks that cover a city or part of a city are a good example of a MAN. MANs are rarely talked about because they are quite often overshadowed by cousin LAN to the left and cousin WAN to the right.

---

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

*Fig. 1.6 NRZ-L Nonreturn to Zero Level Representation Code*

![NRZ-I Representation Code](attachment:nrz_i.png)

*Fig. 1.7 NRZI Nonreturn to Zero Invert on Ones Representation Code*

In NRZ-L, whenever a 1 occurs, a transition from one voltage level to another is used to signal the information. One problem with NRZ signaling techniques is the requirement of a perfect synchronization between the receiver and transmitter clocks. This is, however, reduced by sending a separate clock signal. There are yet other representations such as the Manchester and differential Manchester, which encode clock information along with the data.

One may wonder why go through the hassle of digital encoding and transmission. There are several advantages over its cousin, analog encoding. These include the following:

- Plummeting costs of digital circuitry
- More efficient integration of voice, video, text, and image
- Reduction of noise and other signal impairment because of use of repeaters
- Capacity of channels is utilized best with digital techniques
- Better encryption and hence better security than in analog transmission

#### 1.4.1.3 Multiplexing of Transmission Signals

Quite often during the transmission of data over a network medium, the volume of transmitted data may far exceed the capacity of the medium. Whenever this happens, it may be possible to make multiple signal carriers share a transmission medium. This is referred to as multiplexing. There are two ways in which multiplexing can be achieved: time-division multiplexing (TDM) and frequency-division multiplexing (FDM).

In FDM, all data channels are first converted to analog form. Since a number of signals can be carried on a carrier, each analog signal is then modulated by a separate and different carrier frequency, and this makes it possible to recover during the demultiplexing process. The frequencies are then bundled on the carrier. At the receiving end, the demultiplexer can select the desired carrier signal and use it to extract the data signal for that channel in such a way that the bandwidths do not overlap. FDM has an advantage of supporting full-duplex communication.

TDM, on the other hand, works by dividing the channel into time slots that are allocated to the data streams before they are transmitted. At both ends of the transmission, if the sender and receiver agree on the time-slot assignments, then the receiver can easily recover and reconstruct the original data streams. So multiple digital signals can be carried on one carrier by interleaving portions of each signal in time.

### 1.4.2 Transmission Media

As we have observed above, in any form of communication, there must be a medium through which the communication can take place. So network elements in a network need a medium in order to communicate. No network can function without a transmission medium because there would be no connection between the transmitting elements. The transmission medium plays a vital role in the performance of the network. In total, characteristic quality, dependability, and overall performance of a network depend heavily on its transmission medium. The transmission medium also determines a network's capacity in realizing the expected network traffic, reliability for the network's availability, size of the network in terms of the distance covered, and the transmission rate. Network transmission media can be either wired or wireless.

#### 1.4.2.1 Wired Transmission Media

Wired transmission media are used in fixed networks physically connecting every network element. There are different types of physical media, the most common of which are copper wires, twisted pair, coaxial cables, and optical fibers.

**Copper wires** have been traditionally used in communication because of their low resistance to electrical currents that allows signals to travel even further. But copper wires suffer interference from electromagnetic energy in the environment, and because of this, they must always be insulated.

**Twisted pair** is a pair of wires consisting of insulated copper wire each wrapped around the other, forming frequent and numerous twists. Together, the twisted, insulated copper wires act as a full-duplex communication link. The twisting of the wires reduces the sensitivity of the cable to electromagnetic interference and also reduces the radiation of radio frequency noises that may interfere with nearby cables and electronic components. To increase the capacity of the transmitting medium, more than one pair of the twisted wires may be bundled together in a protective coating. Because twisted pairs were far less expensive, easy to install, and had a high quality of voice data, they were widely used in telephone networks. However, because they are poor in upward scalability in transmission rate, distance, and bandwidth in LANs, twisted pair technology has been abandoned in favor of other technologies.

![Twisted Pair](attachment:twisted_pair.png)

*Fig. 1.8 Twisted Pair*

**Coaxial cables** are dual-conductor cables with a shared inner conductor in the core of the cable protected by an insulation layer and the outer conductor surrounding the insulation. These cables are called coaxial because they share the inner conductor. The inner core conductor is usually made of solid copper wire, but at times can also be made up of stranded wire. The outer conductor commonly made of braided wires, but sometimes made of metallic foil or both, forms a protective tube around the inner conductor. This outer conductor is also further protected by another outer coating called the sheath.

![Coaxial Cable](attachment:coaxial_cable.png)

*Fig. 1.9 Coaxial Cable*

Coaxial cables are commonly used in television transmissions. Unlike twisted pairs, coaxial cables can be used over long distances. There are two types of coaxial cables: thinnet, a light and flexible cabling medium that is inexpensive and easy to install; and the thicknet, which is thicker and harder to break and can carry more signals through a longer distance than thinnet.

**Optical fiber** is a small medium made up of glass and plastics and conducts an optical ray. This is the most ideal cable for data transmission because it can accommodate extremely high bandwidths and has few problems with electromagnetic interference that coaxial cables suffer from. It can also support cabling for several kilometers. The two disadvantages of fiber-optic cables, however, are cost and installation difficulty. As shown in Fig. 1.10, a simple optical fiber has a central core made up of thin fibers of glass or plastics. The fibers are protected by a glass or plastic coating called a cladding. The cladding, though made up of the same materials as the core, has different properties that give it the capacity to reflect back the core rays that tangentially hit on it. The cladding itself is encased in a plastic jacket. The jacket protects the inner fiber from external abuses such as bending and abrasions. Optical fiber cables transmit data signals by first converting them into light signals. The transmitted light is emitted at the source from either a light-emitting diode (LED) or an injection laser diode (ILD). At the receiving end, the emitted rays are received by a photo detector that converts them back to the original form.

![Optical Fiber](attachment:optical_fiber.png)

*Fig. 1.10 Optical Fiber*

#### 1.4.2.2 Wireless Communication

Wireless communication and wireless networks have evolved as a result of rapid development in communication technologies, computing, and people's need for mobility. Wireless networks fall in one of the following three categories depending on distance as follows:

- **Restricted Proximity Network:** This network involves local area networks (LANs) with a mixture of fixed and wireless devices.
- **Intermediate/Extended Network:** This wireless network is actually made up of two fixed LAN components joined together by a wireless component. The bridge may be connecting LANs in two nearby buildings or even further.
- **Mobile Network:** This is a fully wireless network connecting two network elements. One of these elements is usually a mobile unit that connects to the home network (fixed) using cellular or satellite technology.

These three types of wireless networks are connected using basic media such as infrared, laser beam, narrow-band and spread-spectrum radio, microwave, and satellite communication.

**Infrared:** During an infrared transmission, one network element remotely emits and transmits pulses of infrared light that carry coded instructions to the receiving network element. As long as there is no object to stop the transmitted light, the receiver gets the instruction. Infrared is best used effectively in a small confined area, within 100 feet, for example, a television remote communicating with the television set. In a confined area such as this, infrared is relatively fast and can support high bandwidths of up to 10 Mbps.

**High-Frequency Radio:** During a radio communication, high-frequency electromagnetic radio waves or radio frequency commonly referred to as RF transmissions are generated by the transmitter and are picked up by the receiver. Because the range of radio frequency band is greater than that of infrared, mobile computing elements can communicate over a limited area without both transmitter and receiver being placed along a direct line of sight; the signal can bounce off light walls, buildings, and atmospheric objects. RF transmissions are very good for long distances when combined with satellites to refract the radio waves.

**Microwave:** Microwaves are a higher-frequency version of radio waves but whose transmissions, unlike those of the radio, can be focused in a single direction. Microwave transmissions use a pair of parabolic antennas that produce and receive narrow, but highly directional signals. To be sensitive to signals, both the transmitting and receiving antennas must focus within a narrow area. Because of this, both the transmitting and receiving antennas must be carefully adjusted to align the transmitted signal to the receiver. Microwave communication has two forms: terrestrial, when it is near ground, and satellite microwave. The frequencies and technologies employed by these two forms are similar but with notably distinct differences.

**Laser:** Laser light can be used to carry data for several thousand yards through air and optical fibers. But this is possible only if there are no obstacles in the line of sight. Lasers can be used in many of the same situations as microwaves, and like microwaves, laser beams must be refracted when used over long distances.

---

## 1.5 Network Topology

Computer networks, whether LANs, MANs, or WANs, are constructed based on a topology. There are several topologies including the following popular ones.

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

*Fig. 1.13 Bus Topology*

A collision control mechanism must also improve efficiency in the network using a bus topology by allowing only one element in the network to have control of the bus at any one time. This network element is then called the bus master and other elements are considered to be its slaves. This requirement prevents collision from occurring in the network as elements in the network try to seize the bus at the same time. A bus topology is commonly used by LANs.

### 1.5.4 Star

Another very popular topology, especially in LAN network technologies, is a star topology. A star topology is characterized by a central prominent node that connects to every other element in the network. So, all the elements in the network are connected to a central element. Every network element in a star topology is connected pairwise in a point-to-point manner through the central element, and communication between any pair of elements must go through this central element. The central element or node can either operate in a broadcast fashion, in which case information from one element is broadcast to all connected elements, or transmit as a switching device in which the incoming data is transmitted only to one element, the nearest element en route to the destination. The biggest disadvantage to the star topology in networks is that the failure of the central element results in the failure of the entire network.

![Star Topology](attachment:star_topology.png)

*Fig. 1.14 Star Topology*

### 1.5.5 Ring

Finally, another popular network topology is the ring topology. In this topology, each computing element in a network using a ring topology is directly connected to the transmitting medium via a unidirectional connection so that information put on the transmission medium can reach all computing elements in the network through a mechanism of taking turns in sending information around the ring.

![Ring Topology Network](attachment:ring_topology_network.png)

*Fig. 1.15 Ring Topology Network*

The taking of turns in passing information is managed through a token system. A token is a system-wide piece of information that guarantees the current owner to be the bus master. As long as it owns the token, no other network element is allowed to transmit on the bus. When an element currently sending information and holding the token has finished, it passes the token downstream to its nearest neighbor. The token system is a good management system of collision and fairness.

There are variants of a ring topology collectively called hub hybrids combining either a star with a bus or a stretched star as shown in Fig. 1.16.

![Token Ring Hub](attachment:token_ring_hub.png)

*Fig. 1.16 Token Ring Hub*

Although network topologies are important in LANs, the choice of a topology depends on a number of other factors, including the type of transmission medium, reliability of the network, the size of the network, and its anticipated future growth. Recently the most popular LAN topologies have been the bus, star, and ring topologies. The most popular bus- and star-based LAN topology is the Ethernet, and the most popular ring-based LAN topology is the token ring.

---

## 1.6 Network Connectivity and Protocols

In the early days of computing, computers were used as stand-alone machines, and all work that needed cross-computing was done manually. Files were moved on disks from computer to computer. There was, therefore, a need for cross-computing where more than one computer should talk to others and vice versa.

A new movement was, therefore, born. It was called the open system movement, which called for computer hardware and software manufacturers to come up with a way for this to happen. But to make this possible, standardization of equipment and software was needed. To help in this effort and streamline computer communication, the International Standards Organization (ISO) developed the Open System Interconnection (OSI) model. The OSI is an open architecture model that functions as the network communication protocol standard, although it is not the most widely used one. The Transport Control Protocol/Internet Protocol (TCP/IP) model, a rival model to OSI, is the most widely used. Both OSI and TCP/IP models use two protocol stacks, one at the source element and the other at the destination element.

### 1.6.1 Open System Interconnection (OSI) Protocol Suite

The development of the OSI model was based on the secure premise that a communication task over a network can be broken into seven layers, where each layer represents a different portion of the task. Different layers of the protocol provide different services and ensure that each layer can communicate only with its own neighboring layers. That is, the protocols in each layer are based on the protocols of the previous layers.

Starting from the top of the protocol stack, tasks and information move down from the top layers until they reach the bottom layer where they are sent out over the network media from the source system to the destination. At the destination, the task or information rises back up through the layers until it reaches the top. Each layer is designed to accept work from the layer above it and to pass work down to the layer below it, and vice versa. To ease interlayer communication, the interfaces between the layers are standardized. However, each layer remains independent and can be designed independently and each layer's functionality should not affect the functionalities of other layers above and below it.

![ISO Logical Peer Communication Model](attachment:iso_logical_peer_communication.png)

*Fig. 1.17 ISO Logical Peer Communication Model*

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

Table 1.1: ISO Protocol Layers and Corresponding Services

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

Table 1.2: OSI Datagrams Seen in Each Layer with Header Added

Although the development of the OSI model was intended to offer a standard for all other proprietary models, and it was as encompassing of all existing models as possible, it never really replaced many of those rival models it was intended to replace. In fact, it is this "all in one" concept that led to market failure because it became too complex. Its late arrival on the market also prevented its much-anticipated interoperability across networks.

### 1.6.2 Transport Control Protocol/Internet Protocol (TCP/IP) Model

Among the OSI rivals was the TCP/IP, which was far less complex and more historically established by the time the OSI came on the market. The TCP/IP model does not exactly match the OSI model. For example, it has two to three fewer levels than the seven layers of the OSI model. It was developed for the US Department of Defense Advanced Research Project Agency (DARPA); but over the years, it has seen a phenomenal growth in popularity and it is now the de facto standard for the Internet and many intranets. It consists of two major protocols: the transmission control protocol (TCP) and the Internet protocol (IP), hence the TCP/IP designation. Table 1.3 shows the layers and protocols in each layer.

| Layer | Delivery Unit | Protocols |
| :--: | :--: | :--: |
| Application | Message | - Handles all higher level protocols including File Transfer Protocol (FTP), Name Server Protocol (NSP), Simple Mail Transfer Protocol (SMTP), Simple Network Management Protocol (SNMP), HTTP, Remote file access (telnet), Remote file server (NFS), Name Resolution (DNS), HTTP, TFTP, SNMP, DHCP, DNS, BOOTP <br> - Combines Application, Session and Presentation Layers of the OSI model. <br> - Handles all high-level protocols |
| Transport | Segment | - Handles transport protocols including Transmission Control Protocol (TCP), User Datagram Protocol (UDP). |
| Network | Datagram | - Contains the following protocols: Internet Protocol (IP), Internet Control Message Protocol (ICMP), Internet Group Management Protocol (IGMP). <br> - Supports transmitting source packets from any network on the internetwork and makes sure they arrive at the destination independent of the path and networks they took to reach there. <br> - Best path determination and packet switching occur at this layer. |
| Data Link | Frame | Contains protocols that require IP packet to cross a physical link from one device to another directly connected device. <br> - It included the following networks: <br> - WAN - Wide Area Network <br> - LAN - Local Area Network |
| Physical | Bit stream | All network card drivers. |

Table 1.3: TCP/IP Protocol Layers

Since TCP/IP is the most widely used in most network protocol suites by the Internet and many intranets, let us focus on its layers here.

#### 1.6.2.1 Application Layer

This layer, very similar to the application layer in the OSI model, provides the user interface with resources rich in application functions. It supports all network applications and includes many protocols on a data structure consisting of bit streams.

#### 1.6.2.2 Transport Layer

This layer, again similar to the OSI model session layer, is a slightly removed from the user and is hidden from the user. Its main purpose is to transport application layer messages that include application layer protocols in their headers between the host and the server. For the Internet network, the transport layer has two standard protocols: transport control protocol (TCP) and user datagram protocol (UDP). TCP provides a connection-oriented service, and it guarantees the delivery of all application layer packets to their destination. This guarantee is based on two mechanisms: congestion control that throttles the transmission rate of the source element when there is traffic congestion in the network and the flow control mechanism that tries to match sender and receiver speeds to synchronize the flow rate and reduce the packet drop rate. While TCP offers guarantees of delivery of the application layer packets, UDP, on the other hand, offers no such guarantees. It provides a no-frills connectionless service with just delivery and no acknowledgments. But it is much more efficient and a protocol of choice for real-time data such as streaming video and music. Transport layer delivers transport layer packets and protocols to the network layer.

![TCP Data Structure](attachment:tcp_data_structure.png)

*Fig. 1.19 A TCP Data Structure*

|  | 32 bits |
| :--: | :--: |
| Source address | Destination address |
| Sequence number | Acknowledgement number |
| Other control information |  |
| Data |  |

Table 1.4: TCP Data Structure

![UDP Data Structure](attachment:udp_data_structure.png)

*Fig. 1.20 An UDP Data Structure*

|  | 32 bits |
| :--: | :--: |
| Source address | Destination address |
| Other header control information | UDP Checksum |
| Data |  |

Table 1.5: UDP Data Structure

#### 1.6.2.3 Network Layer

This layer moves packets, now called datagrams, from router to router along the path from a source host to the destination host. It supports a number of protocols including the Internet Protocol (IP), Internet Control Message Protocol (ICMP), and Internet Group Management Protocol (IGMP). The IP Protocol is the most widely used network layer protocol. IP uses header information from the transport layer protocols that include datagram source and destination port numbers from IP addresses, and other TCP header and IP information, to move datagrams from router to router through the network. Best routes are found in the network by using routing algorithms.

![IP Datagram Structure](attachment:ip_datagram_structure.png)

*Fig. 1.21 An IP Datagram Structure*

| Other header control information | Source port number | Destination port number | Data |
| :-- | :-- | :-- | :-- |

Table 1.6: IP Datagram Structure

The standard IP address has been the so-called IPv4, a 32-bit addressing scheme. But with the rapid growth of the Internet, there was fear of running out of addresses, so IPv6, a new 64-bit addressing scheme, was created. The network layer conveys the network layer protocols to the data link layer.

#### 1.6.2.4 Data Link Layer

This layer provides the network with services that move packets from one packet switch like a router to the next over connecting links. This layer also offers reliable delivery of network layer packets over links. It is at the lowest level of communication, and it includes the network interface card (NIC) and operating system (OS) protocols. The protocols in this layer include: Ethernet, asynchronous transfer mode (ATM), and others such as frame relay. The data link layer protocol unit, the frame, may be moved over links from source to destination by different link layer protocols at different links along the way.

#### 1.6.2.5 Physical Layer

This layer is responsible for literally moving data link datagrams bit by bit over the links and between the network elements. The protocols here depend on and use the characteristics of the link medium and the signals on the medium.

---

## 1.7 Network Services

For a communication network to work effectively, data in the network must be able to move from one network element to another. This can only happen if the network services to move such data work. For data networks, these services fall into two categories:

- **Connection services** to facilitate the exchange of data between the two network communicating end-systems with as little data loss as possible and in as little time as possible.
- **Switching services** to facilitate the movement of data from host to host across the length and width of the network mesh of hosts, hubs, bridges, routers, and gateways.

### 1.7.1 Connection Services

How do we get the network transmitting elements to exchange data over the network? Two types of connection services are used: the connected-oriented and connectionless services.

#### 1.7.1.1 Connected-Oriented Services

With a connection-oriented service, before a client can send packets with real data to the server, there must be a three-way handshake. We will define this three-way handshake in later chapters. But the purpose of a three-way handshake is to establish a session before the actual communication can begin. Establishing a session before data is moved creates a path of virtual links between the end systems through a network and therefore, guarantees the reservation and establishment of fixed communication channels and other resources needed for the exchange of data before any data is exchanged and as long as the channels are needed. For example, this happens whenever we place telephone calls; before we exchange words, the channels are reserved and established for the duration. Because this technique guarantees that data will arrive in the same order it was sent in, it is considered to be reliable. In short the service offers the following:

- Acknowledgments of all data exchanges between the end-systems.
- Flow control in the network during the exchange.
- Congestion control in the network during the exchange.

Depending on the type of physical connections in place and the services required by the systems that are communicating, connection-oriented methods may be implemented in the data link layers or in the transport layers of the protocol stack, although the trend now is to implement it more at the transport layer. For example, TCP is a connection-oriented transport protocol in the transport layer. Other network technologies that are connection-oriented include the frame relay and ATMs.

#### 1.7.1.2 Connectionless Service

In a connectionless service, there is no handshaking to establish a session between the communicating end-systems, no flow control, and no congestion control in the network. This means that a client can start communicating with a server without warning or inquiry for readiness; it simply sends streams of packets, called datagrams, from its sending port to the server's connection port in single point-to-point transmissions with no relationship established between the packets and between the end-systems. There are advantages and of course disadvantages to this type of connection service. In brief, the connection is faster because there is no handshaking which can sometimes be time-consuming, and it offers periodic burst transfers with large quantities of data and, in addition, it has simple protocol. However, this service offers minimum services, no safeguards and guarantees to the sender since there is no prior control information and no acknowledgment. In addition, the service does not have the reliability of the connection-oriented method, and offers no error handling and no packets ordering; in addition, each packet self-identifies that leads to long headers, and finally, there is no predefined order in the arrival of packets.

Like the connection-oriented method, this service can operate both at the data link and transport layers. For example, UDP, a connectionless service, operates at the transport layer.

---

## 1.7.2 Network Switching Services

Before we discuss communication protocols, let us take a detour and briefly discuss data transfer by a switching element. This is a technique by which data is moved from host to host across the length and width of the network mesh of hosts, hubs, bridges, routers, and gateways. This technique is referred to as data switching. The type of data switching technique used by a network determines how messages are transmitted between the two communicating elements and across that network. There are two types of data switching techniques: circuit switching and packet switching.

### 1.7.2.1 Circuit Switching

In circuit switching networks, one must reserve all the resources before setting up a physical communication channel needed for communication. The physical connection, once established, is then used exclusively by the two end-systems, usually subscribers, for the duration of the communication. The main feature of such a connection is that it provides a fixed data rate channel, and both subscribers must operate at this rate. For example, in a telephone communication network, a connected line is reserved between the two points before the users can start using the service. One issue of debate on circuit switching is the perceived waste of resources during the so-called silent periods when the connection is fully in force but not being used by the parties. This situation occurs when, for example, during a telephone network session, a telephone receiver is not hung up after use, leaving the connection still established. During this period, while no one is utilizing the session, the session line is still open.

### 1.7.2.2 Packet Switching

Packet switching networks, on the other hand, do not require any resources to be reserved before a communication session begins. These networks, however, require the sending host to assemble all data streams to be transmitted into packets. If a message is large, it is broken into several packets. Packet headers contain the source and the destination network addresses of the two communicating end-systems. Then, each of the packets is sent on the communication links and across packet switches (routers). On receipt of each packet, the router inspects the destination address contained in the packet. Using its own routing table, each router then forwards the packet on the appropriate link at the maximum available bit rate. As each packet is received at each intermediate router, it is forwarded on the appropriate link interspersed with other packets being forwarded on that link. Each router checks the destination address, if it is the owner of the packet; it then reassembles the packets into the final message.

![Packet Switching Networks](attachment:packet_switching_networks.png)

*Fig. 1.22 Packet Switching Networks*

Packet switches are considered to be store-and-forward transmitters, meaning that they must receive the entire packet before the packet is retransmitted or switched on to the next switch.

Because there is no predefined route for these packets, there can be unpredictably long delays before the full message can be reassembled. In addition, the network may not dependably deliver all the packets to the intended destination. To ensure that the network has a reliably fast transit time, a fixed maximum length of time is allowed for each packet. Packet switching networks suffer from a few problems, including the following:

- The rate of transmission of a packet between two switching elements depends on the maximum rate of transmission of the link joining them and on the switches themselves.
- Momentary delays are always introduced whenever the switch is waiting for a full packet. The longer the packet, the longer the delay.
- Each switching element has a finite buffer for the packets. It is thus possible for a packet to arrive only to find the buffer full with other packets. Whenever this happens, the newly arrived packet is not stored but gets lost, a process called packet dropping. In peak times, servers may drop a large number of packets. Congestion control techniques use the rate of packet drop as one measure of traffic congestion in a network.

Packet switching networks are commonly referred to as packet networks for obvious reasons. They are also called asynchronous networks and in such networks, packets are ideal because there is a sharing of the bandwidth, and of course, this avoids the hassle of making reservations for any anticipated transmission. There are two types of packet switching networks:

- **Virtual circuit network** in which a packet route is planned, and it becomes a logical connection before a packet is released and
- **Datagram network**, which is the focus of this book.

---

## 1.8 Network Connecting Devices

Before we discuss network connecting devices, let us revisit the network infrastructure. We have defined a network as a mesh of network elements, commonly referred to as network nodes, connected together by conducting media. These network nodes can be either at the ends of the mesh, in which case they are commonly known as clients or in the middle of the network as transmitting elements. In a small network such as a LAN, the nodes are connected together via special connecting and conducting devices that take network traffic from one node and pass it on to the next node. If the network is big Internetwork (large networks of networks like WANs and LANs), these networks are connected to other special intermediate networking devices so that the Internet functions as a single large network.

Now let us look at network connecting devices and focus on two types of devices: those used in networks (small networks such as LANs) and those used in internetworks.

### 1.8.1 LAN Connecting Devices

Because LANs are small networks, connecting devices in LANs are less powerful with limited capabilities. There are hubs, repeaters, bridges, and switches.

#### 1.8.1.1 A Hub

This is the simplest in the family of network connecting devices since it connects the LAN components with identical protocols. It takes in imports and retransmits them verbatim. It can be used to switch both digital and analog data. In each node, pre-setting must be done to prepare for the formatting of the incoming data. For example, if the incoming data is in digital format, the hub must pass it on as packets; however, if the incoming data is analog, then the hub passes as a signal. There are two types of hubs: simple and multiple port hubs.

![Simple Hub](attachment:simple_hub.png)

*Fig. 1.23 A Simple Hub*

![Multi-Ported Hubs](attachment:multi_ported_hubs.png)

*Fig. 1.24 Multi-Ported Hubs*

Network hubs are designed to work with network adapters and cables and can typically run at either 10 Mbps or 100 Mbps; some hubs can run at both speeds. To connect computers with differing speeds, it is better to use hubs that run at both speeds 10/100 Mbps.

#### 1.8.1.2 A Repeater

A network repeater is a low-level local communication device at the physical layer of the network that receives network signals, amplifies them to restore them to full strength, and then retransmits them to another node in the network. Repeaters are used in a network for several purposes including countering the attenuation that occurs when signals travel long distances, and extending the length of the LAN above the specified maximum. Since they work at the lowest network stack layer, they are less intelligent than their counterparts such as bridges, switches, routers, and gateways in the upper layers of the network stack.

![Repeater in an OSI Model](attachment:repeater_osi_model.png)

*Fig. 1.25 A Repeater in an OSI Model*

#### 1.8.1.3 A Bridge

A bridge is like a repeater but differs in that a repeater amplifies electrical signals because it is deployed at the physical layer; a bridge is deployed at the data link and therefore amplifies digital signals. It digitally copies frames. It permits frames from one part of a LAN or a different LAN with different technology to move to another part or another LAN. However, in filtering and isolating a frame from one network to another or another part of the same network, the bridge will not move a damaged frame from one end of the network to the other. As it filters the data packets, the bridge makes no modifications to the format and content of the incoming data. A bridge filters the frames to determine whether a frame should be forwarded or dropped. All "noise" (collisions, faulty wiring, power surges, etc.) packets are not transmitted.

The bridge filters and forwards frames on the network using a dynamic bridge table. The bridge table, which is initially empty, maintains the LAN addresses for each computer in the LAN and the addresses of each bridge interface that connects the LAN to other LANs. Bridges, like hubs, can be either simple or multi-ported.

![Simple Bridge](attachment:simple_bridge.png)

*Fig. 1.26 Simple Bridge*

![Multi-Ported Bridge](attachment:multi_ported_bridge.png)

*Fig. 1.27 Multi-Ported Bridge*

![Position of a Bridge in an OSI Protocol Stack](attachment:bridge_osi_stack.png)

*Fig. 1.28 Position of a Bridge in an OSI Protocol Stack*

#### 1.8.1.4 A Switch

A switch is a network device that connects segments of a network or two small networks such as Ethernet or token ring LANs. Like the bridge, it also filters and forwards frames on the network with the help of a dynamic table. This point-to-point approach allows the switch to connect multiple pairs of segments at a time, allowing more than one computer to transmit data at a time, thus giving them a high performance over their cousins, the bridges.

### 1.8.2 Internetworking Devices

Internetworking devices connect together smaller networks, like several LANs creating much larger networks such as the Internet. Let us look at two of these connectors: the router and the gateway.

#### 1.8.2.1 Routers

Routers are general-purpose devices that interconnect two or more heterogeneous networks represented by IP subnets or unnumbered point-to-point lines. They are usually dedicated special-purpose computers with separate input and output interfaces for each connected network. They are implemented at the network layer in the protocol stack.

![Router in the OSI Protocol Stack](attachment:router_osi_stack.png)

*Fig. 1.29 Router in the OSI Protocol Stack*

According to RFC 1812, a router performs the following functions:

- Conforms to specific Internet protocols specified in the 1812 document, including the Internet protocol (IP), Internet control message protocol (ICMP), and others as necessary.
- Connects to two or more packet networks. For each connected network, the router must implement the functions required by that network because it is a member of that network. These functions typically include the following:
  - Encapsulating and decapsulating the IP datagrams with the connected network framing. For example, if the connected network is an Ethernet LAN, an Ethernet header and checksum must be attached.
  - Sending and receiving IP datagrams up to the maximum size supported by that network; this size is the network's maximum transmission unit or MTU.
  - Translating the IP destination address into an appropriate network-level address for the connected network. These are the Ethernet hardware address on the NIC, for Ethernet cards, if needed. Each network addresses the router as a member computer of its own network. This means that each router is a member of each network it connects to. It, therefore, has a network host address for that network and an interface address for each network it is connected to. Because of this rather strange characteristic, each router interface has its own address resolution protocol (ARP) module, its LAN address (network card address), and its own Internet protocol (IP) address.
  - Responding to network flow control and error indications, if any.
  - Receives and forwards Internet datagrams. Important issues in this process are buffer management, congestion control, and fairness. To do this the router must:
    - Recognize error conditions and generate ICMP error and information messages as required.
    - Drop datagrams whose time-to-live fields have reached zero.
    - Fragment datagrams when necessary to fit into the maximum transmission unit (MTU) of the next network.
    - Chooses a next-hop destination for each IP datagram based on the information in its routing database.
    - Usually supports an interior gateway protocol (IGP) to carry out distributed routing and reachability algorithms with the other routers in the same autonomous system. In addition, some routers will need to support an exterior gateway protocol (EGP) to exchange topological information with other autonomous systems.
    - Provides network management and system support facilities, including loading, debugging, status reporting, exception reporting, and control.

Forwarding an IP datagram from one network across a router requires the router to choose the address and relevant interface of the next-hop router or for the final hop if it is the destination host. The next-hop router is always in the next network of which the router is also a member. The choice of the next-hop router, called forwarding, depends on the entries in the routing table within the router.

Routers are smarter than bridges in that the router with the use of a router table has some knowledge of possible routes a packet could take from its source to its destination. Once it finds the destination, it determines the best, fastest, and most efficient way of routing the package. The routing table, like in the bridge and switch, grows dynamically as activities in the network develop. On receipt of a packet, the router removes the packet headers and trailers and analyzes the IP header by determining the source and destination addresses and data type and noting the arrival time. It also updates the router table with new addresses if not already in the table. The IP header and arrival time information is entered in the routing table. If a router encounters an address it cannot understand, it drops the package. Let us explain the working of a router by an example using Fig. 1.30.

![Working of a Router](attachment:working_router.png)

*Fig. 1.30 Working of a Router*

In Fig. 1.30, suppose host A in LAN1 tries to send a packet to host B in LAN2. Both host A and host B have two addresses: the LAN (host) address and the IP address. The translation between host LAN addresses and IP addresses is done by the ARP, and data is retrieved or built into the ARP table, similar to Table 1.4. Notice also that the router has two network interfaces: interface 1 for LAN1 and interface 2 for LAN2 for the connection to a larger network such as the Internet. Each interface has a LAN (host) address for the network the interface connects on and a corresponding IP address. As we will see later in the chapter, host A sends a packet to router 1 at time 10:01 that includes, among other things, both its addresses, message type, and destination IP address of host B. The packet is received at interface 1 of the router; the router reads the packet and builds row 1 of the routing table as shown in Table 1.5.

The router notices that the packet has to go to network 193.55.1.*, where *** are digits 0-9, and it has knowledge that this network is connected on interface 2. It forwards the packet to interface 2. Now, interface 2 with its own ARP may know host B. If it does, then it forwards the packet and updates the routing table with the inclusion of row 2. What happens when the ARP at the router interface 1 cannot determine the next network? That is, if it has no knowledge of the presence of network 193.55.1.*, it will then ask for help from a gateway. Let us now discuss how IP chooses a gateway to use when delivering a datagram to a remote network.

#### 1.8.2.2 Gateways

Gateways are more versatile devices than routers. They perform protocol conversion between different types of networks, architectures, or applications and serve as translators and interpreters for network computers that communicate in different protocols and operate in dissimilar networks, for example, OSI and TCP/IP. Because the networks are different with different technologies, each network has its own routing algorithms, protocols, domain names servers, and network administration procedures and policies. Gateways perform all of the functions of a router and more. The gateway functionality that does the translation between different network technologies and algorithms is called a protocol converter.

![Position of a Gateway](attachment:gateway_position.png)

*Fig. 1.31 Position of a Gateway*

Gateways services include packet format and/or size conversion, protocol conversion, data translation, terminal emulation, and multiplexing. Since gateways perform a more complicated task of protocol conversion, they operate more slowly and handle fewer devices.

Let us now see how a packet can be routed through a gateway or several gateways before it reaches its destination. We have seen that if a router gets a datagram, it checks the destination address and finds that it is not on the local network. It, therefore, sends it to the default gateway. The default gateway now searches its table for the destination address. In case the default gateway recognizes that the destination address is not on any of the networks it is connected to directly, it has to find yet another gateway to forward it through.

The routing information the server uses for this is in a gateway routing table linking networks to gateways that reach them. The table starts with the network entry 0.0.0.0, a catch-all entry, for default routes. All packets to an unknown network are sent through the default route. Table 1.6 shows the gateway routing table.

| Network | Gateway | Interface |
| :-- | :-- | :-- |
| 0.0.0.0 | 192.133.1.1 | 1 |
| 127.123.0.1 | 198.24.0.1 | 2 |

Table 1.6: A Gateway Routing Table

The choice between a router, a bridge, and a gateway is a balance between functionality and speed. Gateways, as we have indicated, perform a variety of functions; however, because of this variety of functions, gateways may become bottlenecks within a network because they are slow.

Routing tables may be built either manually for small LANs or by using software called routing daemons for larger networks.

---

## 1.9 Network Technologies

Earlier in this chapter, we indicated that computer networks are basically classified according to their sizes with the local area networks (LANs) covering smaller areas, and the bigger ones covering wider areas (WANs). In this last section of the chapter, let us look at a few network technologies in each one of these categories.

### 1.9.1 LAN Technologies

Recall our definition of a LAN at the beginning of this chapter. We defined a LAN to be a small data communication network that consists of a variety of machines that are all part of the network and cover a geographically small area such as one building or one floor. Also, a LAN is usually owned by an individual or a single entity such as an organization. According to IEEE 802.3 Committee on LAN Standardization, a LAN must be a moderately sized and geographically shared peer-to-peer communication network broadcasting information for all on the network to hear via a common 

popular