# COMMON NETWORK PROTOCOLS – STUDY NOTES AND CHEAT SHEET

## Table of Contents

1. Introduction to Network Protocols
2. Classification of Network Protocols
3. Internet and Network Layer Protocols
   - IP
   - IPv4 and IPv6
   - ICMP
   - ARP
   - NDP
4. Transport Layer Protocols
   - TCP
   - UDP
   - QUIC
5. Web and Application Layer Protocols
   - HTTP
   - HTTPS
   - DNS
   - DHCP
6. Email Protocols
   - SMTP
   - POP3
   - IMAP
7. File Transfer and Sharing Protocols
   - FTP
   - FTPS
   - SFTP
   - TFTP
   - SMB
   - NFS
8. Remote Access and Network Management Protocols
   - SSH
   - Telnet
   - RDP
   - SNMP
   - NTP
9. Wireless and Network Access Protocols
   - Ethernet
   - Wi-Fi (IEEE 802.11)
   - Bluetooth
   - PPP
10. Security and Authentication Protocols
    - TLS
    - IPsec
    - WPA2 and WPA3
    - Kerberos
11. Important Port Numbers
12. Protocol Comparison and Real-World Communication Flow

---

# 1. Introduction to Network Protocols

A network protocol is a set of rules that determines how devices communicate and exchange information over a network.

In simple words, protocols make sure that the sender and receiver understand each other's messages. They define how information is formatted, addressed, transmitted, received and sometimes protected.

For example, when a person sends an email, one protocol may be used to send the message, another may be used to retrieve it, and other protocols help deliver the data across the internet.

### Why are protocols needed?

Imagine two people speaking different languages. Even if they are connected by a telephone, they may not understand each other. Network devices face a similar problem. Protocols provide common communication rules so that different devices and operating systems can exchange data.

**Main functions of protocols:**

- Addressing: Identifies the source and destination.
- Data formatting: Defines how information is organised.
- Transmission: Specifies how information is sent.
- Error detection: Helps identify corrupted data.
- Flow control: Manages the rate of communication.
- Reliability: Some protocols confirm delivery and retransmit missing data.
- Security: Some protocols provide encryption and authentication.

### Basic communication flow

```text
          SENDER DEVICE
                |
                v
       Creates information
                |
                v
       Follows protocol rules
                |
                v
        Sends network data
                |
                v
        NETWORK COMMUNICATION
                |
                v
        RECEIVER DEVICE
                |
                v
       Follows the same rules
                |
                v
       Understands the data
```

**Example:** When you open a website, DNS can find its IP address, IP helps route the packets, TCP or QUIC provides transport, and HTTP or HTTPS handles the actual web communication.

---

# 2. Classification of Network Protocols

Network protocols are commonly grouped according to the work they perform.

```text
                 NETWORK PROTOCOLS
                         |
      +------------------+-------------------+
      |                  |                   |
   NETWORK            TRANSPORT          APPLICATION
    LAYER                LAYER                LAYER
      |                  |                   |
   IP, ICMP           TCP, UDP            HTTP, DNS
   ARP, NDP           QUIC                SMTP, FTP
      |                  |                   |
      +------------------+-------------------+
                         |
                   OTHER PROTOCOLS
                         |
               SECURITY / MANAGEMENT
                         |
                 TLS, SSH, SNMP,
                 NTP, IPsec, etc.
```

### Protocols according to their main purpose

| Purpose | Common protocols |
|---|---|
| Addressing and routing | IP, IPv4, IPv6 |
| Error reporting | ICMP |
| Address resolution | ARP, NDP |
| Reliable transport | TCP |
| Fast transport | UDP, QUIC |
| Web communication | HTTP, HTTPS |
| Name resolution | DNS |
| Automatic IP configuration | DHCP |
| Sending email | SMTP |
| Receiving email | POP3, IMAP |
| File transfer | FTP, SFTP, TFTP |
| Remote access | SSH, Telnet, RDP |
| Network monitoring | SNMP |
| Time synchronisation | NTP |
| Secure communication | TLS, IPsec |
| Local wired networking | Ethernet |
| Wireless networking | Wi-Fi, Bluetooth |

### Understanding protocol layers

The OSI model is used to understand where networking functions take place.

| OSI layer | Main work | Examples |
|---|---|---|
| Layer 7 – Application | Services used by applications | HTTP, DNS, SMTP, FTP |
| Layer 6 – Presentation | Data representation and encryption concepts | Data encoding, TLS-related functions |
| Layer 5 – Session | Managing communication sessions | Session management |
| Layer 4 – Transport | End-to-end application communication | TCP, UDP |
| Layer 3 – Network | Logical addressing and routing | IP, ICMP |
| Layer 2 – Data Link | Local delivery and MAC addressing | Ethernet, Wi-Fi MAC |
| Layer 1 – Physical | Transmission of signals | Cables, radio, fibre |

A protocol does not necessarily occupy only one OSI layer. Some technologies cover more than one layer, and the OSI model is mainly a reference for understanding network functions.

---

# 3. Internet and Network Layer Protocols

## 3.1 IP – Internet Protocol

IP stands for Internet Protocol. It is responsible for logical addressing and forwarding packets from a source device to a destination device across networks.

Every device communicating over an IP network uses IP addressing.

**Main functions:**
- Provides logical addresses.
- Helps routers identify packet destinations.
- Supports communication between different networks.
- Carries data from higher-layer protocols.

### How IP works

```text
Source creates data
       |
       v
Transport protocol adds information
       |
       v
IP adds source and destination addresses
       |
       v
Packet reaches router
       |
       v
Router checks destination IP
       |
       v
Packet moves towards destination
       |
       v
Destination receives packet
```

**Applications and use cases:**
- Internet browsing.
- Video calls.
- Online gaming.
- Email communication.
- Communication between office networks.

**Important point:** IP provides best-effort delivery. It does not itself guarantee that packets arrive, arrive in order or are retransmitted if lost.

**Limitation:** Additional protocols such as TCP or UDP are needed for transport services.

## 3.2 IPv4 – Internet Protocol Version 4

IPv4 is the fourth version of the Internet Protocol and uses a 32-bit address.

An IPv4 address is usually written in four decimal numbers separated by dots.

**Example:** `192.168.1.10`

Each part ranges from 0 to 255.

**Features:**
- Uses 32-bit addressing.
- Supports approximately 4.3 billion theoretical address combinations.
- Widely supported by network equipment.
- Uses subnetting to divide networks.
- Supports broadcast communication.

**Applications:**
- Home networks.
- Office LANs.
- Internet service provider networks.
- Servers and websites.

**Real-world example:** A home router may assign `192.168.1.10` to a laptop through DHCP.

**Limitations:**
- Limited address space.
- Often requires NAT to allow many private devices to share a public IPv4 address.
- Broadcast traffic can affect network efficiency.

## 3.3 IPv6 – Internet Protocol Version 6

IPv6 is the newer version of IP, designed mainly to solve the address shortage of IPv4 and improve aspects of network communication.

It uses 128-bit addresses.

**Example:** `2001:db8::1`

**Features:**
- Extremely large address space.
- Simplified base header compared with IPv4.
- Supports automatic address configuration.
- Uses multicast instead of broadcast for many functions.
- Supports IPsec as part of its protocol architecture, though actual security use depends on deployment.

**Applications:**
- Modern internet networks.
- Large enterprise networks.
- Mobile networks.
- IoT devices.
- Data centres.

**Real-world example:** A mobile network may use IPv6 to provide addresses to smartphones and other connected devices.

**Limitations:**
- Some older devices and networks may not support it fully.
- Migration and configuration can require technical planning.
- IPv4 and IPv6 may need to operate together during transition.

### IPv4 and IPv6 comparison

| IPv4 | IPv6 |
|---|---|
| 32-bit address | 128-bit address |
| Example: 192.168.1.1 | Example: 2001:db8::1 |
| Limited address space | Extremely large address space |
| Supports broadcast | Uses multicast instead of broadcast |
| NAT is common | Designed to support large-scale addressing |
| Older and widely deployed | Newer and increasingly deployed |

## 3.4 ICMP – Internet Control Message Protocol

ICMP is used by network devices to send error reports and diagnostic information.

It works alongside IP and helps devices understand certain network problems.

**Features and functions:**
- Reports destination unreachable conditions.
- Helps report time exceeded.
- Supports diagnostic tools.
- Helps troubleshoot connectivity problems.

**Important command: PING**

Ping uses ICMP Echo Request and Echo Reply messages to test whether a destination can be reached.

### How ping works

```text
Computer A
    |
    v
Sends ICMP Echo Request
    |
    v
Network
    |
    v
Computer B
    |
    v
Sends ICMP Echo Reply
    |
    v
Computer A receives reply
    |
    v
Connection reachability is tested
```

**Applications:**
- Checking whether a server is reachable.
- Testing network connectivity.
- Measuring round-trip time.
- Basic network troubleshooting.

**Example:** A technician enters `ping 8.8.8.8` to check whether the computer can reach a public IP address.

**Limitation:** A device may block ICMP messages even when its other network services are working. Therefore, no ping reply does not always mean that the device is offline.

## 3.5 ARP – Address Resolution Protocol

ARP is used in IPv4 local networks to find the MAC address associated with a known IPv4 address.

A computer may know the destination IP address but still need the destination MAC address to send a local Ethernet frame.

### ARP working

```text
Computer needs a MAC address
             |
             v
       Checks ARP cache
             |
        Address found?
          /       \
        Yes        No
         |          |
         v          v
      Use it    Send ARP request
                    |
                    v
              Target replies
                    |
                    v
             MAC address stored
                    |
                    v
              Frame is sent
```

**Features:**
- Resolves IPv4 addresses to MAC addresses.
- Uses ARP requests and replies.
- Stores mappings in an ARP cache.

**Applications:**
- Local Ethernet communication.
- IPv4 LANs.
- Communication between devices on the same subnet.

**Example:** A computer wants to send data to `192.168.1.20` and uses ARP to discover the destination's MAC address.

**Limitation:** ARP can be affected by ARP spoofing attacks. It is used with IPv4, not IPv6.

## 3.6 NDP – Neighbour Discovery Protocol

NDP is an IPv6 protocol used by devices to discover neighbouring devices and routers on a local network.

It performs functions that are partly handled by ARP in IPv4, but it provides additional features.

**Main functions:**
- Discovers neighbouring devices.
- Finds link-layer addresses.
- Helps discover routers.
- Supports IPv6 address configuration.
- Checks whether an IPv6 address is already in use.

**Applications:** IPv6 LANs, modern enterprise networks and IPv6-enabled home networks.

**Example:** An IPv6-enabled laptop uses NDP to discover the router that provides access to the internet.

**Limitation:** Incorrect NDP configuration or attacks against neighbour discovery can affect IPv6 communication.

---

# 4. Transport Layer Protocols

Transport layer protocols provide communication between applications running on different devices.

They use port numbers to identify application processes and services.

The two most common transport protocols are TCP and UDP.

## 4.1 TCP – Transmission Control Protocol

TCP is a connection-oriented transport protocol that provides reliable and ordered data delivery.

It is used when information needs to arrive correctly and in the proper order.

**Main features:**
- Establishes a connection before normal data transfer.
- Uses sequence numbers.
- Uses acknowledgements.
- Retransmits missing data.
- Provides flow control.
- Uses congestion control.

### TCP three-way handshake

```text
          CLIENT                  SERVER
             |                       |
             | ------- SYN --------> |
             |                       |
             | <---- SYN + ACK ----- |
             |                       |
             | ------- ACK --------> |
             |                       |
             |   CONNECTION READY   |
```

**How it works:**
1. Client sends SYN to request a connection.
2. Server responds with SYN-ACK.
3. Client sends ACK.
4. The connection is ready for data transfer.

**Applications and use cases:**
- Web browsing using HTTP/1.1 and HTTP/2.
- Email transmission.
- File transfers.
- Remote access.
- Database communication.

**Example:** When downloading a PDF from a website using a TCP-based connection, TCP helps ensure that the data arrives reliably and in order.

**Limitation:** Connection setup and retransmissions can add delay and overhead, making TCP less suitable for some very time-sensitive applications.

## 4.2 UDP – User Datagram Protocol

UDP is a connectionless transport protocol that sends data without establishing a connection first.

It is often used when low delay and low overhead are important.

**Main features:**
- No connection establishment.
- Low overhead.
- Uses port numbers.
- No built-in retransmission.
- No built-in packet ordering.
- Does not guarantee delivery.

### UDP working

```text
Application creates data
         |
         v
UDP adds port information
         |
         v
Datagram is sent
         |
         v
Receiver receives available data
         |
         v
Application processes it
```

**Applications and use cases:**
- Online gaming.
- Voice and video calls.
- DNS queries in common cases.
- Live media delivery.
- Real-time monitoring.

**Example:** In an online game, receiving the latest player position quickly can be more useful than waiting for an old lost update to be retransmitted.

**Limitation:** Packets can be lost or arrive out of order. Applications needing reliability must provide it themselves.

## 4.3 QUIC

QUIC is a modern transport protocol built on UDP. It provides secure and reliable communication features and is used by HTTP/3.

It was designed to improve connection establishment, security and performance, particularly when network conditions change.

**Features:**
- Uses UDP as its underlying transport.
- Integrates TLS 1.3 security.
- Supports multiple streams.
- Can reduce connection setup delay.
- Supports connection migration, which can help when a device changes networks.

**Applications:**
- HTTP/3 websites.
- Modern web services.
- Mobile internet applications.
- Services requiring reliable, secure communication.

**Example:** A browser accesses a website using HTTP/3, which uses QUIC over UDP.

**Limitations:**
- Requires compatible software and network equipment.
- Some networks may restrict or interfere with UDP traffic.
- Troubleshooting can be less familiar than traditional TCP traffic.

### TCP, UDP and QUIC comparison

| Feature | TCP | UDP | QUIC |
|---|---|---|---|
| Connection | Connection-oriented | Connectionless | Connection-based transport built on UDP |
| Reliability | Built in | Not built in | Built in |
| Ordering | Yes | No guarantee | Per-stream ordering |
| Encryption | Not built in | Not built in | Integrates TLS 1.3 |
| Common use | Web, file transfer, email | DNS, gaming, real-time media | HTTP/3 |
| Main benefit | Reliable delivery | Low overhead | Secure, modern transport |

---

# 5. Web and Application Layer Protocols

## 5.1 HTTP – Hypertext Transfer Protocol

HTTP is an application-layer protocol used for communication between web browsers and web servers.

It defines how a browser requests a resource and how a server responds.

**Example:** Opening a news website in a browser.

### HTTP working

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

**Common HTTP methods:**
- GET – Requests information.
- POST – Sends information.
- PUT – Creates or replaces a resource.
- PATCH – Updates part of a resource.
- DELETE – Requests deletion of a resource.

**Features:**
- Uses request-response communication.
- Supports headers and status codes.
- Transfers web pages and application data.
- Supports different content types.

**Applications:**
- Websites.
- Online shopping.
- Social media.
- Online forms.
- Web applications.

**Port:** TCP 80 is the traditional default port for HTTP.

**Limitation:** Plain HTTP does not encrypt communication, so it should not be used for sensitive information over untrusted networks.

## 5.2 HTTPS – Hypertext Transfer Protocol Secure

HTTPS is HTTP protected by TLS encryption. It provides secure communication between a browser and a web server.

**Features:**
- Encrypts data in transit.
- Helps prevent unauthorised reading of transmitted information.
- Provides integrity protection.
- Authenticates the server through digital certificates.

**Applications:**
- Online banking.
- Shopping websites.
- Social media.
- Login pages.
- Email services.

**Example:** When someone logs into an online banking website, HTTPS helps protect the login details during transmission.

**Port:** TCP 443 is the traditional default port for HTTPS over TCP. HTTP/3 uses QUIC over UDP, commonly on UDP port 443.

**Limitation:** HTTPS protects communication in transit, but it does not guarantee that the website itself is honest or free from malware.

### HTTP and HTTPS comparison

| HTTP | HTTPS |
|---|---|
| Communication is not encrypted by default | Uses TLS encryption |
| Less suitable for sensitive information | Suitable for secure web communication |
| Traditional port 80 | Traditional port 443 |
| Does not authenticate the server through TLS | Uses certificates to authenticate the server |

## 5.3 DNS – Domain Name System

DNS translates domain names into IP addresses.

People remember website names more easily than numerical IP addresses. DNS helps computers locate the correct server.

**Example:** A browser needs to find the IP address for `www.example.com`.

### DNS working

```text
User enters domain name
          |
          v
Device checks local DNS cache
          |
          v
Query goes to DNS resolver
          |
          v
DNS finds the required record
          |
          v
IP address is returned
          |
          v
Browser contacts web server
```

**Important DNS records:**
- A – Maps a domain name to an IPv4 address.
- AAAA – Maps a domain name to an IPv6 address.
- CNAME – Provides an alias for another domain.
- MX – Identifies mail servers.
- NS – Identifies authoritative name servers.
- TXT – Stores text information, often used for verification and email security.

**Applications:**
- Website access.
- Email delivery.
- Service discovery.
- Network administration.

**Port:** 53, commonly UDP for normal queries and TCP in other situations.

**Limitation:** Incorrect DNS records or unavailable DNS servers can prevent users from accessing websites by domain name.

## 5.4 DHCP – Dynamic Host Configuration Protocol

DHCP automatically provides IP configuration to devices joining a network.

It saves administrators from manually entering IP addresses and other network details on every computer.

**Information provided by DHCP may include:**
- IP address.
- Subnet mask.
- Default gateway.
- DNS server address.
- Lease duration.

### DHCP DORA process

```text
        CLIENT DEVICE
              |
              v
          DISCOVER
       Finds DHCP server
              |
              v
           OFFER
       Server offers IP
              |
              v
          REQUEST
       Client requests IP
              |
              v
        ACKNOWLEDGEMENT
       Server confirms lease
              |
              v
       CLIENT USES IP SETTINGS
```

**Applications:**
- Home Wi-Fi.
- College computer laboratories.
- Office networks.
- Public hotspots.
- Enterprise networks.

**Example:** When a phone joins home Wi-Fi, the router's DHCP service can automatically assign it an IP address.

**Ports:** UDP 67 for servers and UDP 68 for clients in IPv4 DHCP.

**Limitation:** If the DHCP server fails or the available address pool is exhausted, new devices may not obtain a valid configuration.

---

# 6. Email Protocols

Email communication uses separate protocols for sending messages and accessing received messages.

## 6.1 SMTP – Simple Mail Transfer Protocol

SMTP is used to send outgoing emails from a client to a mail server and to transfer messages between mail servers.

**Example:** A student sends an assignment to a teacher through their college email account.

**Features and functions:**
- Sends outgoing messages.
- Transfers messages between mail servers.
- Supports message submission and delivery.

**Applications:** Gmail, Outlook, college email and business email systems.

**Common ports:**
- 25 – Mail server-to-server transfer.
- 587 – Message submission.
- 465 – Message submission using implicit TLS.

**Limitation:** SMTP is designed for sending email, not for retrieving messages from an inbox.

### SMTP working

```text
Sender writes email
        |
        v
Email client submits message
        |
        v
SMTP server processes message
        |
        v
Message is transferred
        |
        v
Recipient mail server stores email
        |
        v
Recipient accesses email
```

## 6.2 POP3 – Post Office Protocol Version 3

POP3 is used by an email client to retrieve messages from a mail server.

It is generally designed around downloading messages to the user's device.

**Features:**
- Downloads messages.
- Can be configured to leave copies on the server.
- Provides simple email retrieval.

**Applications:** Basic email access and users who prefer local message storage.

**Example:** A user downloads emails from a mail server to a computer.

**Ports:**
- 110 – POP3.
- 995 – POP3 over TLS.

**Limitations:**
- Less suitable for synchronising multiple devices.
- Messages and folders may not remain consistently synchronised across devices.

## 6.3 IMAP – Internet Message Access Protocol

IMAP allows users to access and manage email stored on a mail server.

It is useful when a person checks the same mailbox using multiple devices.

**Features:**
- Keeps messages on the server.
- Synchronises email across devices.
- Supports folders and message status.
- Allows users to manage messages remotely.

**Applications:** Modern email services accessed through phones, laptops and webmail.

**Example:** A student reads an email on a phone and later sees the same email marked as read on a laptop.

**Ports:**
- 143 – IMAP.
- 993 – IMAP over TLS.

**Limitations:** It relies on server storage and network access for many operations.

### SMTP, POP3 and IMAP comparison

| Protocol | Main function | Direction or purpose |
|---|---|---|
| SMTP | Sends email | Outgoing mail |
| POP3 | Downloads email | Incoming mail |
| IMAP | Accesses and synchronises email | Incoming mail |

**Easy way to remember:** SMTP sends, POP3 downloads, IMAP synchronises.

---

# 7. File Transfer and Sharing Protocols

## 7.1 FTP – File Transfer Protocol

FTP is a protocol used to transfer files between a client and a server over a network.

It allows users to upload, download, rename and manage files on a remote system.

**Features:**
- Supports file uploads and downloads.
- Uses a client-server model.
- Traditionally uses separate control and data connections.
- Supports user authentication.

**Applications:**
- Uploading website files.
- Transferring files between computers.
- Managing files on remote servers.

**Example:** A website administrator uploads webpage files to a web hosting server using FTP.

**Ports:** TCP 21 for control; the data connection uses different ports depending on the mode.

**Limitation:** Traditional FTP does not encrypt passwords or file contents. It should not be used for sensitive transfers over untrusted networks.

## 7.2 FTPS – FTP Secure

FTPS is FTP protected using TLS encryption.

It adds security to traditional FTP communication.

**Features:**
- Encrypts authentication details.
- Can encrypt file transfers.
- Uses certificates and TLS.

**Applications:** Secure file transfers with systems that support FTP-based workflows.

**Example:** A company transfers documents to a server using FTP with TLS protection.

**Ports:** TCP 21 is commonly used for explicit FTPS; implicit FTPS commonly uses TCP 990.

**Limitation:** Firewall configuration can be more complicated because FTP may use separate data connections.

## 7.3 SFTP – SSH File Transfer Protocol

SFTP is a secure file transfer protocol that operates over SSH.

Despite the similar name, SFTP is not simply FTP with encryption. It is a different protocol.

**Features:**
- Encrypts file transfers.
- Supports secure authentication.
- Allows remote file management.
- Uses a single SSH connection.

**Applications:**
- Business file transfer.
- Website management.
- Secure exchange of confidential documents.
- Server administration.

**Example:** An administrator securely uploads website files to a Linux server using SFTP.

**Port:** TCP 22 by default.

**Limitation:** Both client and server must support the SFTP protocol.

## 7.4 TFTP – Trivial File Transfer Protocol

TFTP is a simple file transfer protocol that provides basic file transfer without many of the features found in FTP.

**Features:**
- Simple design.
- Uses UDP.
- Does not provide built-in user authentication.
- Commonly used for basic network-device file transfers.

**Applications:**
- Network-device booting.
- Firmware transfers in controlled environments.
- Transferring configuration files.

**Example:** A network device downloads a boot image from a TFTP server.

**Port:** UDP 69 for initial requests.

**Limitations:**
- No built-in encryption.
- No normal user authentication.
- Not suitable for sensitive file transfers over untrusted networks.

## 7.5 SMB – Server Message Block

SMB is a network protocol used to share files, folders and printers between devices.

It is widely associated with Windows-based networks, although it is also supported by other operating systems.

**Features:**
- File and folder sharing.
- Printer sharing.
- Network resource access.
- User authentication and access control.

**Applications:**
- Office file servers.
- Shared folders.
- Network printers.
- Windows LANs.

**Example:** Employees in an office access a shared folder stored on a central file server.

**Port:** TCP 445 for modern direct-hosted SMB.

**Limitations:** Incorrect permissions or outdated versions can create security risks. SMB should be properly configured and updated.

## 7.6 NFS – Network File System

NFS is a protocol that allows users on one computer to access files stored on another computer over a network.

It is commonly used in Unix and Linux environments.

**Features:**
- Remote file access.
- Shared directory access.
- Centralised storage.
- Allows multiple computers to work with shared files.

**Applications:**
- Linux server environments.
- University computing laboratories.
- Enterprise file storage.
- Data centres.

**Example:** Several Linux computers access the same shared directory hosted on a central server.

**Ports:** TCP or UDP 2049 is commonly used for NFS; supporting services depend on the NFS version and configuration.

**Limitations:** Network interruptions can affect access to shared files, and permissions must be managed carefully.

### File transfer protocols compared

| Protocol | Main use | Security | Common port |
|---|---|---|---|
| FTP | File transfer | No built-in encryption | TCP 21 |
| FTPS | Secure FTP | TLS | TCP 21 or 990 |
| SFTP | Secure file transfer | SSH encryption | TCP 22 |
| TFTP | Simple file transfer | No built-in encryption | UDP 69 |
| SMB | File and printer sharing | Depends on version and configuration | TCP 445 |
| NFS | Network file sharing | Depends on version and configuration | TCP/UDP 2049 |

---

# 8. Remote Access and Network Management Protocols

## 8.1 SSH – Secure Shell

SSH is a protocol that allows users to securely access and manage remote computers over a network.

It encrypts communication between the client and server.

**Features:**
- Secure remote login.
- Encrypted communication.
- Supports command-line administration.
- Supports secure file transfer through SFTP.
- Can provide secure tunnelling.

**Applications:**
- Linux server administration.
- Remote network-device configuration.
- Secure file transfer.
- Managing cloud servers.

**Example:** An administrator connects to a remote Linux server using SSH to update software.

**Port:** TCP 22 by default.

**Limitation:** Requires correct authentication and configuration. Weak passwords or exposed private keys can create security risks.

## 8.2 Telnet

Telnet is an older protocol used for remote terminal access.

It allows a user to connect to a remote computer and execute commands.

**Features:**
- Provides text-based remote access.
- Uses a client-server model.
- Allows remote command interaction.

**Applications:**
- Historical remote administration.
- Controlled networking laboratories.
- Basic connectivity testing.

**Example:** A student uses Telnet in a networking lab to understand remote terminal communication.

**Port:** TCP 23.

**Limitation:** Telnet does not encrypt communication. Usernames, passwords and commands may be exposed. SSH is preferred for secure remote administration.

## 8.3 RDP – Remote Desktop Protocol

RDP is a Microsoft-developed protocol that allows a user to access and control a remote computer through a graphical desktop interface.

**Features:**
- Remote desktop display.
- Keyboard and mouse interaction.
- Supports remote application use.
- Can support audio and clipboard redirection.

**Applications:**
- Remote office work.
- IT support.
- Managing Windows servers.
- Accessing a computer from another location.

**Example:** A technician uses Remote Desktop to access and repair an office computer from another location.

**Port:** TCP 3389 by default; UDP 3389 may also be used.

**Limitations:**
- Requires secure configuration.
- Exposing RDP directly to the public internet can create security risks.
- Performance depends on connection quality.

## 8.4 SNMP – Simple Network Management Protocol

SNMP is used to monitor and manage network devices such as routers, switches, printers and servers.

It helps administrators collect information about the condition and performance of network equipment.

**Features:**
- Monitors network devices.
- Collects performance information.
- Can send alerts or notifications.
- Supports remote management.

**Applications:**
- Monitoring routers and switches.
- Checking network interface usage.
- Monitoring server performance.
- Detecting equipment problems.

**Example:** A network administrator uses SNMP monitoring software to check whether a college switch is overloaded.

**Common ports:**
- UDP 161 – Requests and responses.
- UDP 162 – Notifications or traps.

**Versions:**
- SNMPv1: Original version.
- SNMPv2c: Adds improvements but commonly relies on community strings.
- SNMPv3: Supports stronger authentication and privacy features.

**Limitation:** Older SNMP versions do not provide strong security. SNMPv3 is preferred when security is important.

## 8.5 NTP – Network Time Protocol

NTP is used to synchronise the clocks of computers and network devices.

Accurate time is important because network systems use timestamps for logs, authentication, security and troubleshooting.

**Features:**
- Synchronises system clocks.
- Helps maintain accurate timestamps.
- Supports time synchronisation across networks.

**Applications:**
- Banking systems.
- Servers.
- CCTV systems.
- Network logs.
- Enterprise networks.

**Example:** A college server and its connected computers use NTP so that attendance records and system logs show consistent times.

**Port:** UDP 123.

**Limitation:** Incorrect time sources or blocked NTP traffic can lead to inaccurate device clocks.

---

# 9. Wireless and Network Access Protocols

## 9.1 Ethernet

Ethernet is a family of wired LAN technologies standardised under IEEE 802.3.

It defines how devices communicate over wired local area networks.

**Features:**
- Uses frames.
- Uses MAC addresses.
- Supports different data rates.
- Works over twisted-pair and fibre-optic media.
- Modern Ethernet commonly supports full-duplex communication.

**Applications:**
- Office networks.
- Computer laboratories.
- Data centres.
- Home wired networks.
- Enterprise LANs.

**Example:** A computer connects to a switch using a Cat6 cable.

**Limitation:** Requires physical cabling, and cable installation may be difficult across large buildings.

## 9.2 Wi-Fi – IEEE 802.11

Wi-Fi is a wireless networking technology used to connect devices to a WLAN.

It allows devices to communicate using radio signals instead of requiring a cable connection.

**Features:**
- Wireless access.
- Mobility.
- Supports multiple connected devices.
- Uses access points.
- Supports wireless security standards.

**Applications:**
- Homes.
- Colleges.
- Offices.
- Airports.
- Hotels.
- Public hotspots.

**Example:** A smartphone connects to a home router through Wi-Fi.

**Limitation:** Wireless signals can be affected by obstacles, interference and distance.

### Wi-Fi generation overview

| Generation | IEEE standard | Main development |
|---|---|---|
| Wi-Fi 1 | 802.11b | Early widely used Wi-Fi |
| Wi-Fi 2 | 802.11a | 5 GHz operation |
| Wi-Fi 3 | 802.11g | Higher speed in 2.4 GHz |
| Wi-Fi 4 | 802.11n | MIMO and improved capacity |
| Wi-Fi 5 | 802.11ac | Higher speeds and wider channels |
| Wi-Fi 6 | 802.11ax | Better efficiency in crowded networks |
| Wi-Fi 6E | 802.11ax extension | Adds 6 GHz band where permitted |
| Wi-Fi 7 | 802.11be | Multi-Link Operation and wider channels |

## 9.3 Bluetooth

Bluetooth is a short-range wireless communication technology used to connect nearby devices.

**Features:**
- Low-power communication.
- Short-range connectivity.
- Wireless device pairing.
- Supports different device types and applications.

**Applications:**
- Headphones.
- Wireless speakers.
- Smartwatches.
- Keyboards and mice.
- Car audio systems.

**Example:** A phone connects to a Bluetooth speaker to play audio.

**Limitation:** It is generally intended for shorter distances and lower data rates than Wi-Fi.

## 9.4 PPP – Point-to-Point Protocol

PPP is a Data Link Layer protocol used to establish a direct connection between two network nodes.

It was historically common in dial-up connections and is also used in some point-to-point networking systems.

**Features:**
- Supports point-to-point communication.
- Can carry different network-layer protocols.
- Supports link configuration.
- Can support authentication mechanisms.

**Applications:**
- Older dial-up internet connections.
- Some WAN connections.
- PPP-based access links.

**Example:** A traditional dial-up modem connection uses PPP to carry IP traffic.

**Limitation:** It is not commonly used for ordinary modern home Ethernet LANs.

---

# 10. Security and Authentication Protocols

## 10.1 TLS – Transport Layer Security

TLS is a security protocol that protects communication between applications over a network.

It provides encryption, authentication and integrity protection.

**Features:**
- Encrypts communication.
- Helps authenticate the server.
- Detects unauthorised changes to transmitted data.
- Protects protocols such as HTTPS.

**Applications:**
- Secure websites.
- Email security.
- Secure APIs.
- Online banking.
- Business applications.

**Example:** A browser uses TLS when connecting to an HTTPS banking website.

**Common versions:** TLS 1.2 and TLS 1.3 are widely recognised modern versions.

**Limitation:** TLS does not make an unsafe website trustworthy. It protects the communication channel, not every part of the application.

## 10.2 IPsec – Internet Protocol Security

IPsec is a collection of protocols used to protect IP communication.

It provides security at the network layer and is commonly used in VPNs.

**Features:**
- Provides encryption.
- Supports authentication.
- Protects data integrity.
- Can operate in transport mode or tunnel mode.

**Applications:**
- Site-to-site VPNs.
- Remote access VPNs.
- Secure communication between office networks.
- Enterprise network protection.

**Example:** A company uses an IPsec VPN to securely connect its Srinagar office with its Delhi office over the internet.

**Limitation:** Configuration can be complex, and different equipment must use compatible settings.

## 10.3 WPA2 and WPA3

WPA2 and WPA3 are Wi-Fi security certification standards based on IEEE 802.11 security mechanisms.

They help protect wireless networks against unauthorised access and data interception.

### WPA2

- Widely used wireless security.
- Commonly uses AES-based CCMP protection.
- Suitable when configured properly.

### WPA3

- Newer wireless security standard.
- Provides stronger password-based protection through SAE in personal networks.
- Improves security in supported deployments.

**Applications:** Home Wi-Fi, office wireless networks, colleges and public wireless systems.

**Example:** A home router uses WPA3 so that only authorised users with the correct credentials can join the network.

**Limitations:** Older devices may not support WPA3. Security still depends on proper configuration and strong credentials.

## 10.4 Kerberos

Kerberos is a network authentication protocol that allows users and services to prove their identities securely.

It uses tickets rather than repeatedly sending passwords across the network.

**Features:**
- Centralised authentication.
- Ticket-based access.
- Supports mutual authentication.
- Uses time-limited credentials.

**Applications:**
- Enterprise networks.
- Windows Active Directory environments.
- University authentication systems.
- Internal business services.

**Example:** An employee signs into an organisation's network and accesses approved services using Kerberos-based authentication.

**Limitation:** It depends on correctly configured authentication servers and reasonably synchronised clocks.

---

# 11. Important Port Numbers

A port number identifies an application or service endpoint on a device. It is used with transport protocols such as TCP and UDP.

The following are common default port numbers that are useful for networking examinations.

| Protocol or service | Port | Transport |
|---|---:|---|
| FTP control | 21 | TCP |
| SSH | 22 | TCP |
| Telnet | 23 | TCP |
| SMTP server transfer | 25 | TCP |
| DNS | 53 | UDP/TCP |
| DHCP server | 67 | UDP |
| DHCP client | 68 | UDP |
| TFTP | 69 | UDP |
| HTTP | 80 | TCP |
| POP3 | 110 | TCP |
| NTP | 123 | UDP |
| IMAP | 143 | TCP |
| SNMP requests | 161 | UDP |
| SNMP traps | 162 | UDP |
| HTTPS over TCP | 443 | TCP |
| SMB | 445 | TCP |
| SMTP submission | 587 | TCP |
| IPsec NAT Traversal | 4500 | UDP |
| FTPS implicit | 990 | TCP |
| IMAPS | 993 | TCP |
| POP3S | 995 | TCP |
| RDP | 3389 | TCP/UDP |

**Important notes:**
- A port number is not the same as an IP address.
- Port numbers identify services or application endpoints.
- Some protocols use more than one port.
- A service may be configured to use a different port.
- HTTP/3 uses QUIC over UDP, commonly on port 443.

### Easy port-number memory tips

- 20 and 21 – FTP data and control in traditional active FTP.
- 22 – SSH.
- 23 – Telnet.
- 25 – SMTP.
- 53 – DNS.
- 67 and 68 – DHCP.
- 80 – HTTP.
- 110 – POP3.
- 143 – IMAP.
- 443 – HTTPS.
- 3389 – RDP.

---

# 12. Protocol Comparison and Real-World Communication Flow

## 12.1 Common protocols at a glance

| Protocol | Main purpose | Main layer |
|---|---|---|
| IP | Addressing and routing | Network |
| IPv4 | 32-bit IP addressing | Network |
| IPv6 | 128-bit IP addressing | Network |
| ICMP | Error reporting and diagnostics | Network |
| ARP | IPv4-to-MAC address resolution | Between L2/L3 functions |
| NDP | IPv6 neighbour discovery | Network |
| TCP | Reliable transport | Transport |
| UDP | Lightweight datagram transport | Transport |
| QUIC | Secure reliable transport over UDP | Transport |
| HTTP | Web communication | Application |
| HTTPS | Secure web communication | Application |
| DNS | Domain-name resolution | Application |
| DHCP | Automatic network configuration | Application |
| SMTP | Sending email | Application |
| POP3 | Downloading email | Application |
| IMAP | Email access and synchronisation | Application |
| FTP | File transfer | Application |
| SFTP | Secure file transfer over SSH | Application |
| SSH | Secure remote access | Application |
| Telnet | Unencrypted remote terminal access | Application |
| RDP | Remote graphical desktop | Application |
| SNMP | Network monitoring and management | Application |
| NTP | Time synchronisation | Application |
| Ethernet | Wired LAN communication | Data Link / Physical |
| Wi-Fi | Wireless LAN communication | Data Link / Physical |
| TLS | Secure communication | Between application and transport functions |

## 12.2 Real-world example: Opening a website

Suppose a student opens a college website using a laptop connected to Wi-Fi.

```text
        STUDENT OPENS BROWSER
                 |
                 v
          ENTERS WEBSITE NAME
                 |
                 v
          DNS RESOLVES DOMAIN
                 |
                 v
         WEBSITE IP IS FOUND
                 |
                 v
       TCP OR QUIC CONNECTION
                 |
                 v
       TLS SECURES COMMUNICATION
                 |
                 v
         HTTP/HTTPS REQUEST
                 |
                 v
       IP ROUTES NETWORK PACKETS
                 |
                 v
        WI-FI / ETHERNET LINKS
                 |
                 v
          ROUTERS FORWARD DATA
                 |
                 v
          WEBSITE SERVER
                 |
                 v
        RESPONSE RETURNS TO USER
                 |
                 v
          WEBSITE IS DISPLAYED
```

The exact sequence can vary depending on DNS caching, HTTP version and network configuration. For example, HTTP/3 uses QUIC rather than TCP.

## 12.3 Real-world example: Sending an email

```text
       USER WRITES AN EMAIL
                |
                v
        EMAIL CLIENT PREPARES
             MESSAGE
                |
                v
          SMTP SENDS EMAIL
                |
                v
        RECIPIENT MAIL SERVER
           RECEIVES MESSAGE
                |
                v
        MESSAGE IS STORED
                |
                v
        RECIPIENT OPENS EMAIL
                |
          +-----+-----+
          |           |
          v           v
         IMAP        POP3
      Synchronise   Download
          |           |
          +-----+-----+
                |
                v
         EMAIL IS READ
```

## 12.4 Real-world example: Transferring a file securely

```text
       USER SELECTS A FILE
                |
                v
        CONNECTS TO SERVER
                |
                v
          SSH CONNECTION
                |
                v
          SFTP TRANSFER
                |
                v
        DATA IS ENCRYPTED
                |
                v
         FILE REACHES SERVER
                |
                v
        SERVER STORES FILE
```

---

# 13. Important Points to Remember for Exams

1. A protocol is a set of rules that controls communication between network devices.
2. TCP is connection-oriented and provides reliable, ordered delivery.
3. UDP is connectionless and has low overhead.
4. IP is responsible for logical addressing and packet forwarding.
5. IPv4 uses 32-bit addresses, while IPv6 uses 128-bit addresses.
6. ICMP is used for error reporting and network diagnostics.
7. ARP finds the MAC address associated with an IPv4 address on a local network.
8. NDP performs neighbour discovery functions in IPv6.
9. HTTP is used for web communication.
10. HTTPS uses TLS to protect HTTP communication.
11. DNS translates domain names into IP addresses.
12. DHCP automatically provides IP configuration.
13. SMTP is used for sending email.
14. POP3 is used for downloading email.
15. IMAP is used for accessing and synchronising email.
16. FTP transfers files but does not provide built-in encryption.
17. SFTP provides secure file transfer over SSH.
18. SSH provides secure remote access.
19. Telnet is an older, unencrypted remote access protocol.
20. SNMP is used for network monitoring and management.
21. NTP synchronises computer and network-device clocks.
22. TLS provides encryption, authentication and integrity protection.
23. IPsec protects IP communication and is commonly used in VPNs.
24. Ethernet is a common wired LAN technology.
25. Wi-Fi is based on the IEEE 802.11 family of standards.

**Final understanding:** Protocols are the rules that make network communication possible. Some protocols identify devices and route data, some transport information, some provide application services, and others protect or manage communication. Together, they allow different computers, phones, servers and network devices to work as one connected system.