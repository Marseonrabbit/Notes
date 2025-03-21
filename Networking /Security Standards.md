The computer network model also suffers from the standardization problem. Secu- rity protocols, solutions, and best practices that can secure the computer network model come in many different types and use different technologies resulting in incompatibility of interfaces (more in Chapter 16), less interoperability, and unifor- mity among the many system resources with differing technologies within the sys- tem and between systems. System managers, security chiefs, and experts, therefore, choose or prefer standards, if no de facto standard exists, that are based on service, industry, size, or mission. The type of service offered by an organization determines the types of security standards used. Like service, the nature of the industry an organization is in also determines the types of services offered by the system, which in turn determines the type of standards to adopt. The size of an organization also determines what type of standards to adopt. In relatively small establishments, the ease of implementation and running of the system influence the standards to be adopted. Finally, the mission of the establishment also determines the types of stan- dards used. For example, government agencies have a mission that differs from that of a university. These two organizations, therefore, may choose different standards. We are, therefore, going to discuss security standards along these divisions. Before we do that, however, let us look at the bodies and organizations behind the formula- tion, development, and maintenance of these standards. These bodies fall into the following categories:

- International organizations such as the Internet Engineering Task Force (IETF),• the Institute of Electronic and Electric Engineers (IEEE), the International Standards Organization (ISO), and the International Telecommunications Union (ITU)
- Multinational organizations like the European Committee for Standardization• (CEN), Commission of European Union (CEU), and European Telecommunications Standards Institute (ETSI). 
- National governmental organizations like the National Institute of Standards• and Technology (NIST), American National Standards Institute (ANSI), and Canadian Standards Council (CSC). 
- Sector specific organizations such as the European Committee for Banking• Standards (ECBS), European Computer Manufacturers Association (ECMA), and Institute of Electronic and Electric Engineers (IEEE). 
- Industry standards such as RSA, the Open Group (OSF + X/Open), Object• Management Group (OMG), World Wide Web Consortium (W3C)), and the Organization for the Advancement of Structured Information Standards (OASIS). Other sources of standards in security and cryptography.• 

Each one of these organizations has a set of standards. Table 2.1 shows some of these standards. In the table, x is any digit between 0 and 9.

## Security Standards Based on Type of Service/Industry

System and security managers and users may choose a security standard to use based on the type of industry they are in and what type of services that industry provides. Table 2.2 shows some of these services and the corresponding security standards that can be used for these services.

Let us now give some details of some of these standards
![[Pasted image 20250321130327.png]]
![[Pasted image 20250321130358.png]]
### Public-Key Cryptography Standards (PKCS)

In order to provide a basis and a catalyst for interoperable security based on public-key cryptographic techniques, the Public-Key Cryptography Standards (PKCS) were estab- lished. These are recent security standards, first published in 1991 following discussions of a small group of early adopters of public-key technology. Since their establishment, they have become the basis for many formal standards and are implemented widely. In general, PKCS are security specifications produced by RSA Laboratories in cooperation with secure systems developers worldwide for the purpose of acceler- ating the deployment of public-key cryptography. In fact, worldwide contributions from the PKCS series have become part of many formal and de facto standards, including ANSI X9 documents, PKIX, SET, S/MIME, and SSL.

### The Standards For Interoperable Secure MIME (S/MIME)

S/MIME (Secure Multipurpose Internet Mail Extensions) is a specification for secure electronic messaging. It came to address a growing problem of e-mail inter- ception and forgery at the time of increasing digital communication. So, in 1995 several software vendors got together and created the S/MIME specification with the goal of making it easy to secure messages from prying eyes. It works by building a security layer on top of the industry standard MIME pro- tocol based on PKCS. The use of PKCS avails the user of S/MIME with immediate privacy, data integrity, and authentication of an e-mail package. This has given the standard a wide appeal, leading to S/MIME moving beyond just e-mail. Already vendor software warehouses, including Microsoft, Lotus, Banyan, and other on-line electronic commerce services are using S/MIME.

### Federal Information Processing Standards (FIPS)

Federal Information Processing Standards (FIPS) are National Institute of Stan- dards and Technology (NIST)-approved standards for advanced encryption. These are U.S. federal government standards and guidelines in a variety of areas in data processing. They are recommended by NIST to be used by U.S. government organi- zations and others in the private sector to protect sensitive information. They range from FIPS 31 issued in 1974 to current FIPS 198.

### Secure Sockets Layer (SSL)

SSL is an encryption standard for most Web transactions. In fact, it is becoming the most popular type of e-commerce encryption. Most conventional intranet and extranet applications would typically require a combination of security mechanisms that include Encryption• Authentication• Access control• SSL provides the encryption component implemented within the TCP/IP proto- col. Developed by Netscape Communications, SSL provides secure web client and server communications, including encryption, authentication, and integrity check- ing for a TCP/IP connection.

### Web Services Security Standards

In order for Web transactions such as e-commerce to really take off, customers will need to see an open architectural model backed up by a standards-based secu- rity framework. Security players, including standards organizations, must provide that open model and a framework that is interoperable, that is, as vendor-neutral as possible, and able to resolve critical, often sensitive, issues related to security. The security framework must also include Web interoperability standards for access control, provisioning, biometrics, and digital rights.

To meet the challenges of Web security, two industry rival standards companies are developing new standards for XML digital signatures that include XML Encryption, XML Signature, and exXensible Key Management Specification (XKMS) by the World Wide Web Consortium (W3C), and BSAFE SecurXML-C software development kit (SDK) for implementing XML digital signatures by rival RSA Security. In addition, RSA also offers a SAML Specification (Security Assertion Markup Language), an XML framework for exchanging authentication, and authorization information. It is designed to enable secure single sign-on across portals within and across organizations


## Security Standards Based on Size/Implementation

If the network is small or it is a small organization such as a university, for example, security standards can be spelled out as best practices on the security of the sys- tem, including the physical security of equipment, system software, and application software. 

- **Physical security** – this emphasizes the need for security of computers running• the Web servers and how these machines should be kept physically secured in a locked area. Standards are also needed for backup storage media like tapes and removable disks.
- **Operating systems.** The emphasis here is on privileges and number of accounts,• and security standards are set based on these. For example, the number of users with most privileged access like root in UNIX or Administrator in NT should be kept to a minimum. Set standards for privileged users. Keep to a minimum the number of user accounts on the system. State the number of services offered to clients computers by the server, keeping them to a minimum. Set a standard for authentication such as user passwords and for applying security patches. 
- **System logs.** Logs always contain sensitive information such as dates and times• of user access. Logs containing sensitive information should be accessible only to authorized staff and should not be publicly accessible. Set a standard on who and when logs should be viewed and analyzed. 
- **Data security.** Set a standard for dealing with files that contain sensitive data. For• example, files containing sensitive data should be encrypted wherever possible using strong encryption or should be transferred as soon as possible and practical to a secured system not providing public services.

![[Pasted image 20250321131848.png]]
![[Pasted image 20250321131907.png]]

## Security Standards Based on Interests

In many cases, institutions and government agencies choose to pick a security stan- dard based solely on the interest of the institution or the country. Table 2.4 below shows some security standards based on interest, and the subsections following the table also show security best practices and security standards based more on national interests.

### British Standard 799 (BS 7799)

The BS 7799 standard outlines a code of practice for information security manage- ment that further helps to determine how to secure network systems. It puts forward a common framework that enables companies to develop, implement, and measure effective security management practice and provide confidence in inter-company trading. BS 7799 was first written in 1993, but it was not officially published until 1995, and it was published as an international standard BS ISO/IEC 17799:2000 in December 2000.

### Orange Book

This is the U.S. Department of Defense Trusted Computer System Evaluation Cri- teria (DOD-5200.28-STD) standard known as the Orange Book. For a long time, it has been the de facto standard for computer security used in government and industry, but as we will see in Chapter 15, other standards have now been developed to either supplement it or replace it. First published in 1983, its security levels are referred to as Rainbow Series.


### Homeland National Security Awareness

![[Pasted image 20250321132101.png]]

## Best Practices in Security

As you noticed from our discussion, there is a rich repertoire of standards and best practices on the system and infosecurity landscape because as technology evolves, the security situation becomes more complex and it grows more so every day. With these changes, however, some truths and approaches to security remain the same. One of these constants is having a sound strategy of dealing with the changing secu- rity landscape. Developing such a security strategy involves keeping an eye on the reality of the changing technology scene and rapidly increasing security threats. To keep abreast of all these changes, security experts and security managers must know how and what to protect and what controls to put in place and at what time. It takes security management, planning, policy development, and the design of procedures. Here are some examples of best practices. Commonly Accepted Security Practices and Regulations (CASPR): Devel- oped by the CASPR Project, this effort aims to provide a set of best practices that can be universally applied to any organization regardless of industry, size or mission. Such best practices would, for example, come from the world’s experts in information security. CASPR distills the knowledge into a series of papers and publishes them so they are freely available on the Internet to everyone. The project covers a wide area, including operating system and system security, network and telecommunication security, access control and authentication, infosecurity man- agement, infosecurity auditing and assessment, infosecurity logging and monitor- ing, application security, application and system development, and investigations and forensics. In order to distribute their papers freely, the founders of CASPR use the open source movement as a guide, and they release the papers under the GNU Free Document License to make sure they and any derivatives remain freely available. 

Control Objectives for Information and (Related) Technology (COBIT): Developed by IT auditors and made available through the Information Systems Audit and Control Association, COBIT provides a framework for assessing a secu- rity program. COBIT is an open standard for control of information technology. The IT Governance Institute has, together with the world-wide industry experts, analysts and academics, developed new definitions for COBIT that consist of Maturity Models, Critical Success Factors (CSFs), Key Goal Indicators (KGIs), and Key Performance Indicators (KPIs). COBIT was designed to help three distinct audiences:

- Management who need to balance risk and control investment in an often• unpredictable IT environment 
- Users who need to obtain assurance on the security and controls of the IT services• upon which they depend to deliver their products and services to internal and external customers 
- Auditors who can use it to substantiate their opinions and/or provide advice to• management on internal controls

Operationally Critical Threat, Asset and Vulnerability Evaluation (OCTAVE) by Carnegie Mellon’s CERT Coordination Center: OCTAVE is an approach for self- directed information security risk evaluations that:

- Puts organizations in charge•
- Balances critical information assets, business needs, threats, and vulnerabilities• 
- Measures the organization against known or accepted good security practices• 
- Establishes an organization-wide protection strategy and information security• risk mitigation plans 

In short, it provides measures based on accepted best practices for evaluating security programs. It does this in three phases: 

- First, it determines information assets that must be protected.• 
- Evaluates the technology infrastructure to determine if it can protect those assets• and how vulnerable it is and defines the risks to critical assets 
- Uses good security practices, establishes an organization-wide protection strategy• and mitigation plans for specific risks to critical assets

