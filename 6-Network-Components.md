# STUDY NOTES: NETWORK COMPONENTS

## Table of Contents

1. Introduction to Network Components
2. Nodes
   - Meaning and working of nodes
   - Types of nodes
   - Client, server and peer nodes
   - MAC address, IP address, hostname and port number
3. Network Links and Transmission Media
   - Wired links
   - Wireless links
   - Bandwidth, speed, latency and other link characteristics
4. Intermediary Network Devices
   - Hub
   - Switch
   - Router
   - Bridge
   - Repeater
   - Gateway
   - Modem
   - Wireless Access Point
   - Firewall
5. Network Protocols
   - Meaning and importance of protocols
   - OSI reference model
   - TCP/IP model
   - TCP
   - UDP
   - IP
   - HTTP and HTTPS
   - DNS
   - DHCP
   - Ethernet
   - ARP
   - SMTP, POP3 and IMAP
6. Wireless LAN (WLAN) and Wi-Fi Evolution
   - Meaning and working of WLAN
   - Wi-Fi generations: Wi-Fi 1 to Wi-Fi 7
   - Wi-Fi bands and security
   - Advantages, applications and limitations
7. How All Network Components Work Together
8. Important Networking Terms

---

# 1. Introduction to Network Components

A computer network is a group of interconnected devices that communicate with each other and share information, resources and services. These devices may be computers, mobile phones, printers, servers, cameras or other smart devices.

For a network to work properly, several components are required. A computer needs a way to connect to another computer, a path through which data can travel, devices that help direct the data and rules that make communication possible.

These basic components are:

**1. Nodes:** Devices connected to a network.

**2. Links:** The communication paths that connect network devices.

**3. Intermediary devices:** Equipment that connects networks or helps forward and control data.

**4. Protocols:** Rules that define how devices communicate and exchange information.

### Basic mind map of a computer network

```text
                    COMPUTER NETWORK
                           |
          +----------------+----------------+
          |                |                |
         NODES            LINKS         INTERMEDIARY
       (Devices)       (Connections)       DEVICES
          |                |                |
     Computers         Wired cables       Switch
     Mobiles           Wireless           Router
     Printers          signals            Access Point
     Servers                              Firewall
          |
          +-------------------------------+
                          |
                       PROTOCOLS
                    (Communication rules)
                          |
                    TCP/IP, HTTP,
                    DNS, DHCP, etc.
```

**Real-world example:** Consider a college computer laboratory. The computers are nodes, Ethernet cables provide the links, switches connect the computers, a router connects the laboratory to the internet, and protocols such as TCP/IP allow the computers to exchange information.

---

# 2. Nodes

A **node** is any device connected to a network that can send, receive, process or forward data. In simple words, every device that participates in network communication can be considered a node.

A node does not necessarily have to be a computer. A smartphone, printer, server, smart television, CCTV camera and network router can all be nodes.

### How a node works

```text
Device connects to network
          |
          v
Obtains network identity
          |
          v
Sends or receives data
          |
          v
Processes the information
          |
          v
Communicates with other devices
```

For example, when a laptop connects to college Wi-Fi, it becomes a node on that network. It can access websites, communicate with the college server or send documents to a network printer.

## 2.1 Types of nodes

### A. Client node

A client is a device or system that requests a service or resource from another device, usually a server.

**Example:** A student's laptop requesting lecture notes from the college website.

**Features and functions:**
- Sends requests to servers.
- Receives information and services.
- Uses network resources such as files, websites and printers.
- Usually runs applications such as browsers, email programs and office software.

**Applications:** Student computers, office laptops, smartphones, ATM machines and online shopping applications.

**Limitations:** A client may not be able to access information when the server is unavailable or the network connection is interrupted.

### B. Server node

A server is a computer or software system that provides information, services or resources to other devices on a network.

**Example:** A college server storing student records, attendance details and examination results.

**Features and functions:**
- Handles requests from multiple clients.
- Stores and manages data.
- Provides services such as websites, email and file sharing.
- Controls access through user accounts and permissions.
- May run continuously to provide services.

**Applications:** Banking systems, websites, cloud storage, college management systems and online shopping platforms.

**Limitations:** Servers may be expensive to maintain. If a central server fails without a backup system, many users may lose access to its services.

### C. Peer node

A peer is a device that can act as both a client and a server. It can request information and also provide resources to other devices.

**Example:** Two computers sharing files directly without using a central file server.

**Features and functions:**
- Allows direct communication between devices.
- Shares files and other resources.
- Does not always require a central server.
- Can distribute work among multiple devices.

**Applications:** Small home networks, peer-to-peer file sharing and some distributed applications.

**Limitations:** Security, backup and access management can become difficult when the number of devices increases.

### D. Network device node

Network equipment can also be treated as nodes because it participates in communication and forwards data.

**Examples:** Routers, switches, firewalls and wireless access points.

**Functions:** Connecting devices, forwarding traffic, managing communication and controlling access.

**Applications:** Homes, schools, offices, data centres and internet service provider networks.

## 2.2 Important identities used by nodes

A device needs an identity so that data can reach the correct destination.

### MAC address (Media Access Control address)

A MAC address is a hardware-level or link-layer address associated with a network interface. It is commonly used for communication within a local network.

**Example:** `00:1A:2B:3C:4D:5E`

**Features:**
- Commonly represented using hexadecimal numbers.
- Usually assigned to a network interface by its manufacturer.
- Used by Ethernet and Wi-Fi networks for local frame delivery.
- A device with multiple network interfaces may have multiple MAC addresses.

**Limitation:** A MAC address is not a replacement for an IP address when communication has to take place across different networks. It can also be changed or spoofed in some situations.

### IP address (Internet Protocol address)

An IP address is a logical address assigned to a network interface so that it can communicate using the Internet Protocol.

There are two main versions:

**IPv4:** Uses 32-bit addresses.

Example: `192.168.1.10`

**IPv6:** Uses 128-bit addresses.

Example: `2001:db8::1`

**Functions:**
- Identifies network interfaces logically.
- Helps deliver packets from source to destination.
- Supports communication between different networks.

**Applications:** Internet browsing, email, online gaming, video calls and file transfers.

### Hostname

A hostname is a readable name assigned to a device.

Example: `Library-PC-01`

It is easier for a person to remember a hostname than a numerical IP address.

### Port number

A port number identifies a particular application or service on a device when using transport-layer protocols such as TCP or UDP.

Examples:
- HTTP: TCP port 80
- HTTPS: TCP port 443
- DNS: commonly port 53
- SMTP submission: commonly port 587

### Difference between MAC address, IP address, hostname and port

| Term | Purpose | Example |
|---|---|---|
| MAC address | Identifies a network interface at the link layer | 00:1A:2B:3C:4D:5E |
| IP address | Identifies a network interface logically | 192.168.1.10 |
| Hostname | Gives a readable name to a device | Library-PC-01 |
| Port number | Identifies an application or service | 443 |

---

# 3. Network Links and Transmission Media

A **network link** is the communication path that connects two or more network devices and allows data to travel between them.

For example, the Ethernet cable connecting a computer to a switch is a wired link. The radio connection between a phone and a Wi-Fi access point is a wireless link.

### How a network link works

```text
          SENDING DEVICE
                |
                v
         Data is converted
           into signals
                |
                v
        Signals travel through
          the transmission
              medium
                |
                v
         Receiving device
          detects signals
                |
                v
         Data is reconstructed
```

Network links can be divided into two main categories: wired links and wireless links.

## 3.1 Wired links

Wired links use physical cables to connect network devices. They are commonly used when a stable and reliable connection is required.

### A. Twisted-pair cable

Twisted-pair cable consists of pairs of insulated copper wires twisted together. The twisting helps reduce electromagnetic interference.

**Types:**
- UTP (Unshielded Twisted Pair): Does not have additional metallic shielding around the wire pairs.
- STP (Shielded Twisted Pair): Includes shielding to reduce interference.

**Features and functions:**
- Commonly used for Ethernet connections.
- Easy to install and relatively inexpensive.
- Supports different Ethernet speeds depending on the cable category.
- Connects computers, switches, routers and access points.

**Applications:** Computer laboratories, offices, home networks and CCTV systems.

**Limitations:** Performance depends on cable quality, distance and installation. Many familiar copper Ethernet connections have a standard maximum channel length of 100 metres.

**Example:** A desktop computer connected to an office switch using a Cat6 Ethernet cable.

### B. Coaxial cable

Coaxial cable contains a central copper conductor surrounded by insulation, a metallic shield and an outer protective covering.

**Features and functions:**
- Provides shielding against interference.
- Carries high-frequency electrical signals.
- Used for television and broadband communication.

**Applications:** Cable television, cable internet and some CCTV installations.

**Limitations:** It is bulkier than twisted-pair cable and is not commonly used for modern office Ethernet connections.

**Example:** A cable modem connected to the broadband coaxial line supplied by an internet provider.

### C. Optical fibre cable

Optical fibre uses light signals to transmit information through thin strands of glass or plastic.

**Types:**

1. **Single-mode fibre:** Uses a very small core and is generally used for long-distance communication.
2. **Multimode fibre:** Uses a larger core and is commonly used for shorter-distance connections, such as within buildings and data centres.

**Features and functions:**
- Supports very high bandwidth.
- Carries data over long distances.
- Has low signal loss compared with many copper connections.
- Is not affected by electromagnetic interference in the same way as copper cables.

**Applications:** Internet backbone networks, telecom networks, university campuses and data centres.

**Limitations:** Installation and repair require specialised equipment and trained technicians. Fibre equipment can also be more expensive.

**Example:** An internet service provider using fibre cables to connect a neighbourhood to its main network.

## 3.2 Wireless links

Wireless links transmit data without requiring a physical cable between communicating devices. They generally use radio waves or other electromagnetic signals.

### A. Wi-Fi

Wi-Fi is a wireless networking technology based on the IEEE 802.11 family of standards. It allows devices to connect to a local area network without using Ethernet cables.

**Features and functions:**
- Provides wireless network access.
- Allows several devices to connect to one network.
- Supports mobility within the coverage area.
- Can connect devices to the internet through a wireless access point or router.

**Applications:** Homes, colleges, offices, airports, hotels and public hotspots.

**Limitations:** Signal strength can decrease with distance and obstacles. Interference from neighbouring networks and other devices can reduce performance.

**Example:** A student using a laptop to attend an online class through college Wi-Fi.

### B. Bluetooth

Bluetooth is a short-range wireless technology used to exchange information between nearby devices.

**Features and functions:**
- Provides short-range wireless communication.
- Uses relatively low power for many device applications.
- Supports convenient device pairing.
- Can connect devices without requiring a traditional Wi-Fi network.

**Applications:** Wireless headphones, speakers, keyboards, smartwatches and car audio systems.

**Limitations:** It is generally designed for shorter distances and lower data rates than Wi-Fi.

**Example:** A smartphone connected to wireless earbuds.

### C. Cellular network

A cellular network uses radio communication between mobile devices and nearby base stations.

**Features and functions:**
- Provides wide-area mobile connectivity.
- Supports movement between coverage areas.
- Carries voice, messages and internet data.

**Applications:** Smartphones, mobile broadband, vehicle tracking and connected devices.

**Limitations:** Speed and coverage depend on signal strength, location, network congestion and the service plan.

**Example:** A smartphone using 4G or 5G mobile data while travelling.

### D. Satellite communication

Satellite communication uses satellites to transmit signals between distant locations.

**Features and functions:**
- Provides communication over large geographical areas.
- Can reach places where terrestrial networks are difficult to install.
- Supports internet, television and other communication services.

**Applications:** Ships, aircraft, rural communities and remote research stations.

**Limitations:** Some satellite services have higher latency than fibre or local wireless networks. Weather and installation conditions may also affect performance.

**Example:** A remote village using satellite internet because fibre broadband is unavailable.

## 3.3 Important characteristics of network links

**Bandwidth:** The maximum capacity of a communication link to carry data, generally measured in bits per second.

**Throughput:** The actual amount of data successfully transferred over a period of time.

**Latency:** The time taken for data to travel from one point to another. It is commonly measured in milliseconds.

**Jitter:** Variation in packet delay. High jitter can affect video calls and online gaming.

**Packet loss:** The loss of data packets while they travel through a network.

**Interference:** Unwanted signals that disturb communication, particularly in wireless networks.

**Reliability:** The ability of a link to operate consistently without frequent failures.

### Wired and wireless links compared

| Point | Wired link | Wireless link |
|---|---|---|
| Medium | Physical cable | Radio or other wireless signals |
| Mobility | Limited by cable | Greater mobility |
| Interference | Usually less affected by radio interference | Can be affected by radio interference |
| Installation | Requires cable routing | Requires wireless coverage |
| Example | Ethernet | Wi-Fi, Bluetooth |

---

# 4. Intermediary Network Devices

Intermediary devices are networking devices that connect end devices or networks and help data reach its destination. They may forward traffic, control access, repeat signals, translate between networks or manage wireless communication.

They are important because two computers cannot always communicate directly. When a device needs to reach another network, intermediary equipment helps carry the information along the correct path.

### General working of intermediary devices

```text
       COMPUTER A
            |
            v
          SWITCH
            |
            v
          ROUTER
            |
            v
         INTERNET
            |
            v
       REMOTE ROUTER
            |
            v
        COMPUTER B
```

## 4.1 Hub

A hub is a basic networking device that connects multiple computers in a local network. When it receives data through one port, it repeats the signal to all other ports.

**Working:** A hub does not examine the destination MAC address. It simply sends the incoming signal to the other connected ports.

**Features and functions:**
- Connects multiple devices.
- Operates at the Physical Layer (Layer 1) of the OSI model.
- Repeats incoming signals.
- Does not intelligently filter network traffic.

**Applications:** Older small networks and networking demonstrations.

**Limitations:**
- Sends data to every connected device.
- Creates unnecessary network traffic.
- Shares bandwidth among connected devices.
- Can cause collisions in traditional shared Ethernet environments.

**Example:** In an old computer laboratory, a hub may send data from one computer to every other connected computer, even when only one computer is the intended recipient.

Hubs are now largely replaced by switches.

## 4.2 Switch

A switch connects multiple devices within a LAN and forwards Ethernet frames towards the correct destination using MAC addresses.

**Working:** When a switch receives a frame, it examines the source MAC address and learns which port that device is connected to. It stores this information in a MAC address table. When another frame arrives, the switch checks the destination MAC address and forwards the frame through the appropriate port if it knows the destination.

**Features and functions:**
- Connects computers, printers, servers and access points.
- Learns MAC addresses automatically.
- Reduces unnecessary traffic compared with a hub.
- Supports full-duplex communication on typical modern Ethernet links.
- Managed switches can support VLANs, monitoring and traffic-control features.

**Applications:** College computer labs, offices, hospitals, business networks and data centres.

**Limitations:**
- A normal Layer 2 switch does not perform routing between different IP networks.
- Incorrect configuration can cause loops or security problems.
- Managed switches may require technical knowledge.

**Example:** In a computer lab, a switch connects 30 computers and forwards a frame towards the port connected to the intended destination computer.

**OSI layer:** Usually Layer 2 (Data Link). Layer 3 switches can also perform routing.

## 4.3 Router

A router is a networking device that connects different IP networks and forwards packets between them.

**Working:** A router examines the destination IP address of a packet and checks its routing table to decide where to forward it.

**Features and functions:**
- Connects different networks.
- Selects routes for data packets.
- Can connect a home or office LAN to the internet.
- May provide NAT, DHCP, firewall and other services.
- Can use static or dynamic routing.

**Applications:** Home internet connections, office networks, college campuses, data centres and internet service provider networks.

**Limitations:**
- A router can become a point of failure if no backup route or device exists.
- Poor configuration may create security or connectivity problems.
- Performance depends on the router's processing capacity and traffic load.

**Example:** A home router forwards a request from a laptop to a website hosted on a server somewhere on the internet.

**OSI layer:** Mainly Layer 3 (Network Layer).

## 4.4 Bridge

A bridge is a networking device used to connect two or more LAN segments and filter traffic using MAC addresses.

**Working:** It examines the destination MAC address and decides whether a frame needs to be forwarded to another network segment.

**Features and functions:**
- Connects LAN segments.
- Filters unnecessary traffic.
- Learns MAC addresses.
- Operates at the Data Link Layer.

**Applications:** Older LAN designs and some specialised network equipment.

**Limitations:** Modern switches perform the same basic function more efficiently and with more ports.

**Example:** A bridge connecting two sections of an older office LAN.

## 4.5 Repeater

A repeater is a device that receives a weakened signal, regenerates it and sends it onwards.

**Working:**

```text
Weak signal
     |
     v
  Repeater
     |
     v
Regenerated signal
     |
     v
Extended communication path
```

**Features and functions:**
- Regenerates signals.
- Extends the communication distance.
- Does not normally examine destination addresses.
- Operates at the Physical Layer.

**Applications:** Extending wired communication paths and some wireless coverage systems.

**Limitations:** A repeater does not understand or filter the data being transmitted. It cannot solve every problem caused by congestion or poor network design.

**Example:** A wireless range extender relaying a Wi-Fi signal to an area with weak coverage.

## 4.6 Gateway

A gateway is a device or software system that connects different networks or systems and may translate between different communication protocols or formats.

**Working:** A gateway receives information from one system and passes it to another system. Depending on its purpose, it may translate addresses, protocols, data formats or application requests.

**Features and functions:**
- Connects different systems.
- Can translate between communication methods.
- Provides access between different network environments.
- May apply security and traffic-control policies.

**Applications:** Enterprise networks, cloud connections, industrial networks and smart-home systems.

**Limitations:** Complex gateways can be expensive and may introduce extra processing delays. Incorrect configuration can prevent communication.

**Example:** An IoT gateway connecting smart sensors that use one wireless technology to an IP-based office network.

## 4.7 Modem

A modem is a device that converts signals so that digital network equipment can communicate through a particular transmission system. The word modem comes from modulator-demodulator.

**Working:** Depending on the connection technology, it modulates and demodulates signals so that digital information can travel through the service provider's communication medium.

**Features and functions:**
- Provides access through a broadband service.
- Connects a home or office network to an internet service provider.
- Works with technologies such as cable, DSL and cellular broadband.

**Applications:** Home broadband, small businesses and mobile internet connections.

**Limitations:** Its performance depends on the service technology, provider network and subscribed plan.

**Example:** A cable modem connects a home network to an internet service provider through a coaxial cable.

## 4.8 Wireless Access Point (WAP)

A wireless access point allows wireless devices to connect to a wired local area network using Wi-Fi.

**Working:** The access point sends and receives radio signals from wireless devices and bridges their traffic into the wired LAN.

**Features and functions:**
- Provides Wi-Fi coverage.
- Connects wireless clients to a LAN.
- Supports multiple wireless devices.
- Can support several wireless networks and security settings.

**Applications:** Colleges, hotels, offices, hospitals, shopping centres and airports.

**Limitations:** Coverage is affected by walls, distance and interference. Too many active clients can also reduce performance.

**Example:** A college installs several access points across its building so that students can use Wi-Fi in different classrooms.

## 4.9 Firewall

A firewall is a security system that monitors and controls incoming and outgoing network traffic according to defined security rules.

**Working:** It checks network traffic against its rules and allows or blocks communication accordingly.

**Types:**
- Hardware firewall.
- Software firewall.
- Network firewall.
- Host-based firewall.
- Next-generation firewall.

**Features and functions:**
- Blocks unauthorised access.
- Controls traffic between networks.
- Can filter traffic by IP address, port and protocol.
- May inspect application traffic and detect suspicious activity.

**Applications:** Office networks, banking systems, data centres, schools and personal computers.

**Limitations:** A firewall cannot prevent every attack. It must be configured and updated properly, and it should be used alongside other security measures.

**Example:** A college firewall blocks unauthorised access to its internal student database from the public internet.

### Comparison of intermediary devices

| Device | Main purpose | Common OSI layer |
|---|---|---|
| Hub | Repeats signals to all ports | Layer 1 |
| Repeater | Regenerates signals | Layer 1 |
| Bridge | Connects LAN segments and filters frames | Layer 2 |
| Switch | Forwards frames using MAC addresses | Layer 2 |
| Router | Forwards packets between IP networks | Layer 3 |
| Gateway | Connects or translates between systems | Depends on function |
| Modem | Converts signals for a transmission system | Depends on technology |
| Wireless access point | Connects wireless devices to a LAN | Mainly Layers 1 and 2 |
| Firewall | Controls and filters network traffic | Depends on firewall type |

---

# 5. Network Protocols

A **network protocol** is a set of rules that defines how devices communicate and exchange information over a network.

Without protocols, one device might send information in a format that another device cannot understand. Protocols make communication organised by defining how data is formatted, addressed, transmitted, received and checked.

**Real-world example:** When a person opens a website, DNS may help find the website's IP address, IP helps deliver packets, TCP or QUIC provides transport, and HTTP or HTTPS handles the web communication.

### Basic protocol communication

```text
Sender creates data
       |
       v
Protocol adds required information
       |
       v
Data travels through network
       |
       v
Receiver follows the same rules
       |
       v
Data is understood by receiver
```

## 5.1 Important features of network protocols

- **Addressing:** Identifies the source and destination.
- **Data formatting:** Defines how information is organised.
- **Error handling:** Helps detect or recover from transmission problems.
- **Flow control:** Prevents a sender from overwhelming a receiver.
- **Sequencing:** Helps arrange data in the correct order where required.
- **Connection management:** Defines how communication sessions begin and end.
- **Security:** Some protocols provide authentication, encryption and integrity checks.

## 5.2 Understanding network layers

Network communication is divided into layers. Each layer performs a particular job and provides services to the layer above it.

The most widely taught reference model is the **OSI model**, which has seven layers. The Internet commonly uses the **TCP/IP model**, which has four layers. Some textbooks use a five-layer teaching model by separating the physical and data-link functions.

### OSI model: Seven layers

```text
+-----------------------------+
| 7. APPLICATION              |
| User-facing network services|
+-----------------------------+
| 6. PRESENTATION             |
| Data format, encryption     |
+-----------------------------+
| 5. SESSION                  |
| Session management          |
+-----------------------------+
| 4. TRANSPORT                |
| End-to-end delivery         |
+-----------------------------+
| 3. NETWORK                  |
| Logical addressing, routing |
+-----------------------------+
| 2. DATA LINK                |
| Frames, MAC addressing      |
+-----------------------------+
| 1. PHYSICAL                 |
| Signals, cables, radio      |
+-----------------------------+
```

**Layer 1 – Physical Layer**

This layer is responsible for transmitting raw bits through a physical or wireless medium.

Includes:
- Cables and connectors.
- Radio signals.
- Electrical and optical signals.
- Data transmission rates.
- Physical network interfaces.

Example: Ethernet cable carrying electrical signals or fibre carrying light pulses.

**Layer 2 – Data Link Layer**

This layer handles communication over a local link.

Includes:
- Frames.
- MAC addresses.
- Media access.
- Error detection.
- Switching and bridging.

Example: Ethernet and Wi-Fi link-layer communication.

**Layer 3 – Network Layer**

This layer handles logical addressing and routing between networks.

Includes:
- IP addresses.
- Packet forwarding.
- Routing.
- Fragmentation in IPv4 where applicable.

Example: IP forwarding a packet from a home network to a remote website.

**Layer 4 – Transport Layer**

This layer provides communication between applications on different devices.

Includes:
- TCP and UDP.
- Port numbers.
- Segmentation and reassembly.
- Reliability and flow control in TCP.
- Checksums.

Example: TCP delivering web data reliably between a browser and a server.

**Layer 5 – Session Layer**

This layer is responsible for establishing, managing and ending communication sessions in the OSI reference model.

Includes:
- Session establishment.
- Session management.
- Dialog control.
- Synchronisation and checkpoints.

Example: Managing a logical communication session between two applications.

**Layer 6 – Presentation Layer**

This layer deals with how information is represented so that different systems can understand it.

Includes:
- Data formatting.
- Character encoding.
- Compression.
- Encryption and decryption.

Example: Converting information into a format that the receiving application can interpret.

**Layer 7 – Application Layer**

This layer provides network services that applications use.

Includes:
- Web communication.
- Email services.
- File transfer.
- Name resolution.
- Network management.

Examples: HTTP, DNS and SMTP.

**Important:** The OSI model is a reference model for understanding networking. Real-world protocols do not always fit perfectly into one individual OSI layer.

## 5.3 TCP/IP model

The TCP/IP model describes the layered architecture used by the internet.

```text
+-------------------------------+
| APPLICATION                   |
| HTTP, DNS, SMTP, DHCP         |
+-------------------------------+
| TRANSPORT                     |
| TCP, UDP                      |
+-------------------------------+
| INTERNET                      |
| IP, ICMP                      |
+-------------------------------+
| NETWORK ACCESS / LINK         |
| Ethernet, Wi-Fi               |
+-------------------------------+
```

| TCP/IP layer | Main responsibility | Examples |
|---|---|---|
| Application | Provides network services to applications | HTTP, DNS, SMTP, DHCP |
| Transport | Communication between application processes | TCP, UDP |
| Internet | Logical addressing and routing | IP, ICMP |
| Network Access / Link | Local delivery over a network medium | Ethernet, Wi-Fi |

Some textbooks divide the Network Access layer into two separate layers: Data Link and Physical. This produces the commonly taught five-layer model.

---

# 5.4 TCP (Transmission Control Protocol)

TCP is a connection-oriented transport-layer protocol that provides reliable and ordered delivery of data between applications.

It is commonly used when information must arrive correctly and in the right order.

**Example:** Downloading a PDF, sending an email or loading a website over HTTPS using TCP.

### How TCP works

```text
Application creates data
          |
          v
TCP establishes connection
          |
          v
Data is divided into segments
          |
          v
Segments are transmitted
          |
          v
Receiver checks received data
          |
          v
Acknowledgements are sent
          |
          v
Missing data is retransmitted
          |
          v
Data is delivered in order
```

### TCP connection establishment: Three-way handshake

Before normal TCP data transfer, the two devices establish a connection.

```text
CLIENT                         SERVER
  |                               |
  | -------- SYN ---------------> |
  |                               |
  | <------ SYN + ACK ------------|
  |                               |
  | -------- ACK ---------------> |
  |                               |
  |       CONNECTION READY        |
```

**Step 1 – SYN:** The client requests a connection.

**Step 2 – SYN-ACK:** The server acknowledges the request and responds.

**Step 3 – ACK:** The client acknowledges the server's response. The connection is established.

### TCP features and functions

- Connection-oriented communication.
- Reliable delivery.
- Sequence numbers to organise data.
- Acknowledgements to confirm receipt.
- Retransmission of missing data.
- Flow control.
- Congestion control.
- Error detection through checksums.

### TCP at different layers

| Layer | What is involved |
|---|---|
| Layer 1 – Physical | Carries the signals used to transmit TCP data |
| Layer 2 – Data Link | Carries IP packets inside Ethernet or Wi-Fi frames |
| Layer 3 – Network | IP delivers packets between network interfaces |
| Layer 4 – Transport | TCP provides reliable, ordered communication |
| Layer 5 – Session | Application sessions may be managed by software above TCP |
| Layer 6 – Presentation | Data formatting and encryption may be handled by higher-level software |
| Layer 7 – Application | Applications such as HTTP or SMTP use TCP where required |

TCP itself is a **Layer 4 protocol**. It does not independently perform all seven OSI-layer functions.

### Applications of TCP

- Web browsing using HTTP/1.1 or HTTP/2.
- Email transfer.
- File transfer.
- Remote login.
- Database communication.

### Limitations of TCP

- Has more overhead than UDP.
- Connection establishment takes time.
- Retransmissions can increase delay.
- It may not be ideal for applications where very low latency is more important than perfect delivery.

---

# 5.5 UDP (User Datagram Protocol)

UDP is a connectionless transport-layer protocol that sends data without establishing a connection first.

Unlike TCP, it does not guarantee delivery, ordering or retransmission of lost packets. This makes it useful for applications where speed and low delay are important.

**Example:** Live voice communication, online gaming and some video-streaming applications.

### How UDP works

```text
Application creates data
          |
          v
UDP adds port information
          |
          v
Data is divided into datagrams
          |
          v
Datagrams are transmitted
          |
          v
Receiver processes received data
```

UDP does not require a connection handshake before sending data.

### UDP features and functions

- Connectionless communication.
- Low protocol overhead.
- No built-in acknowledgement system.
- No built-in retransmission of lost data.
- No guarantee of packet ordering.
- Uses port numbers to identify application processes.
- Includes a checksum for error detection.

### UDP at different layers

| Layer | What is involved |
|---|---|
| Layer 1 – Physical | Carries the transmitted signals |
| Layer 2 – Data Link | Ethernet or Wi-Fi carries the IP packet in a frame |
| Layer 3 – Network | IP delivers the packet |
| Layer 4 – Transport | UDP provides lightweight datagram delivery |
| Layer 5 – Session | Session handling may be performed by the application |
| Layer 6 – Presentation | Data formatting and encryption may be handled above UDP |
| Layer 7 – Application | Applications such as DNS and some real-time communication systems use UDP |

UDP itself operates at **Layer 4**.

### Applications of UDP

- Online gaming.
- Voice and video communication.
- DNS queries in many common cases.
- Live streaming.
- Real-time monitoring.

### Limitations of UDP

- Does not guarantee delivery.
- Does not automatically resend lost packets.
- Does not guarantee that packets arrive in order.
- Applications may need to implement their own reliability mechanisms.

### TCP and UDP comparison

| TCP | UDP |
|---|---|
| Connection-oriented | Connectionless |
| Reliable delivery | No built-in delivery guarantee |
| Uses acknowledgements | No built-in acknowledgements |
| Maintains data order | No built-in ordering |
| More overhead | Less overhead |
| Suitable for file transfers and many web connections | Suitable for many real-time applications |

---

# 5.6 IP (Internet Protocol)

IP stands for Internet Protocol. It is a network-layer protocol responsible for addressing and forwarding packets from a source to a destination across interconnected networks.

IP provides the addressing system that allows devices on different networks to communicate.

### Types of IP

**IPv4:** Uses 32-bit addresses.

Example: `192.168.1.10`

**IPv6:** Uses 128-bit addresses.

Example: `2001:db8::1`

### How IP works

```text
Source device creates data
           |
           v
Transport layer adds its header
           |
           v
IP adds source and destination addresses
           |
           v
Packet is sent to the next network device
           |
           v
Routers examine destination IP
           |
           v
Packet moves towards destination
           |
           v
Destination device receives packet
```

### IP features and functions

- Provides logical addressing.
- Supports communication between different networks.
- Enables routing.
- Uses packets to carry data.
- IPv4 and IPv6 provide different address formats.
- IP is generally a best-effort delivery protocol; it does not itself guarantee that packets arrive.

### IP at different layers

| Layer | What is involved |
|---|---|
| Layer 1 – Physical | Signals carry the packet |
| Layer 2 – Data Link | Ethernet or Wi-Fi frames carry IP packets over a local link |
| Layer 3 – Network | IP provides addressing and packet forwarding |
| Layer 4 – Transport | TCP or UDP carries application data |
| Layer 5 – Session | Application session handling is above IP |
| Layer 6 – Presentation | Data representation and encryption are handled by higher-level protocols or software |
| Layer 7 – Application | Applications generate the data that IP helps deliver |

IP operates at **Layer 3**.

### Applications of IP

- Internet browsing.
- Email communication.
- Online gaming.
- Video calls.
- Communication between offices and data centres.

### Limitations of IP

- IP alone does not guarantee delivery.
- It does not guarantee packet ordering.
- It does not provide application-level encryption by itself.
- Additional protocols such as TCP, UDP and security protocols are needed for other functions.

---

# 5.7 HTTP and HTTPS

HTTP stands for Hypertext Transfer Protocol. It is an application-layer protocol used to transfer information between web browsers and web servers.

HTTPS is HTTP protected by TLS encryption, which helps protect the confidentiality and integrity of communication and authenticate the server.

**Example:** When someone opens an online shopping website, the browser sends requests and receives website content using HTTP or HTTPS.

### How HTTP works

```text
User enters website address
           |
           v
Browser identifies server
           |
           v
Browser sends HTTP request
           |
           v
Server processes request
           |
           v
Server sends HTTP response
           |
           v
Browser displays webpage
```

### Common HTTP methods

- **GET:** Requests information.
- **POST:** Sends information to a server.
- **PUT:** Creates or replaces a resource.
- **PATCH:** Updates part of a resource.
- **DELETE:** Requests deletion of a resource.

### Features and functions

- Transfers web pages and web application data.
- Uses request-response communication.
- Supports headers and status codes.
- Supports different content types.
- HTTPS adds TLS protection.

### HTTP and HTTPS at different layers

| Layer | What is involved |
|---|---|
| Layer 1 – Physical | Carries electrical, optical or radio signals |
| Layer 2 – Data Link | Ethernet or Wi-Fi carries frames |
| Layer 3 – Network | IP routes packets |
| Layer 4 – Transport | TCP commonly carries HTTP/1.1 and HTTP/2; HTTP/3 uses QUIC over UDP |
| Layer 5 – Session | Session management may be handled by application software |
| Layer 6 – Presentation | TLS encryption and data representation are related to these functions in the OSI teaching model |
| Layer 7 – Application | HTTP defines web requests and responses |

HTTP and HTTPS are **Application Layer protocols**.

### Applications

- Websites.
- Online shopping.
- Banking portals.
- Social media.
- Web-based learning platforms.
- Online forms and applications.

### Limitations

- Plain HTTP does not encrypt the communication.
- HTTPS requires proper certificate and TLS configuration.
- HTTP itself does not guarantee that a website is trustworthy; users must still check the website and its security.

---

# 5.8 DNS (Domain Name System)

DNS is a system that translates human-readable domain names into IP addresses.

People find names such as `www.example.com` easier to remember than numerical IP addresses. DNS helps devices locate the correct server.

### How DNS works

```text
User enters website name
          |
          v
Device checks its DNS cache
          |
          v
DNS resolver receives query
          |
          v
DNS system finds the IP address
          |
          v
IP address is returned
          |
          v
Browser contacts the website
```

### Features and functions

- Translates domain names into IP addresses.
- Supports different types of DNS records.
- Helps users access websites by name.
- Uses caching to reduce repeated queries.

### Common DNS records

- **A record:** Maps a domain name to an IPv4 address.
- **AAAA record:** Maps a domain name to an IPv6 address.
- **CNAME record:** Provides an alias for another domain name.
- **MX record:** Identifies mail servers for a domain.
- **NS record:** Identifies authoritative name servers.
- **TXT record:** Stores text information, often used for verification and email security.

### DNS at different layers

| Layer | What is involved |
|---|---|
| Layer 1 – Physical | Signals carry DNS messages |
| Layer 2 – Data Link | Frames carry IP packets |
| Layer 3 – Network | IP routes DNS queries and responses |
| Layer 4 – Transport | DNS commonly uses UDP port 53; TCP port 53 is also used in specific situations |
| Layer 5 – Session | Session handling is not a separate DNS layer function |
| Layer 6 – Presentation | DNS uses defined message formats and encodings |
| Layer 7 – Application | DNS performs domain-name resolution |

DNS is an **Application Layer protocol**.

### Applications

- Website access.
- Email server discovery.
- Service discovery.
- Network administration.

### Limitations

- DNS problems can prevent users from reaching websites by name.
- Incorrect DNS records can direct users to the wrong server.
- DNS queries need suitable security measures to reduce certain attacks.

---

# 5.9 DHCP (Dynamic Host Configuration Protocol)

DHCP is a network protocol that automatically provides devices with IP configuration when they join a network.

Without DHCP, an administrator may need to configure IP addresses manually on every device. DHCP makes this easier by assigning network settings automatically.

### How DHCP works: DORA process

```text
        CLIENT DEVICE
              |
              v
          DISCOVER
     Searches for DHCP server
              |
              v
           OFFER
     Server offers IP address
              |
              v
          REQUEST
     Client requests the offer
              |
              v
        ACKNOWLEDGEMENT
     Server confirms the lease
              |
              v
     DEVICE USES IP SETTINGS
```

DORA stands for:

- **Discover:** Client searches for a DHCP server.
- **Offer:** Server offers an IP address and other settings.
- **Request:** Client requests the offered address.
- **Acknowledgement:** Server confirms the assignment.

### Features and functions

DHCP can provide:
- IP address.
- Subnet mask.
- Default gateway.
- DNS server addresses.
- Lease duration.

### DHCP at different layers

| Layer | What is involved |
|---|---|
| Layer 1 – Physical | Carries the transmitted signals |
| Layer 2 – Data Link | Carries DHCP messages in local network frames |
| Layer 3 – Network | Uses IP addressing; initial IPv4 configuration commonly uses broadcast communication |
| Layer 4 – Transport | Uses UDP ports 67 and 68 for IPv4 DHCP |
| Layer 5 – Session | Does not provide a separate session-layer function |
| Layer 6 – Presentation | Uses a defined message structure |
| Layer 7 – Application | DHCP provides automatic network configuration |

DHCP is an **Application Layer protocol**.

### Applications

- Home Wi-Fi networks.
- College computer laboratories.
- Office networks.
- Public Wi-Fi hotspots.
- Large enterprise networks.

### Limitations

- A failed DHCP server can prevent devices from obtaining automatic configuration.
- Incorrect DHCP settings may assign unsuitable network details.
- Rogue DHCP servers can create security problems.

---

# 5.10 Ethernet

Ethernet is a widely used family of wired networking technologies standardised by IEEE 802.3. It defines how devices communicate over wired local area networks.

**Example:** A desktop computer connected to a switch through an Ethernet cable.

### Features and functions

- Uses frames for local network communication.
- Uses MAC addresses.
- Supports different transmission speeds.
- Commonly operates over twisted-pair and fibre-optic cables.
- Modern Ethernet commonly supports full-duplex communication.

### Ethernet layers

| Layer | What is involved |
|---|---|
| Layer 1 – Physical | Cables, connectors, electrical or optical signals |
| Layer 2 – Data Link | Ethernet frames, MAC addressing and frame checks |
| Layer 3 – Network | IP packets may be carried inside Ethernet frames |
| Layer 4 – Transport | TCP or UDP data is carried inside IP packets |
| Layer 5 | Application session handling occurs above Ethernet |
| Layer 6 | Data representation occurs above Ethernet |
| Layer 7 | Applications use network services carried over Ethernet |

Ethernet mainly defines the **Physical and Data Link layer technologies**.

### Applications

- Office networks.
- Computer laboratories.
- Data centres.
- Home wired networks.
- Enterprise LANs.

### Limitations

- Requires physical cabling.
- Cable installation can be difficult across large buildings.
- Traditional copper Ethernet links have distance limitations.

---

# 5.11 ARP (Address Resolution Protocol)

ARP is used in IPv4 local networks to discover the MAC address associated with a known IPv4 address.

For example, a computer may know that another device has the IP address `192.168.1.20`, but it needs that device's MAC address to send a local Ethernet frame.

### How ARP works

```text
Computer needs destination MAC
             |
             v
Checks its ARP cache
             |
             v
If not found, sends ARP request
             |
             v
Target device recognises its IP
             |
             v
Target sends ARP reply
             |
             v
Sender stores IP-to-MAC mapping
             |
             v
Frame can be sent locally
```

**Features and functions:**
- Resolves IPv4 addresses to MAC addresses on a local network.
- Uses request and reply messages.
- Stores mappings in an ARP cache.

**Applications:** Local IPv4 communication, Ethernet networks and home LANs.

**Limitations:** ARP is designed for local IPv4 networks and can be vulnerable to ARP spoofing. IPv6 uses Neighbour Discovery instead of ARP.

ARP is commonly described as operating between the Data Link and Network layer functions in the OSI teaching model.

---

# 5.12 Email protocols: SMTP, POP3 and IMAP

Email communication uses different protocols for sending and receiving messages.

### A. SMTP (Simple Mail Transfer Protocol)

SMTP is used to send email from a client to a mail server and between mail servers.

**Example:** Sending an email from a student's college account to a teacher.

**Common ports:** TCP 25 for server-to-server transfer, TCP 587 for message submission and TCP 465 for implicit TLS submission.

**Functions:**
- Sends outgoing messages.
- Transfers messages between mail servers.
- Supports message delivery processes.

**Limitation:** SMTP is primarily for sending email, not retrieving messages from an inbox.

### B. POP3 (Post Office Protocol version 3)

POP3 is used by email clients to retrieve messages from a mail server.

**Common ports:** TCP 110 and TCP 995 for POP3 over TLS.

**Features:**
- Downloads messages to a client.
- Can be configured to leave or remove copies on the server.
- Provides relatively simple email retrieval.

**Applications:** Basic email access, especially when users prefer local message storage.

**Limitations:** It is less suited to keeping multiple devices synchronised compared with IMAP.

### C. IMAP (Internet Message Access Protocol)

IMAP allows users to access and manage email stored on a mail server.

**Common ports:** TCP 143 and TCP 993 for IMAP over TLS.

**Features and functions:**
- Keeps messages on the server.
- Synchronises email across multiple devices.
- Supports folders and message status.
- Allows users to access the same mailbox from different devices.

**Applications:** Modern email services accessed through phones, laptops and webmail.

**Limitations:** It relies on server storage and network connectivity for many operations.

### SMTP, POP3 and IMAP compared

| Protocol | Main function | Example |
|---|---|---|
| SMTP | Sends email | Sending an email |
| POP3 | Retrieves email | Downloading messages |
| IMAP | Accesses and synchronises email | Using the same mailbox on phone and laptop |

All three are Application Layer protocols.

---

# 6. Wireless LAN (WLAN) and Wi-Fi Evolution

## 6.1 Meaning of WLAN

WLAN stands for **Wireless Local Area Network**. It is a local area network in which devices communicate using wireless signals rather than requiring a physical cable for every connection.

A WLAN is commonly based on Wi-Fi technology, which follows the IEEE 802.11 family of standards.

**Example:** A college provides wireless internet access to students throughout its library and classrooms. The connected laptops and smartphones form part of the college WLAN.

### Basic WLAN structure

```text
          INTERNET
              |
              v
            ROUTER
              |
              v
       WIRELESS ACCESS POINT
          /      |       \
         /       |        \
        v        v         v
     LAPTOP    PHONE     TABLET
        \        |         /
         \       |        /
          WIRELESS LAN
```

## 6.2 Components of a WLAN

**1. Wireless client:** A device that connects to the wireless network, such as a phone, laptop or tablet.

**2. Wireless access point:** Provides the radio connection between wireless devices and the wired LAN.

**3. Wireless router:** A device that commonly combines routing, switching and Wi-Fi access point functions.

**4. SSID (Service Set Identifier):** The name of the wireless network that users see when choosing a Wi-Fi network.

**5. Wireless network adapter:** Hardware that allows a device to send and receive Wi-Fi signals.

**6. Antenna:** Transmits and receives radio signals.

## 6.3 How WLAN works

```text
User switches on Wi-Fi
          |
          v
Device searches for available networks
          |
          v
User selects an SSID
          |
          v
Device authenticates with network
          |
          v
Device obtains IP configuration
          |
          v
Device communicates through access point
          |
          v
Data travels to local network or internet
```

## 6.4 Features of WLAN

- Provides wireless connectivity.
- Supports mobility within the coverage area.
- Allows several devices to share network access.
- Reduces the need for cables to every device.
- Can be expanded by adding more access points.
- Supports security features such as WPA2 and WPA3, depending on equipment.

## 6.5 Wi-Fi generations: Evolution from Wi-Fi 1 to Wi-Fi 7

Wi-Fi has developed over time to provide higher data rates, improved efficiency, better handling of multiple devices and more reliable wireless communication.

The Wi-Fi generation names are easier to remember than the technical IEEE standard numbers.

### Wi-Fi 1 – IEEE 802.11b

**Introduced:** 1999

**Frequency band:** 2.4 GHz

**Maximum theoretical link rate:** 11 Mbps

**Features:**
- One of the early widely used Wi-Fi standards.
- Provided wireless networking for homes and small offices.
- Used the 2.4 GHz frequency band.

**Applications:** Early home wireless networks and basic internet access.

**Limitations:** Low data rate compared with modern Wi-Fi and possible interference from other devices using 2.4 GHz.

### Wi-Fi 2 – IEEE 802.11a

**Introduced:** 1999

**Frequency band:** 5 GHz

**Maximum theoretical link rate:** 54 Mbps

**Features:**
- Used the 5 GHz band.
- Offered higher theoretical speed than 802.11b.
- Used OFDM technology.

**Applications:** Early office wireless networks and environments requiring greater capacity.

**Limitations:** Shorter coverage in many conditions compared with 2.4 GHz and less widespread early adoption.

### Wi-Fi 3 – IEEE 802.11g

**Introduced:** 2003

**Frequency band:** 2.4 GHz

**Maximum theoretical link rate:** 54 Mbps

**Features:**
- Combined higher data rates with the 2.4 GHz band.
- Was compatible with many 802.11b devices.
- Helped increase Wi-Fi use in homes.

**Applications:** Home wireless networks, laptops and early wireless broadband connections.

**Limitations:** Shared the crowded 2.4 GHz band and could be affected by interference.

### Wi-Fi 4 – IEEE 802.11n

**Introduced:** 2009

**Frequency bands:** 2.4 GHz and 5 GHz

**Maximum theoretical link rate:** Up to 600 Mbps under specified configurations.

**Features:**
- Introduced or popularised MIMO technology in Wi-Fi.
- Improved data rates and coverage.
- Supported operation in both 2.4 GHz and 5 GHz bands.
- Used channel bonding to increase capacity.

**Applications:** Home broadband, offices, wireless media streaming and laptop networks.

**Limitations:** Actual speed depends on the number of antennas, channel width, interference and connected devices.

### Wi-Fi 5 – IEEE 802.11ac

**Introduced:** 2013

**Frequency band:** 5 GHz

**Maximum theoretical link rate:** Several Gbps, with the standard's maximum commonly stated as about 6.9 Gbps under ideal configurations.

**Features:**
- Increased wireless data rates.
- Used wider channels.
- Improved MIMO capabilities.
- Supported multi-user MIMO in later Wave 2 equipment.
- Mainly operated in the 5 GHz band.

**Applications:** HD video streaming, gaming, office networks and faster home internet.

**Limitations:** Devices using only 2.4 GHz cannot use the 5 GHz-only 802.11ac features. Coverage can be affected by walls and distance.

### Wi-Fi 6 – IEEE 802.11ax

**Introduced:** 2019

**Frequency bands:** 2.4 GHz and 5 GHz

**Maximum theoretical link rate:** Up to approximately 9.6 Gbps.

**Features:**
- Uses OFDMA to improve how multiple devices share wireless resources.
- Supports improved multi-user communication.
- Uses 1024-QAM under suitable conditions.
- Improves efficiency in crowded networks.
- Supports Target Wake Time to help compatible devices manage power use.

**Applications:** Smart homes, universities, offices, public venues and networks with many connected devices.

**Limitations:** To gain the full benefits, compatible access points and client devices are needed. Real-world speed is lower than theoretical maximums.

### Wi-Fi 6E – Extension of Wi-Fi 6

Wi-Fi 6E is not a separate generation after Wi-Fi 6. It extends Wi-Fi 6 operation into the 6 GHz band where regulations allow.

**Frequency bands:** 2.4 GHz, 5 GHz and 6 GHz, depending on equipment and regional rules.

**Features:**
- Provides access to additional spectrum in the 6 GHz band.
- Can offer more channels and less congestion in suitable environments.
- Uses Wi-Fi 6 technology.

**Applications:** High-capacity home networks, offices and environments with many wireless devices.

**Limitations:** 6 GHz signals have shorter practical coverage in many environments than lower-frequency signals, and device support and permitted spectrum vary by country.

### Wi-Fi 7 – IEEE 802.11be

**Introduced commercially:** Wi-Fi 7 devices began appearing in the 2023–2024 period; certification and deployment have continued since then.

**Frequency bands:** 2.4 GHz, 5 GHz and 6 GHz, where permitted.

**Maximum theoretical link rate:** Up to approximately 46 Gbps under the standard's highest theoretical configurations.

**Features:**
- Supports wider channels up to 320 MHz in the 6 GHz band.
- Uses 4096-QAM under suitable conditions.
- Introduces Multi-Link Operation (MLO), allowing compatible devices to use multiple links.
- Improves capacity and efficiency.
- Designed to reduce latency and improve performance in demanding environments.

**Applications:** High-performance home networks, advanced gaming, high-resolution streaming, augmented and virtual reality, and enterprise wireless networks.

**Limitations:**
- Requires compatible Wi-Fi 7 routers and client devices.
- Full 320 MHz channel operation depends on access to the 6 GHz band.
- Actual speed depends on distance, interference, channel availability and device capability.

### Wi-Fi generation comparison

| Wi-Fi generation | IEEE standard | Main frequency band | Maximum theoretical rate |
|---|---|---|---|
| Wi-Fi 1 | 802.11b | 2.4 GHz | 11 Mbps |
| Wi-Fi 2 | 802.11a | 5 GHz | 54 Mbps |
| Wi-Fi 3 | 802.11g | 2.4 GHz | 54 Mbps |
| Wi-Fi 4 | 802.11n | 2.4 and 5 GHz | Up to 600 Mbps |
| Wi-Fi 5 | 802.11ac | 5 GHz | Up to about 6.9 Gbps |
| Wi-Fi 6 | 802.11ax | 2.4 and 5 GHz | Up to about 9.6 Gbps |
| Wi-Fi 6E | 802.11ax extension | 2.4, 5 and 6 GHz | Same Wi-Fi 6 standard capabilities |
| Wi-Fi 7 | 802.11be | 2.4, 5 and 6 GHz | Up to about 46 Gbps |

These are theoretical maximum rates under specific configurations, not the speeds a user should expect in everyday use.

## 6.6 Wi-Fi frequency bands

### 2.4 GHz band

- Offers wider coverage in many situations.
- Can pass through obstacles relatively well.
- Has fewer available channels in many regions.
- Can experience interference from Bluetooth and other devices.

**Example:** A smart home device connecting to a router from another room.

### 5 GHz band

- Offers more channel options in many regions.
- Can provide higher practical speeds.
- Often experiences less interference than 2.4 GHz.
- Usually has shorter range through obstacles than 2.4 GHz.

**Example:** A laptop streaming high-quality video near a Wi-Fi router.

### 6 GHz band

- Provides additional spectrum for compatible Wi-Fi 6E and Wi-Fi 7 devices.
- Can support wider channels.
- Can be useful in crowded wireless environments.
- Has shorter practical coverage through obstacles in many situations.

**Example:** A Wi-Fi 7 laptop using a 6 GHz connection near a compatible access point.

## 6.7 Wi-Fi security

Wireless networks need security because signals travel through the air and may be detected by nearby devices.

**WEP:** An old wireless security method that is now considered insecure.

**WPA:** Improved security compared with WEP, but it has been superseded.

**WPA2:** Widely used Wi-Fi security based on strong encryption when configured properly.

**WPA3:** A newer security standard that improves protection, including stronger password-based authentication methods.

**Good practice:** Use WPA2-AES or WPA3 where supported, set a strong Wi-Fi password, update router firmware and avoid leaving the network open to everyone.

## 6.8 Advantages of WLAN

- Users can connect without physical cables.
- Devices can move within the coverage area.
- New devices can be added easily.
- Useful in places where cable installation is difficult.
- Several users can share one internet connection.

## 6.9 Limitations of WLAN

- Wireless signals can be affected by walls and distance.
- Interference can reduce network speed.
- Wireless networks require suitable security settings.
- Performance may decrease when too many devices use the same access point.
- Coverage may require multiple access points in large buildings.

## 6.10 Real-world applications of WLAN

- **Education:** Students connect laptops and tablets to college Wi-Fi.
- **Healthcare:** Staff use wireless devices to access hospital systems.
- **Business:** Employees connect laptops and phones to office networks.
- **Hospitality:** Hotels provide wireless internet to guests.
- **Smart homes:** Smart televisions, cameras and appliances connect through Wi-Fi.
- **Public spaces:** Airports, railway stations and libraries provide public wireless access.

---

# 7. How All Network Components Work Together

All the components discussed above work together whenever information travels across a network.

Consider a student opening a college website on a laptop connected to Wi-Fi.

### Complete communication flow

```text
        STUDENT OPENS WEBSITE
                  |
                  v
          LAPTOP (NODE)
                  |
                  v
       CONNECTS TO WI-FI ACCESS POINT
                  |
                  v
       OBTAINS IP SETTINGS THROUGH DHCP
                  |
                  v
       DNS FINDS THE WEBSITE IP ADDRESS
                  |
                  v
       DATA IS PREPARED BY APPLICATION
                  |
                  v
       TCP OR QUIC HANDLES TRANSPORT
                  |
                  v
       IP ADDRESSES AND ROUTES PACKETS
                  |
                  v
       WI-FI CARRIES DATA TO ACCESS POINT
                  |
                  v
       SWITCH / ROUTER FORWARDS TRAFFIC
                  |
                  v
             INTERNET
                  |
                  v
          WEBSITE SERVER
                  |
                  v
       RESPONSE RETURNS TO LAPTOP
                  |
                  v
          WEBPAGE IS DISPLAYED
```

### Understanding the example

1. The laptop is the **node** that requests the webpage.
2. Wi-Fi provides the **wireless link** between the laptop and access point.
3. The access point connects the laptop to the local network.
4. DHCP can provide the laptop with an IP address and other network settings.
5. DNS helps find the IP address associated with the website's domain name.
6. HTTP or HTTPS handles the web request and response.
7. TCP or QUIC provides the transport function, depending on the HTTP version.
8. IP helps packets travel between different networks.
9. Switches and routers forward traffic towards its destination.
10. The web server processes the request and sends the webpage back.

This shows that network communication is not performed by one component alone. Nodes, links, intermediary devices and protocols all have different responsibilities, but they work together to complete the communication process.

---

# 8. Important Networking Terms

| Term | Meaning |
|---|---|
| Network | A group of connected devices that communicate and share resources |
| Node | A device that participates in network communication |
| Link | A communication path between network devices |
| NIC | Network Interface Card; hardware that connects a device to a network |
| MAC address | Link-layer address associated with a network interface |
| IP address | Logical address used for communication across IP networks |
| Hostname | Readable name assigned to a device |
| Port | Number identifying an application or service endpoint |
| Bandwidth | Maximum data-carrying capacity of a link |
| Throughput | Actual successful data transfer rate |
| Latency | Time taken for data to travel from source to destination |
| Jitter | Variation in packet delay |
| Packet | A unit of data carried by a network-layer protocol |
| Frame | A unit of data used at the Data Link Layer |
| Protocol | Rules used for network communication |
| Router | Device that forwards packets between IP networks |
| Switch | Device that forwards frames using MAC addresses |
| Hub | Device that repeats signals to all connected ports |
| Gateway | Device or system connecting different networks or systems |
| Firewall | Security system that filters network traffic |
| Access Point | Device that connects wireless clients to a LAN |
| WLAN | Wireless Local Area Network |
| SSID | Name of a wireless network |
| DHCP | Protocol that automatically provides network configuration |
| DNS | System that translates domain names into IP addresses |
| TCP | Reliable, connection-oriented transport protocol |
| UDP | Connectionless transport protocol with low overhead |
| IP | Protocol responsible for logical addressing and packet forwarding |
| HTTP | Protocol used for web communication |
| HTTPS | HTTP protected using TLS |
| Ethernet | Family of wired LAN technologies |
| ARP | Protocol used to discover MAC addresses for IPv4 local communication |

