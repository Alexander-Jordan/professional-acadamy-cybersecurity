# Unit 4: Network Security Basics

## Summary

In this Unit we covered:

- Historical Timeline
- Technologies, Protocols & Standards
- Internet, Intranet & Extranet
- Data Communication Principles
- Transmission Concepts
- OSI Reference Model
- Network Data devices
- Cloud Computing

## U4P1-P2: Unit Introduction and Video: A Brief History of the Internet

Learning outcomes:

- Historical Timeline
- The Internet & The World Wide Web
- Protocols, Standards & Technologies
- Data Communication Principles
- Transmission Concepts
- Cloud Computing - Intro

[A Brief History of the Internet](https://www.youtube.com/watch?v=FbMHY8I_kQ8)

## U4P3: Activity

Read about the history of networking the web:

[Timeline of Computer History - Networking the web](https://www.computerhistory.org/timeline/networking-the-web/)

## U4P4-P5: Historical Timeline - The Internet and Video - What is the Internet?

### The internet

> A global computer network providing a variety of information and communication facilities, consisting of interconnected networks using standardized communication protocols.

- Public infrastructure
- Carries data from protocols
  - WWW
  - FTP
  - Email
  - etc.

Started as a concept to create a decentralized and distributed network of computers.

To communicate even if some nodes in the network was disconnected.

### Centralized, Decentralized and Distributed networks

[LinkedIn: Centralised, Decentralised and Distributed networks - What's the deal?](https://www.linkedin.com/pulse/centralised-decentralised-distributed-networks-whats)

- Centralized: all nodes are connected under a single authority
- Decentralized: no single authority server controls the nodes, they all have individual entity
- Distributed: every node is independent and interconnected with each other

> It's important to note that many real-world systems exist on a spectrum between these models, and the choice of network architecture depends on factors like efficiency, security, scalability, and the specific goals of the network.

### What is the internet? (video)

<https://youtu.be/Dxcc6ycZ73M>

## U4P6-P7: The Internet: Important Developments and Video

1. TCP/IP: Transmission Control Protocol/Internet Protocol. Data communication protocols used on internet. Developed by Robert Kahn and Vint Cerf of DARPA. Maintained by IETF. Vint Cerf interview. 1970s
2. World Wide Web and HTML: Tim Berners-Lee, CERN, Interconnecting documents via links. Web protocol and code free to all. Tim Berners- Lee interview. 1990s
3. Browser – WWW useless without browser to "view" it. 1990s
4. Search Engines – Way to find stuff. Google
5. Internet Service Providers – Provide and lease the infrastructure to run the internet. Telephone line to broadband (ISPs actually makes us dependent on them to have access to the internet, creating a 1 point failure)

### The Internet: Packets, Routing & Reliability (video)

<https://www.youtube.com/watch?v=AYdF7b3nMto>

- Data is not transmitted from a server to the end user in a straight path, in order to be **fault tolerant** and follow the key principle of the internet: **reliability**
- Instead one piece of data is divided into smaller **packets** that are sent using **different paths** depending on the **availability** and **cheapest** cost (time, politics, relationships)
- The paths are determined by special computers in the network called **routers**, acting as **traffic managers**, and the more routers: the more **reliable** the internet becomes
- **TCP** (Transmission Control Protocol) **checks and verify** that all packets have been sent and received, and will either **acknowledge** that a package has been received, or ask the server to send any **missing packages**
- All different devices making up the internet can **connect**, **communicate** and **collaborate** because of **agreed upon standards** for how data is sent around

## U4P8-P9: The World Wide Web and Video

- End device: any device that can send or receive packets. Anything with an IP address.
- Internet allows applications to operate. Types of applications include
  - WWW
  - Email
  - FTP
  - VPN

### The open university video

- The internet rely on protocols like IP (Internet Protocol) and TCP (Transmission Control Protocol), or TCP/IP
- Since all computers use these protocols it might seem all are connecting in 1 network, but there are really multiple networks in tiers
- The lowest tier are computers being connected in a LAN (Local Area Network), which is connected to the next tier: ISPs (Internet Service Provider) or cooperative networks, which then are connected to the next tier: telecommunication companies that own the cables making up the physical internet
- The top-most tier of the internet is sometimes called `The internet backbone`
- Before sending data, TCP breaks up data into smaller packets and sends it with other needed information, like the sender, receiver, and a serial number
- The routers try to send the packets to a known receiver from a list of connected devices (router table), and will delegate the job to a router from a higher tier if it's not possible, which mean that a packet could at the end go all the way to the backbone of the internet before finding it's destination
- Routers inform each other if they are available or overloaded, so that the traffic can be redirected
- TCP on the receiving computer verifies, acknowledges, asks for missing or damage packets, and assemble the packets in the correct order using the serial number for each packet

## U4P10-12: The Internet Continued, The World Wide Web and Video: "How This Guy Invented the World Wide Web"

<https://hootsuite.widen.net/s/kd6qgn9rwx/digital2022globaloverview_report_en>

In 2022, some numbers to show the scale of the internet:

- Population: 7.91 billion (57% urbanization)
- Unique mobile phone users: 5.31 billion (67.1%)
- Internet users: 4.95 billion (62.5%)
- Active social media users: 4.62 billion (58.4%)

From **2015 to 2025** we have gone from **15.41 billion** connected IoT (Internet of Things) devices to **75.44 billion** worldwide.

### World Wide Web

> Definition: an information system on the internet which allows documents (identified by URLs) to be connected to other documents by hypertext links, enabling the user to search for information by moving from one document to another. (Oxford, 2021)

DNS (Domain Name System): is the phonebook of the Internet. Humans access information online through domain names, like nytimes.com or espn.com. Web browsers interact through Internet Protocol (IP) addresses. DNS translates domain names to IP addresses so browsers can load Internet resources.

HTML (Hypertext Markup Language): a standardized system for tagging text files to achieve font, color, graphic, and hyperlink effects on World Wide Web pages.

### A brief history of the World Wide Web (video)

<https://www.youtube.com/watch?v=sSqZ_hJu9zA>

- 1980: used fax machines to share documents, and travel agencies to book flights and hotels
- Tim Berners-Lee wrote a program named `ENQUIRE` to link different software and hardware, so all personal could work and share information easier together
- 1989 & 1990: Time proposed the idea of the World Wide Web as a Hypertext project
- 1993: CERN management decided that the Web should act as an open standard for all to use

### Tim Berners-Lee: How This Guy Invented the World Wide Web 30 Years Ago (video)

<https://www.youtube.com/watch?v=GUrDI6OkJfU>

- Combines 3 main ideas: Hypertext, TCP, and DNS
- First ever created website (6 Aug 1991): <https://info.cern.ch/>
- The World Wide Web is the application using the internet, so they are not the same thing

## U4P13: Protocols & Standard

### URL (Uniform Resource Locator)

- Example: <https://subdomain.domain.com/subfolder/slug> (`https://`: protocol; `.com`: TLD (Top-Level Domain))
- Protocol: HTTP, HTTPS
- Subdomain: most recognized: `www`, but can be anything, and each domain can have multiple domains
- Domain: the core website you're targeting/visiting
- TLD (Top-Level Domain): `com` stood for `company` originally, and now the TLD is often used to indicate the location or intent of the website
- Subfolder: Used to find a specific folder or part of the website
- Slug: Used to find a specific resource of the website (a page or file)

### Browsers

- 1990: WorldWideWeb is created, the first ever web browser
- 1991: Erwise is launched providing a graphical interface to the web browser
- 1992: ViolaWWW launches and brings scripts to the web
- 1993: Mosaic is released and makes web browsing mainstream
- 1994: Netscape Navigator becomes the worlds top browser
- 1996: Microsoft invests in it's own browser, starting the browser war
- 1999: Internet Explorer is the top browser (preinstalled on all Windows PCs)
- 2002: Netscape code becomes Mozilla Firefox
- 2008: Google Chrome launches
- 2012: Google Chrome is the most used browser in the world
- 2015: Microsoft rebrand their browser: Microsoft Edge
- 2020: Google Chrome remains as the top used browser

### Protocols

- Set of agreed rules to enable communication over a connection.
  - Type of data
  - Format of data
  - Headers include information on the data
  - How to process the data
  - How to deal with errors detection and resending packets

### Standards

Standards are used throughout all industries to provide interoperability between products developed by different vendors.

Some examples:

- IETF (Internet Engineering Task Force): a large open international community of network designers, operators, vendors, and researchers concerned with the evolution of the Internet architecture and the smooth operation of the Internet.
- ISO (International Organization for Standardization): an independent, non-governmental international organization with a membership of 165 national standards bodies. ISO27001: Information Security Management
- IEEE (Institute of Electrical and Electronic Engineers): IEEE and its members inspire a global community to innovate for a better tomorrow through its more than 396,000 members in over 160 countries, and its highly cited publications, conferences, technology standards, and professional and educational activities. 802 LAN Standards
- ITU (International Telecommunications Union): The United Nations specialized agency for information and communication technologies – ICTs. ITU is committed to connecting all the world's people – wherever they live and whatever their means. Through our work, we protect and support everyone's right to communicate. Remote connectivity standards.
- NIST (National Institute of Standards and Technology): Part of US Department of Commerce. Provides testing lab to rigorously test new standards to ensure that they meet the requirements for the product they cover. Another area that crops up regularly for Communications and the Internet is timing and keeping everything in synchronization. NIST provide access to one of the most accurate time signals on the Internet through a network of Atomic Clocks.
- ANSI (American National Standards Institute): responsible for setting standards across all areas of business in the US. They are the US representative on other
international standards organizations. ASCII code.

### Internet, intranet & extranet

They work basically the same, but the access is different.

- Internet: A public network that is open to anyone owning a device that can access it
- Intranet: A private network that is locked and only accessible to people within a specific organization
- Extranet: A branch of a company's intranet that third-parties, like vendors or customers, have access to

### Net neutrality (activity)

- What is it: ISPs (Internet Service Providers) must treat all internet communications equally, offering consistent transfer rates regardless of content, website, platform, application, type of equipment, source address, destination address, or method of communication (source: [Wikipedia](https://en.wikipedia.org/wiki/Net_neutrality))
- Who benefits from net neutrality: the end-user of the web
- Who is opposed to net neutrality: ISPs, broadband and telecommunications companies, computer hardware manufacturers, economists, and notable technologists
- Europe vs US: Contrary to Europe, US is has had their ups and downs supporting net neutrality
- What’s zero-rating: it's like a free sample of web content. ISPs will not add any costs to these resources, and they are therefore more accessible than other resources on the web
- Why does it matter: it makes it more accessible and introduces content that would not be introduced otherwise

## U4P15-16: Data Communication Principles and Video

Data is transferred in the form of bits between two or more digital devices.

### Serial Transmission

Serial data transmission sends data bits one after another over a single channel.

- Asynchronous Serial Transmission: cost effective but slower
- Synchronous Serial Transmission: continuous stream, dependent on timing

### Parallel Transmission

Parallel data transmission sends multiple data bits at the same time over multiple channels.

- Data can be sent much faster
- Easier to program
- Errors more frequent
- Used for video as prevents buffering

### Modes of Transmission

Mode | Direction of communication | Send / Receive | Performance | Example
---|---|---|---|---
**Simplex** | Unidirectional | Sender can only send data | Worst performing mode of transmission | Keyboard & monitor
**Half Duplex** | Two-directional (one at a time) | Sender can send & receive data (one at a time) | Better than Simplex | Walkie-talkie
**Full Duplex** | Two-directional, simultaneously | Sender can send & receive data simultaneously | Best performing mode of transmission | Telephone

### Errors

- Error Control: reduce and fix errors.
- Error Prevention: good connections.
- Error Detection: detect early using checkbits, checksum procedures etc.
- Error Correction: detect, drop and call for retransmit.

### Types of Networks

Size Based

- PAN (Personal Area Network): network in your home office, for 1 person (access to printers, external storage, etc)
- LAN (Local Area Network): typical office, for multiple persons a localized area
- MAN (Metropolitan Area Network): collection of LANs, college for example
- WAN (Wide Area Network): large geographical area, like a city, or the internet

Purpose Based

- SAN (Storage Area Network)
- EPN (Enterprise Private Network)
- VPN (Virtual Private Network)

### The OSI (Open Systems Interconnection) Reference Model

Developed by the ISO (International Standards Organization) as a model for computer communications architectures, and as a framework for developing protocol standards.

- **Layer 7: Application** (end-user layer)
  - Most familiar to users
  - Utilizes services to transmit and receive data to/from layer 6
  - Applications such as browsers or email clients utilizes these services/protocols
  - Protocols: HTTP, FTP, IRC, SSH, DNS
- **Layer 6: Presentation** (syntax layer)
  - Converting data from one format to another
  - After converting data from either layer 7 (transmitting) or 5 (receiving), it sends the translated data to the other layer
  - Protocols: SSL, SSH, IMAP, FTP, MPEG, JPEG
- **Layer 5: Session** (sync & send to port layer)
  - Where the construction, direction, & conclusion of connections between devices occur
  - Responsible for authentication and reconnection if disrupted
  - After establishing the connection, it transfers data either from or to layer 4
  - Protocols: API's, Sockets, WinSock
- **Layer 4: Transport** (end-to-end connections layer)
  - Responsible for the transmission of data between network connections
  - How much data is sent, how fast, where it goes, etc
  - Protocols: TCP, UDP
- **Layer 3: Network** (packets layer)
  - Handles the routing of the data
  - Will decide if the data has either reached its target, or send it further away
  - Protocols: IP, ICMP, IPSec, IGMP
- **Layer 2: Data link** (frames layer)
  - Responsible for framing, error detection (parity check, checksum, CRC), error correction, flow control, addressing
  - From within the same local network
  - Most complex, divided between:
    - MAC (Media Access Control) layer
      - Manages device interaction, addressing frames, controls physical media access
    - LLC (Logical Link Control) layer
      - Deals with multiplexing, the flow of data among applications & other devices, and provides error messages and acknowledgements
  - Sets up links across the physical network
  - When data is received from the physical layer (1), it checks for transmission errors and then packages the bits into data frames
  - When data is received from the network layer (3), it divides packets into frames and sends those frames bit-by-bit to the physical layer (1)
  - From there, it manages the physical addressing methods for the MAC or LLC layers
  - Protocols: Ethernet, PPP, Switch, Bridge, NIC, WAP
- **Layer 1: Physical** (physical structure layer)
  - Responsible for transmitting digital data bits from the source over network communications media (electrical, mechanical or radio) to the receiving devices
  - When troubleshooting, this is in most cases the first place to check
  - Protocols: Coax, Fiber, Wireless, Hubs, Repeaters

Not how it look in actuality, but the reference model and how it's structured is great for when we develop or troubleshoot where the issues are.

[What is OSI Model?](https://www.youtube.com/watch?v=Ilk7UXzV_Qc)

## U4P17-18: IP Addresses and Video

A unique identifier (a series of characters, such as `192.168.1.1`) assigned to a device or domain that connects to the Internet.

IP packets are created by adding an IP header to each packet of data before it is sent on its way.

An IP header is just a series of bits, and records several pieces of information about the packet, including the sending and receiving IP address.

### The Internet: IP Addresses & DNS (video)

<https://youtu.be/5o8CwafCxnU?feature=shared>

- IP (Internet Protocol) addresses acts similar to a receivers address in the real world
- The numbers and characters in an IP address is represented in bits
- Traditional IP addresses are 32-bits, with 8 bits for each part of the address
- The first part is pointing to the network (previously country and region)
- The next part is pointing to the subnetwork
- And lastly it points to the device
- This specific IP version is name IPv4, designed 1973, provides more than 4 billion unique addresses
- We are now in a multi-year transition from IPv4 to IPv6, which uses 128-bits (340 undecillion unique addresses)
- DNS (Domain Name System) is used to find the corresponding IP address from a domain name (such as example.com)
- DNS servers are connected into a distributed hierarchy, divided into zones for major domains (such as .org, .com, .net, etc)
- DNS is an open & public protocol, which makes it susceptible to cyber attacks (like DNS spoofing, which is an attacker changing the corresponding IP address for a saved domain)

## U4P19: Transmission Concepts

The physical means by which data is transmitted from one geographic or electronic location to another is called transmission, or “communication” media.

The data transmission capabilities of the various medias vary differently depending upon the various factors. These factors are:

- **Bandwidth:** refers to the data carrying capacity of a channel or medium. Higher bandwidth communication channels support higher data rates.
- **Radiation:** refers to the leakage of signal from the medium due to undesirable electrical characteristics of the medium.
- **Noise Absorption:** refers to the susceptibility of the media to external electrical noise that can cause distortion of data signal.
- **Attenuation:** refers to loss of energy as signal propagates outwards. The amount of energy lost depends on frequency.

### Types of transmission media

- Guided media (cable)
  - Twisted pair cable
  - Coaxial cable
  - Optical fibre cable
- Unguided (unbound) media
  - Radiowaves
    - Electromagnetic waves ranging in frequencies between 3 kHz and 1 GHz
    - Omnidirectional
    - Long distance
    - Multicasting (one sender, many receivers)
    - AM & FM Radio, TV, cordless phone, pagers.
  - Microwaves
    - Electromagnetic waves ranging in frequencies between 1-300 GHz
    - Unidirectional
    - Line-of-sight
    - Unicast (one-to-one)
    - Satellite comms, mobile phone comms, wifi etc.
  - Infrared
    - Frequencies 300 Ghz to 400 THz
    - Short-range communication
    - Can’t penetrate walls
    - TV remote, Alarm sensors

#### Ground, sky, and line-of-sight propagation

Ground wave propagation travels along the Earth's surface and is effective at lower frequencies, while sky wave propagation reflects off the ionosphere and is used for long-distance communication at higher frequencies. Line-of-sight propagation occurs when radio waves travel directly in a straight line between transmitting and receiving antennas, typically used for short-range communications.

[Sky Wave vs. LOS Wave vs. Ground Wave Propagation](https://www.rfwireless-world.com/terminology/sky-wave-vs-los-wave-vs-ground-wave-propagation)

### Bluetooth

- Bluetooth is a type of wireless communication used to transmit voice and data at high speeds using radio waves at 2.45 GHz.
- Standard protocol for short-range radio communications between many different types of devices (mobile phones, computers, entertainment systems and other).
- Within 10 meters of each other.
- Spread-spectrum frequency-hopping technology

### Connecting to internet

- Fixed Internet
  - Dial-up connection (obsolete)
  - DSL (Digital Subscriber Line): broadband over phone lines. 24 Mbps
  - Cable Internet: cable TV infrastructure 200 Mbps
  - Fiber Broadband: up to 1000 Mbps
  - Satellite Internet: via dish (rural option) 50 Mbps
- Mobile Internet
  - Via mobile device
  - 3G/4G: 100 Mbps
  - 5G: 1 GBps

## U4P20-21: Network Data Devices and Video

- Repeaters: enables signals to travel longer distances over a network by regenerating the signal.
- Hubs: simple devices that direct data packets to all devices connected to the hub, regardless of whether the data package is destined for the device.
- Switches: more advanced. Instead of broadcasting the frames everywhere, a switch actually checks for the destination MAC address and forward it to the relevant port to reach that computer only.
- Routers: a physical or virtual appliance that passes information between two or more packet-switched computer networks - analyzing a given data packet's destination IP address, calculating the best way for it to reach that destination and then forwarding it accordingly.

### Cloud computing (video)

In preparation for unit 6.

In essence, cloud computing is viewed as a utility much like water and electricity.
Instead of having limited amounts of it (normal users) or lot's of it (big corporations), you can request more or lower the computing power if you need to.
You pay for what you use.

## U4P22-23: Video "The Future of the Internet"

[Interview with Vint Cerf about the future of the internet](https://www.youtube.com/watch?v=BRakbBZkhyA)
