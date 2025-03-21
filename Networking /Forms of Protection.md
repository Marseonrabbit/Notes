Now, we know what model objects are or need to be protected. Let us briefly, keep details for later, survey ways and forms of protecting these objects. Prevention of unauthorized access to system resources is achieved through a number of services that include access control, authentication, confidentiality, integrity, and nonrepu- diation.

## Access Control

This is a service the system uses, together with a user pre-provided identification information such as a password, to determine who uses what of its services. Let us look at some forms of access control based on hardware and software.

### Hardware Access Control Systems

Rapid advances in technology have resulted in efficient access control tools that are open and flexible, while at the same time ensuring reasonable precau- tions against risks. Access control tools falling in this category include the following:

- **Access terminal.** Terminal access points have become very sophisticated, and• now they not only carry out user identification but also verify access rights, control access points, and communicate with host computers. These activities can be done in a variety of ways including fingerprint verification and real-time anti-break-in sensors. Network technology has made it possible for these units to be connected to a monitoring network or remain in a stand-alone off-line mode. 
- **Visual event monitoring.** This is a combination of many technologies into one• very useful and rapidly growing form of access control using a variety of real- time technologies including video and audio signals, aerial photographs, and global positioning system (GPS) technology to identify locations.
- **Identification cards.**** Sometimes called proximity cards, these cards have• become very common these days as a means of access control in buildings, financial institutions, and other restricted areas. The cards come in a variety of forms, including magnetic, bar coded, contact chip, and a combination of these. 
- **Biometric identification**. This is perhaps the fastest growing form of control• access tool today. Some of the most popular forms include fingerprint, iris, and voice recognition. However, fingerprint recognition offers a higher level of security. 
- **Video surveillance.** This is a replacement of CCTV of yester year, and it is• gaining popularity as an access control tool. With fast networking technologies and digital cameras, images can now be taken and analyzed very quickly, and action taken in minutes.

### Software Access Control Systems

Software access control falls into two types: point of access monitoring and remote monitoring. In point of access (POA), personal activities can be monitored by a PC-based application. The application can even be connected to a network or to a designated machine or machines. The application collects and stores access events and other events connected to the system operation and download access rights to access terminals. In remote mode, the terminals can be linked in a variety of ways, including the use of modems, telephone lines, and all forms of wireless connections. Such termi- nals may, sometimes if needed, have an automatic calling at pre-set times if desired or have an attendant to report regularly.

## Authentication

Authentication is a service used to identify a user. User identity, especially of remote users, is difficult because many users, especially those intending to cause harm, may masquerade as the legitimate users when they actually are not. This service provides a system with the capability to verify that a user is the very one he or she claims to be based on what the user is, knows, and has. 

Physically, we can authenticate users or user surrogates based on checking one or more of the following user items: 
- **User name (sometimes screen name)**• 
- **Password**• 
- **Retinal images•** : The user looks into an electronic device that maps his or her eye retina image; the system then compares this map with a similar map stored on the system. 
- **Fingerprints•** : The user presses on or sometimes inserts a particular finger into a device that makes a copy of the user fingerprint and then compares it with a similar image on the system user file. 
- **Physical location•** : The physical location of the system initiating an entry request is checked to ensure that a request is actually originating from a known and authorized location. In networks, to check the authenticity of a client’s location a network or Internet protocol (IP) address of the client machine is compared with the one on the system user file. This method is used mostly in addition to other security measures because it alone cannot guarantee security. If used alone, it provides access to the requested system to anybody who has access to the client machine. 
- I**dentity cards•** : Increasingly, cards are being used as authenticating documents. Whoever is the carrier of the card gains access to the requested system. As is the case with physical location authentication, card authentication is usually used as a second-level authentication tool because whoever has access to the card automatically can gain access to the requested system

## Confidentiality

The confidentiality service protects system data and information from unauthorized disclosure. When data leave one extreme of a system such as a client’s computer in a network, it ventures out into a nontrusting environment. So, the recipient of that data may not fully trust that no third party like a cryptanalysis or a man-in-the middle has eavesdropped on the data. This service uses encryption algorithms to ensure that nothing of the sort happened while the data was in the wild. Encryption protects the communications channel from sniffers. Sniffers are easy to write and install and difficult to detect. The encryption process uses an encryption algorithm and key to transform data at the source, called plaintext; turn it into an encrypted form called ciphertext, usually unintelligible form; and finally recover it at the sink. The encryption algorithm can either be symmetric or asymmetric. Symmetric encryption or secret key encryption, as it is usually called, uses a common key and the same cryptographic algorithm to scramble and unscramble the message. Asymmetric encryption commonly known as public key encryption uses two different keys: a pub- lic key known by all and a private key known by only the sender and the receiver. Both the sender and the receiver each has a pair of these keys, one public and one private. To encrypt a message, a sender uses the receiver’s public key which was published. Upon receipt, the recipient of the message decrypts it with his or her private key.

## Integrity

The integrity service protects data against active threats such as those that may alter it. Just like data confidentiality, data in transition between the sending and receiving parties is susceptible to many threats from hackers, eavesdroppers, and cryptanalysts whose goal is to intercept the data and alter it based on their motives. This service, through encryption and hashing algorithms, ensures that the integrity of the transient data is intact. A hash function takes an input message M and creates a code from it. The code is commonly referred to as a hash or a message digest. A one-way hash function is used to create a signature of the message – just like a human fingerprint. The hash function is, therefore, used to provide the message’s integrity and authenticity. The signature is then attached to the message before it is sent by the sender to the recipient.

## Nonrepudiation

This is a security service that provides proof of origin and delivery of service and/ or information. In real life, it is possible that the sender may deny the ownership of the exchanged digital data that originated from him or her. This service, through digital signature and encryption algorithms, ensures that digital data may not be repudiated by providing proof of origin that is difficult to deny. A digital signature is a cryptographic mechanism that is the electronic equivalent of a written signature to authenticate a piece of data as to the identity of the sender. We have to be careful here because the term “nonrepudiation” has two meanings, one in the legal world and the other in the cryptotechnical world. Adrian McCullagh and Willian Caelli define “nonrepudiation” in a cryptotechnical way as follows:

- In authentication, a service that provides proof of the integrity and origin of data,• both in a forgery-proof relationship, which can be verified by any third party at any time; or
- In authentication, an authentication that with high assurance can be asserted to• be genuine, and that cannot subsequently be refuted

However, in the legal world, there is always a basis for repudiation This basis, again according to Adrian McCullagh, can be as follows:

- **The signature is a forgery.•** 
- **The signature is not a forgery, but was obtained via**• 
- **Unconscionable conduct by a party to a transaction;•**
- **Fraud instigated by a third party;•** 
- **Undue influence exerted by a third party.•**

We will use the cryptotechnical definition throughout the book. To achieve non- repudiation, users and application environments require a nonrepudiation service to collect, maintain, and make available the irrefutable evidence. The best services for nonrepudiation are digital signatures and encryption. These services offer trust by generating unforgettable evidence of transactions that can be used for dispute resolution after the fact.
