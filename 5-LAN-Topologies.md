# COMPUTER NETWORKS – 

## TABLE OF CONTENTS

1. Introduction to Networks
2. Basic Idea Behind Communication
3. Evolution and History of Computer Networks
4. Computer Networks – Meaning and Working
5. Basic Components of a Computer Network
6. Types of Computer Networks
7. LAN (Local Area Network) – Detailed Explanation
8. Network Topologies
   - Bus Topology
   - Star Topology
   - Mesh Topology
9. Comparison Between Bus, Star and Mesh Topologies
10. Modern Networking Technologies
11. Important Networking Terms and Definitions

---

# 1. INTRODUCTION TO NETWORKS

Before understanding computer networks, it is important to understand why the concept of networking was introduced.

In the beginning, computers were mostly independent machines. They could perform calculations, process information and store data, but sharing information between two different computers was not easy.

For example, imagine a college where every department has its own computer. If the examination department wants to send a file to the accounts department, it would need an external method, such as a storage device.

This was not very convenient.

People needed a system through which computers could communicate with each other, exchange information and share resources. This requirement led to the development of computer networking.

**Definition:** A network is a group of two or more connected devices that can communicate and share information or resources with one another.

In simple words, networking means connecting different devices so that they can exchange information.

# 2. THE BASIC IDEA BEHIND COMMUNICATION

The idea of networking did not begin with computers. Humans have always needed ways to communicate information over distances.

Let's understand how communication developed step by step.

### 2.1 Early Communication

In ancient times, people communicated through:
- Spoken messages.
- Written letters.
- Messengers.
- Smoke signals.
- Drums and other sound signals.

These methods were useful, but they were slow and had limitations when distances increased.

### 2.2 Telegraph System (1830s–1840s)

The telegraph was one of the earliest technologies that allowed messages to travel over long distances using electrical signals.

It commonly used Morse code, a system of representing letters and numbers through combinations of dots and dashes.

**Morse Code:** A communication system in which letters and numbers are represented using short and long signals.

### 2.3 Telephone (1876)

The invention of the telephone made it possible for people to communicate through voice over long distances.

Unlike the telegraph, which transmitted coded messages, the telephone transmitted human speech.

### 2.4 Radio Communication (Late 19th and Early 20th Century)

Radio technology made wireless communication possible.

**Wireless Communication:** Transmitting information without using physical cables, generally through electromagnetic waves.

This development later became important for wireless computer networks, Wi-Fi and mobile communication.

These early technologies created the foundation for modern communication systems.

# 3. EVOLUTION AND HISTORY OF COMPUTER NETWORKS

Computer networking developed gradually. It did not appear in its present form all at once.

The following timeline explains its major developments in chronological order.

### 3.1 Early Computers (1940s–1950s)

Early computers were large, expensive machines. They were mainly used by governments, research institutions and large organisations.

Most computers worked independently, and exchanging information between them was difficult.

### 3.2 Time-Sharing Systems (1950s–1960s)

As computers became more advanced, researchers developed time-sharing systems.

**Time-Sharing:** A method in which multiple users can use the resources of one computer by sharing its processing time.

This made computing more accessible to several users, although it was not the same as today's computer networking.

### 3.3 ARPANET (1969)

One of the most important milestones in networking was the development of ARPANET.

**ARPANET:** Advanced Research Projects Agency Network.

It was an early packet-switching network developed with support from the US Department of Defense's ARPA.

Its main purpose was to connect research computers at different universities and institutions.

**Packet Switching:** A method of sending information by dividing it into smaller units called packets. These packets travel through a network and are reassembled at their destination.

ARPANET became an important foundation for the development of the modern Internet.

### 3.4 Development of Ethernet (1970s)

Ethernet was developed at Xerox PARC in the 1970s.

It provided a practical way to connect computers within a local area.

**Ethernet:** A widely used technology for connecting devices in wired local area networks.

It helped make LANs useful in offices, laboratories and educational institutions.

### 3.5 TCP/IP Protocol (1980s)

As different networks developed, there was a need for a common communication system.

This led to the development and adoption of TCP/IP.

**TCP/IP:** Transmission Control Protocol/Internet Protocol.

It is a collection of communication protocols that allows different devices and networks to exchange information.

On 1 January 1983, ARPANET officially transitioned to TCP/IP, an important milestone in the development of the Internet.

### 3.6 World Wide Web (1989–1991)

The World Wide Web was invented by Tim Berners-Lee.

It made it easier for people to access and share information through linked web pages.

**World Wide Web (WWW):** A system of interconnected web pages and online resources that can be accessed through the Internet.

Remember that the Internet and the World Wide Web are not exactly the same. The Internet is the global network infrastructure, while the Web is one of the services that operates on it.

### 3.7 Wi-Fi Technology (Late 1990s)

Wi-Fi made it possible to connect devices to networks wirelessly.

Instead of requiring a physical cable for every connection, devices could communicate using radio waves.

It became widely used in homes, schools, offices and public places.

### 3.8 Broadband and Mobile Internet (2000s)

Broadband connections provided faster Internet access than traditional dial-up connections.

Mobile networks also developed, allowing people to access the Internet through mobile phones.

### 3.9 Cloud Computing and IoT (2010s)

Two important developments during this period were cloud computing and the Internet of Things.

**Cloud Computing:** A technology that allows users to store data, run applications and use computing resources through remote servers over a network.

**Internet of Things (IoT):** A system in which physical devices, such as smart watches, sensors, cameras and home appliances, connect to the Internet and exchange data.

### 3.10 Modern Networking (2020s and Beyond)

Modern networks are becoming faster, smarter and more automated.

Some important developments include:

- **5G:** Fifth-generation mobile network technology, providing high-speed communication and support for many connected devices.
- **Wi-Fi 6 and Wi-Fi 7:** Newer generations of wireless networking technology designed to improve speed, capacity and efficiency.
- **Artificial Intelligence in Networking:** AI is being used to monitor network performance, detect unusual activities and help manage network problems.
- **Software-Defined Networking (SDN):** An approach that allows network management and control to be handled through software.
- **Edge Computing:** Processing data closer to the devices that generate it instead of sending everything to a distant data centre.
- **6G Research:** The next generation of mobile communication is being researched, with the aim of improving connectivity and supporting new applications.

Thus, networking has developed from simple communication methods into a worldwide system connecting billions of devices.

# 4. COMPUTER NETWORKS – MEANING AND WORKING

## 4.1 Definition

A computer network is a group of two or more computers or other electronic devices connected through wired or wireless communication channels to exchange data and share resources.

A network allows users to:

1. Share files and documents.
2. Share printers and other hardware.
3. Communicate through email and messaging.
4. Access the Internet.
5. Share software and information.
6. Work together from different locations.

**Example:** When several computers in a computer laboratory are connected to the same network, students can share files and access a common printer.

## 4.2 How Does a Computer Network Work?

A computer network works by sending information from one device to another through a communication medium.

Let's understand it with a simple example.

Suppose Computer A wants to send a file to Computer B.

1. Computer A prepares the information.
2. The information is divided into smaller packets when packet-based communication is used.
3. These packets are sent through a network medium.
4. Network devices help forward the information towards its destination.
5. Computer B receives the packets and reassembles the information.

**Flowchart:**

```text
       Computer A (Sender)
               |
               v
        Data is prepared
               |
               v
       Data is transmitted
               |
               v
     Communication Medium
               |
               v
       Computer B (Receiver)
               |
               v
       Information received
```

## 4.3 Characteristics of a Computer Network

- Connects two or more devices.
- Allows information sharing.
- Supports communication between users.
- Enables hardware and software resource sharing.
- Can use wired or wireless connections.
- Can cover a small or very large geographical area.

## 4.4 Advantages of Computer Networks

- Easy sharing of files and information.
- Saves time and resources.
- Allows communication over long distances.
- Makes collaboration easier.
- Provides shared access to hardware and software.
- Supports centralised data storage.

## 4.5 Limitations of Computer Networks

- Installation and maintenance can be expensive.
- Security threats can affect connected devices.
- Network failures may interrupt communication.
- Viruses and malware can spread through networks.
- Technical knowledge may be required to manage large networks.

## 4.6 Real-Life Applications

Computer networks are used in almost every field:

- **Education:** Online classes and digital libraries.
- **Banking:** Online transactions and ATM communication.
- **Healthcare:** Sharing medical records and reports.
- **Business:** Communication between employees and departments.
- **Entertainment:** Online gaming and video streaming.
- **Government:** Digital services and online information systems.

# 5. BASIC COMPONENTS OF A COMPUTER NETWORK

A computer network consists of several important components that work together to make communication possible.

## 5.1 Computer or Node

A **node** is any device connected to a network.

Examples include computers, laptops, printers, servers and smartphones.

**Characteristics:**
- Every node can be identified within a network.
- It may send, receive or forward information.
- Different types of devices can act as nodes.

**Applications:** Computers in laboratories, smartphones connected to Wi-Fi and printers connected to office networks.

## 5.2 Server

A **server** is a computer or software system that provides services or resources to other devices on a network.

For example, a file server stores files that can be accessed by other computers.

**Characteristics:**
- Provides shared resources.
- Can store and manage data centrally.
- May serve multiple users at the same time.

**Advantages:** Centralised storage, easier administration and convenient resource sharing.

**Limitations:** Server failure can interrupt services, and maintaining a server may be costly.

**Applications:** Banking systems, college databases, websites and company file storage.

## 5.3 Client

A **client** is a computer or application that requests services or information from a server.

For example, when a student opens a college website, their browser acts as a client requesting information from the website's server.

**Applications:** Web browsers, email applications and online banking applications.

## 5.4 Network Interface Card (NIC)

A Network Interface Card is a hardware component that allows a device to connect to a network.

It may support a wired Ethernet connection or wireless networking.

**Characteristics:**
- Provides network connectivity.
- Has a unique hardware address called a MAC address.
- May be built into the motherboard or installed separately.

**Applications:** Connecting desktop computers to Ethernet networks and laptops to wireless networks.

## 5.5 Transmission Media

Transmission media are the paths through which information travels.

They are mainly divided into two types.

**A. Guided Media**

Guided media uses physical cables to transmit information.

Examples:
- Twisted-pair cable.
- Coaxial cable.
- Optical fibre cable.

**B. Unguided Media**

Unguided media transmits information without physical cables, using electromagnetic signals.

Examples:
- Radio waves.
- Microwaves.
- Infrared signals.

**Applications:** Ethernet connections, fibre-optic Internet, Wi-Fi and mobile communication.

## 5.6 Switch

A switch connects multiple devices within a LAN and forwards data to the appropriate device using hardware addresses.

**Characteristics:**
- Connects several devices.
- Reduces unnecessary data transmission between devices.
- Commonly operates at the Data Link Layer of the OSI model.

**Advantages:** Efficient communication, good LAN performance and easy network expansion.

**Limitations:** Requires configuration and management in larger networks. Failure of a central switch can interrupt connected devices.

**Applications:** Computer laboratories, office networks and school networks.

## 5.7 Router

A router connects different networks and forwards data between them.

For example, a home router connects a home network to the Internet.

**Characteristics:**
- Connects separate networks.
- Uses IP addresses to forward packets.
- Selects suitable routes for data transmission.

**Advantages:** Allows communication between networks and provides access to the Internet.

**Limitations:** Incorrect configuration or router failure can interrupt network connectivity.

**Applications:** Home Internet connections, offices and large organisational networks.

## 5.8 Modem

A modem converts signals into a form suitable for transmission over a particular communication connection. It is commonly used to connect a home or office network to an Internet service provider.

**Modem:** Modulator-Demodulator.

**Applications:** Broadband Internet connections, cable Internet and certain fibre or telephone-based Internet services.

# 6. TYPES OF COMPUTER NETWORKS

Computer networks can be classified according to the geographical area they cover.

## 6.1 PAN (Personal Area Network)

**Definition:** PAN stands for Personal Area Network. It covers a very small area around an individual.

**Characteristics:**
- Covers a short distance.
- Connects personal devices.
- Commonly uses Bluetooth or other short-range technologies.

**Advantages:**
- Easy to establish.
- Convenient for connecting personal devices.
- Usually requires little infrastructure.

**Limitations:**
- Limited coverage area.
- Generally supports fewer devices.
- Some technologies have lower data transfer speeds than LAN connections.

**Real-Life Applications:**
- Connecting a smartphone to wireless earbuds.
- Connecting a laptop to a Bluetooth mouse.
- Sharing data between personal devices.

## 6.2 LAN (Local Area Network)

LAN stands for Local Area Network.

It connects computers and other devices within a limited geographical area, such as a room, office, school or computer laboratory.

**Characteristics:**
- Covers a limited geographical area.
- Usually provides high-speed communication.
- Commonly owned and managed by one person or organisation.
- Supports resource sharing.

**Advantages:**
- Fast communication.
- Easy file sharing.
- Shared access to printers and other devices.
- Convenient management of information.

**Limitations:**
- Limited geographical coverage.
- Requires installation and maintenance.
- Security problems can affect connected devices.

**Real-Life Applications:** Computer laboratories, offices, banks, schools and homes.

## 6.3 MAN (Metropolitan Area Network)

MAN stands for Metropolitan Area Network.

It connects multiple networks across a city or a large urban area.

**Characteristics:**
- Covers a larger area than LAN.
- Can connect multiple buildings and offices.
- Often uses high-speed fibre-optic connections.

**Advantages:**
- Connects different locations within a city.
- Supports communication between branches.
- Allows centralised services across multiple sites.

**Limitations:**
- More expensive than a small LAN.
- Requires specialised management.
- Network maintenance can be complex.

**Real-Life Applications:**
- Connecting university campuses across a city.
- Connecting bank branches within a metropolitan area.
- City-wide communication infrastructure.

## 6.4 WAN (Wide Area Network)

WAN stands for Wide Area Network.

It covers a large geographical area, such as countries or continents.

The Internet is the largest and most well-known example of a WAN.

**Characteristics:**
- Covers large geographical areas.
- Connects multiple LANs and other networks.
- Uses communication links such as fibre optics, satellites and leased lines.

**Advantages:**
- Supports communication over long distances.
- Connects offices in different cities and countries.
- Allows access to information from different locations.

**Limitations:**
- Expensive infrastructure and maintenance.
- More complex security management.
- Communication delays may be higher than in a local network.

**Real-Life Applications:**
- International banking networks.
- Multinational companies.
- Airline reservation systems.
- The Internet.

# 7. LAN (LOCAL AREA NETWORK) – DETAILED EXPLANATION

LAN is one of the most commonly used types of computer networks, especially in educational institutions, offices and homes.

## 7.1 Definition

A Local Area Network (LAN) is a computer network that connects multiple computers and devices within a small geographical area, such as a home, school, office, laboratory or building.

The main purpose of a LAN is to allow connected devices to communicate and share resources easily.

**Example:**

Imagine a computer laboratory containing 30 computers. All computers are connected to one network so that students can share files, access the Internet and use a common printer.

This arrangement is an example of a LAN.

## 7.2 Characteristics of LAN

1. **Limited Coverage Area:** A LAN usually covers a small area, such as a building or campus.
2. **High Speed:** LANs generally provide fast data transmission within the local network.
3. **Resource Sharing:** Users can share printers, files, applications and Internet connections.
4. **Private Ownership:** LANs are commonly owned and managed by an individual, institution or organisation.
5. **Low Communication Delay:** Communication within a properly designed LAN generally has low delay.
6. **Easy Management:** A small LAN is usually easier to manage than a large network.

## 7.3 Advantages of LAN

1. Fast communication between connected devices.
2. Easy sharing of files and documents.
3. Sharing of expensive hardware such as printers.
4. Centralised storage and management of information.
5. Reduced cost when multiple users share resources.
6. Convenient communication between users.

## 7.4 Limitations of LAN

1. Its coverage area is limited.
2. Initial installation may require cables and networking devices.
3. Network failure can affect multiple connected users.
4. Poor security settings may allow unauthorised access.
5. Network maintenance requires technical knowledge.

## 7.5 Real-Life Applications of LAN

LANs are commonly used in:

- **Schools and Colleges:** Connecting computers in laboratories and libraries.
- **Banks:** Connecting computers used by employees to access shared information.
- **Offices:** Sharing documents, printers and other resources.
- **Hospitals:** Accessing patient records and reports through connected systems.
- **Libraries:** Managing digital resources and library databases.
- **Homes:** Connecting smartphones, laptops, televisions and printers to a home network.
- **Small Businesses:** Connecting billing systems, computers and storage devices.

## 7.6 Basic LAN Diagram

```text
           COMPUTER LABORATORY

       [PC 1]     [PC 2]     [PC 3]
          \         |         /
           \        |        /
            \       |       /
              [ NETWORK SWITCH ]
                     |
                     |
                [ ROUTER ]
                     |
                     |
                  INTERNET
```

**Explanation:**

All computers are connected to a central switch. The switch allows them to communicate with one another, while the router provides a connection to another network, such as the Internet.

# 8. NETWORK TOPOLOGIES

Before studying different LAN topologies, we need to understand what topology means.

**Network Topology:** Network topology refers to the physical or logical arrangement of devices and connections within a network.

In simple words, topology explains how computers and other devices are connected to one another.

There are different types of network topologies, but here we will study three important ones:

1. Bus Topology
2. Star Topology
3. Mesh Topology

## 8.1 BUS TOPOLOGY

### Definition

Bus topology is a type of network topology in which all computers and devices are connected to a single main cable called the backbone cable.

The backbone cable acts as the common communication path for all connected devices.

When a device sends data, the data travels along the main cable. All connected devices can receive the signal, but only the device with the matching destination address accepts the data.

**Backbone Cable:** The main cable that connects all devices in a bus topology.

### Diagram of Bus Topology

```text
   [PC 1]       [PC 2]       [PC 3]       [PC 4]
      |            |            |            |
================================================
               BACKBONE CABLE
================================================
```

The main idea is that all devices share one common communication cable.

**Note:** In a traditional bus network, terminators are fitted at both ends of the backbone cable to prevent signals from reflecting back along the cable.

### How Bus Topology Works

1. All computers are connected to a common backbone cable.
2. When one computer sends data, the signal travels along the cable.
3. The other connected computers can detect the signal.
4. The computer whose address matches the destination accepts the data.
5. Terminators at both ends help prevent signal reflection.

### Characteristics of Bus Topology

- All devices share one main communication cable.
- Data travels along the backbone.
- Terminators are used at both ends.
- There is no central switch or hub.
- The entire network depends on the condition of the backbone cable.

### Advantages of Bus Topology

1. **Easy Installation:** It is relatively simple to install in a small network.
2. **Less Cable Required:** It uses a single main cable, so less cable may be needed.
3. **Low Initial Cost:** It can be economical for small and simple networks.
4. **No Central Device Required:** It does not need a central switch or hub.
5. **Suitable for Small Networks:** It can be useful in simple networking arrangements.

### Limitations of Bus Topology

1. **Backbone Failure:** If the main cable fails, the entire network may stop working.
2. **Limited Cable Length:** The main cable cannot be extended indefinitely.
3. **Performance Issues:** As more devices communicate, network performance can decrease.
4. **Difficult Troubleshooting:** Finding a fault in the main cable can be difficult.
5. **Data Collisions:** When multiple devices transmit at the same time, their signals may collide.
6. **Limited Expansion:** Adding more devices can make the network harder to manage.

**Data Collision:** A situation in which two or more devices transmit data simultaneously over a shared communication medium, causing the transmissions to interfere.

### Real-Life Applications of Bus Topology

- Older Ethernet LAN installations.
- Small experimental networking setups.
- Certain industrial communication systems.
- Some embedded communication arrangements.

Bus topology was commonly used in older Ethernet networks, but it is rarely used for modern office LANs.

## 8.2 STAR TOPOLOGY

### Definition

Star topology is a network topology in which all computers and devices are connected to one central networking device.

The central device is generally a switch, although older networks sometimes used a hub.

Each computer has its own separate connection to the central device.

**Central Device:** A device that connects the computers and manages communication between them.

**Hub:** A basic networking device that sends received data to all connected ports.

**Switch:** A networking device that forwards data to the intended device or devices based on their hardware addresses.

### Diagram of Star Topology

```text
                   [PC 1]
                      |
                      |
        [PC 2] --- [SWITCH] --- [PC 3]
                      |
                      |
                   [PC 4]
                      |
                      |
                   [PC 5]
```

The central switch acts as the connection point for all computers.

### How Star Topology Works

1. Every computer is connected to a central switch or hub.
2. When a computer wants to send data, it sends the information to the central device.
3. The central device forwards the data towards the destination computer.
4. The destination computer receives the information.

### Characteristics of Star Topology

- All devices are connected to a central device.
- Each computer has its own separate cable connection.
- Communication passes through the central device.
- Failure of one individual cable usually affects only one device.
- The central switch or hub is an important part of the network.

### Advantages of Star Topology

1. **Easy Installation:** Connecting devices to a central switch is straightforward.
2. **Easy Troubleshooting:** If one cable or computer fails, it is usually easy to identify the problem.
3. **Independent Connections:** Failure of one individual cable generally does not affect other computers.
4. **Easy Expansion:** New devices can be added by connecting them to the central switch.
5. **Good Performance:** Modern switches provide efficient communication between connected devices.
6. **Better Management:** Network administration is easier because all connections meet at one central point.

### Limitations of Star Topology

1. **Central Device Failure:** If the central switch fails, communication between connected devices may stop.
2. **More Cable Required:** Each computer needs an individual connection to the central device.
3. **Higher Installation Cost:** The central device and individual cables increase the initial cost.
4. **Limited by Central Device Capacity:** The number of connections depends on the available ports and capacity of the central device.
5. **Centralised Dependency:** Network communication depends heavily on the central device.

### Real-Life Applications of Star Topology

- Computer laboratories in schools and colleges.
- Office networks.
- Banks and business organisations.
- Home networks.
- Hospital computer systems.
- Small and medium-sized businesses.

Star topology is widely used in modern LANs because it is relatively easy to install, manage and expand.

## 8.3 MESH TOPOLOGY

### Definition

Mesh topology is a type of network topology in which devices are connected through multiple communication links.

In a full mesh topology, every device has a direct connection to every other device.

In a partial mesh topology, only some devices have direct connections to multiple other devices.

This arrangement provides alternative paths for data transmission.

**Alternative Path:** Another available route through which data can travel if the original route becomes unavailable.

### Types of Mesh Topology

**A. Full Mesh Topology**

In a full mesh topology, every device is directly connected to every other device.

For example, if there are four computers, each computer has a direct connection to the other three computers.

```text
       [A] -------- [B]
        |\          /|
        | \        / |
        |  \      /  |
        |   \    /   |
        |    \  /    |
        |    / \     |
        |   /   \    |
        |  /     \   |
       [C] -------- [D]
```

The main concept is that every computer has a direct connection to every other computer.

**B. Partial Mesh Topology**

In partial mesh topology, only selected devices are directly connected to multiple other devices.

Some devices may have several connections, while others may have only one or two.

```text
[A] -------- [B]
 |             |
 |             |
[C] -------- [D]
               |
               |
              [E]
```

Unlike full mesh, not every computer is connected directly to every other computer.

### How Mesh Topology Works

1. Devices are connected through multiple links.
2. A device sends data through an available connection.
3. Data travels towards its destination.
4. If one link fails, another available route may be used.
5. This provides better network reliability.

### Characteristics of Mesh Topology

- Devices have multiple communication links.
- Full mesh provides a direct connection between every pair of devices.
- Partial mesh connects selected devices through multiple paths.
- Multiple routes can provide better fault tolerance.
- It requires more connections than bus and star topologies.

### Advantages of Mesh Topology

1. **High Reliability:** Multiple connections provide alternative communication paths.
2. **Fault Tolerance:** Failure of one connection does not necessarily stop the entire network.
3. **Better Availability:** Devices can continue communicating through alternative routes.
4. **Dedicated Connections:** In a full mesh, each pair of devices has a direct communication link.
5. **Better Fault Isolation:** Problems can often be identified by examining individual connections.

**Fault Tolerance:** The ability of a system to continue operating even when some of its components fail.

**Reliability:** The ability of a network to perform its intended functions consistently.

### Limitations of Mesh Topology

1. **High Cost:** A full mesh requires many cables and network interfaces.
2. **Complex Installation:** Connecting every device to every other device can be difficult.
3. **Difficult Maintenance:** Managing a large number of connections requires more effort.
4. **More Hardware Required:** Each device needs enough network interfaces to support its connections.
5. **Not Suitable for Every Network:** It may be unnecessary and expensive for small networks.

### Real-Life Applications of Mesh Topology

- Wireless mesh networks.
- Communication infrastructure.
- Some large enterprise networks.
- Critical communication systems.
- Networks that require alternative communication paths.

Mesh topology is especially useful where reliable communication is important.

# 9. COMPARISON BETWEEN BUS, STAR AND MESH TOPOLOGIES

After studying all three topologies individually, let's compare them to understand their differences.

| Feature | Bus | Star | Mesh |
|---|---|---|---|
| Structure | Single main cable | Central device | Multiple connections |
| Main Component | Backbone cable | Switch or hub | Multiple links |
| Cost | Low initially | Moderate | High |
| Installation | Simple for small networks | Easy | Complex |
| Reliability | Lower | Good, but central device is critical | High |
| Cable Requirement | Less | More than bus | Very high in full mesh |
| Expansion | Limited | Easy | Difficult |
| Fault Detection | Difficult | Easier | More complex |
| Common Use | Older LANs | Modern LANs | High-reliability networks |

## 9.1 Which Topology Is Better and Why?

There is no single topology that is best for every situation. The choice depends on cost, network size, performance and reliability requirements.

- **Bus Topology:** Suitable for simple arrangements where low initial cost and less cabling are important.
- **Star Topology:** Suitable for offices, schools and computer laboratories because it is easy to manage and expand.
- **Mesh Topology:** Suitable for systems where communication must continue even if one or more connections fail.

For most modern wired LANs, star topology is commonly preferred because of its practical balance between cost, performance and maintenance.

# 10. MODERN NETWORKING TECHNOLOGIES

After understanding LAN and its topologies, it is useful to see how modern networking has developed.

Today's networking is not limited to connecting desktop computers through cables. It includes wireless communication, mobile networks, cloud systems and smart devices.

## 10.1 Ethernet

**Definition:** Ethernet is a technology used for wired LAN communication. It allows computers and other devices to exchange data through network cables.

**Characteristics:**
- Uses physical cables.
- Provides reliable communication.
- Commonly uses switches.
- Supports different transmission speeds.

**Advantages:** Stable connection, high speed and low interference compared with many wireless connections.

**Limitations:** Requires physical cabling and limits device mobility.

**Applications:** Offices, computer laboratories, data centres and home wired networks.

## 10.2 Wi-Fi

**Definition:** Wi-Fi is a wireless networking technology that allows devices to connect to a local network using radio signals.

**Characteristics:**
- Does not require a physical network cable for each device.
- Uses wireless access points or routers.
- Supports multiple connected devices.
- Provides mobility within the coverage area.

**Advantages:** Convenient, flexible and easy to use with portable devices.

**Limitations:** Signal strength can decrease with distance and obstacles. Wireless networks also require proper security settings.

**Applications:** Homes, schools, offices, airports, hotels and public places.

## 10.3 Bluetooth

**Definition:** Bluetooth is a short-range wireless communication technology used to connect devices such as phones, keyboards, speakers and headphones.

**Characteristics:**
- Uses radio communication.
- Designed for short distances.
- Generally consumes relatively little power.
- Connects nearby devices.

**Advantages:** Convenient, wireless and useful for personal devices.

**Limitations:** Limited range and generally lower data transfer capacity than modern Wi-Fi.

**Applications:** Wireless earbuds, smart watches, speakers, keyboards and computer mice.

## 10.4 Fibre Optic Networking

**Definition:** Fibre optic cables transmit information using light signals.

They provide high-speed data transmission and are widely used in Internet infrastructure and long-distance communication.

**Characteristics:**
- Uses light instead of electrical signals.
- Supports high bandwidth.
- Can transmit data over long distances.
- Is less affected by electromagnetic interference.

**Advantages:** Very high speed, long-distance transmission and reliable communication.

**Limitations:** Installation and repair may require specialised equipment and technical expertise.

**Applications:** High-speed broadband Internet, undersea communication cables, telecommunications and data centres.

## 10.5 5G Networks

**Definition:** 5G is the fifth generation of mobile communication technology.

It improves mobile connectivity and supports applications such as high-speed Internet access, connected devices and advanced communication systems.

**Characteristics:**
- Higher potential data speeds.
- Improved network capacity.
- Lower latency in suitable conditions.
- Supports a large number of connected devices.

**Advantages:** Faster mobile communication and better support for advanced connected services.

**Limitations:** Coverage and performance vary by location, frequency and infrastructure. Deployment can also be expensive.

**Applications:** Mobile Internet, smart cities, connected vehicles and industrial automation.

## 10.6 Cloud Networking

**Definition:** Cloud networking uses network-based infrastructure and services to connect users, applications and computing resources.

It helps organisations manage resources without depending entirely on physical equipment at their own location.

**Characteristics:**
- Uses remote computing infrastructure.
- Supports access from different locations.
- Can scale according to requirements.
- Allows centralised management of services.

**Advantages:** Flexibility, scalability and convenient access to resources.

**Limitations:** Depends on network connectivity and requires careful security and access management.

**Applications:** Online storage, web applications, remote working and business software.

## 10.7 Internet of Things (IoT)

**Definition:** IoT connects everyday physical devices to networks so that they can exchange information.

For example, a smart home system can connect lights, cameras, sensors and appliances.

**Characteristics:**
- Connects physical objects to networks.
- Uses sensors to collect information.
- Allows devices to exchange data.
- Can support automatic actions.

**Advantages:** Automation, remote monitoring and improved convenience.

**Limitations:** Privacy concerns, security risks and dependence on network connectivity.

**Applications:** Smart homes, healthcare monitoring, agriculture, industrial systems and smart cities.

## 10.8 Artificial Intelligence in Networking

**Definition:** Artificial intelligence in networking refers to the use of AI techniques to monitor, analyse and manage network operations.

**Characteristics:**
- Analyses network traffic.
- Identifies unusual behaviour.
- Helps detect security threats.
- Supports automated network management.

**Advantages:** Faster fault detection, improved monitoring and more efficient network management.

**Limitations:** Requires good-quality data, computing resources and careful human supervision.

**Applications:** Network security, traffic management, fault detection and data centre operations.

## 10.9 Software-Defined Networking (SDN)

**Definition:** Software-Defined Networking is an approach in which network control and management are handled through software, allowing administrators to manage network behaviour more flexibly.

**Characteristics:**
- Separates network control from data forwarding.
- Supports centralised network management.
- Allows programmable network configuration.

**Advantages:** Flexible management, easier automation and efficient network control.

**Limitations:** Requires specialised knowledge and careful security management.

**Applications:** Data centres, cloud infrastructure and large enterprise networks.

## 10.10 Edge Computing

**Definition:** Edge computing is a method of processing data closer to the devices that generate it instead of sending all information to a distant central data centre.

**Characteristics:**
- Processes data near its source.
- Reduces the need to transfer every piece of data to a remote server.
- Can reduce response time.

**Advantages:** Lower latency, faster local processing and reduced network traffic.

**Limitations:** Requires computing resources at multiple locations and can make management more complex.

**Applications:** Smart factories, connected vehicles, security cameras and IoT systems.

## 10.11 6G Research

**Definition:** 6G refers to the next generation of mobile communication technology currently under research and development.

It is expected to build on 5G and support future communication requirements.

**Characteristics and Expected Goals:**
- Higher communication capacity.
- More advanced connectivity.
- Integration of sensing and communication.
- Support for future intelligent applications.

**Limitations:** It is not yet a commercially established worldwide mobile network standard. Its technical requirements and deployment are still developing.

**Potential Applications:** Advanced robotics, intelligent transportation, immersive communication and future smart infrastructure.

# 11. IMPORTANT NETWORKING TERMS AND DEFINITIONS

The following table contains important technical words used throughout the chapter. These definitions are useful for understanding concepts as well as preparing short-answer examination questions.

| Term | Definition |
|---|---|
| Network | A group of connected devices that communicate and share resources. |
| Node | Any device connected to a network. |
| LAN | Local Area Network; a network covering a limited geographical area. |
| WAN | Wide Area Network; a network covering a large geographical area. |
| MAN | Metropolitan Area Network; a network covering a city or metropolitan area. |
| PAN | Personal Area Network; a network covering an individual's personal space. |
| Topology | The arrangement of devices and connections in a network. |
| Backbone | The main communication cable or connection in a network. |
| Packet | A small unit of data transmitted through a packet-based network. |
| Protocol | A set of rules governing communication between devices. |
| Server | A system that provides services or resources to other devices. |
| Client | A device or application that requests services from a server. |
| Router | A device that connects different networks and forwards data between them. |
| Switch | A device that connects devices within a LAN and forwards data to the appropriate destination. |
| Hub | A device that sends incoming data to all connected ports. |
| Modem | A device that converts signals for transmission over a communication connection. |
| NIC | Network Interface Card; hardware that enables a device to connect to a network. |
| MAC Address | A hardware address used to identify a network interface on a local network. |
| IP Address | A logical address used to identify a device or interface on an IP network. |
| Ethernet | A widely used technology for wired LANs. |
| Wi-Fi | A wireless networking technology. |
| Bluetooth | A short-range wireless communication technology. |
| Transmission Media | The path through which data travels. |
| Data Collision | Interference caused when multiple devices transmit simultaneously over a shared medium. |
| Fault Tolerance | The ability of a network to continue operating despite component failures. |
| Reliability | The ability of a network to operate consistently. |
| Cloud Computing | Using computing resources over a network, often through remote servers. |
| IoT | Internet of Things; a system of connected physical devices that exchange data. |
| TCP/IP | A collection of communication protocols used for communication across networks. |
| ARPANET | An early packet-switching network that helped establish the foundation for the Internet. |
| WWW | World Wide Web; a system of linked web pages and online resources. |
| 5G | Fifth-generation mobile communication technology. |
| SDN | Software-Defined Networking; an approach to managing network control through software. |
| Edge Computing | Processing data closer to the devices that generate it. |
| Latency | The time taken for data to travel from its source to its destination. |
| Bandwidth | The maximum data-carrying capacity of a communication link. |
| Terminator | A component fitted at the end of a traditional bus cable to prevent signal reflection. |
| Fault Isolation | The process of identifying and separating the source of a network problem. |
| Wireless Access Point | A device that allows wireless devices to connect to a wired network. |

---
