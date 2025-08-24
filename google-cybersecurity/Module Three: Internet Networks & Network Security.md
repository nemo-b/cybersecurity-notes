COURSE LEARNINGS:

- Structure of a network
- Network operations
- Network attacks
- Security hardening

Addresses and identifiers

**Local area network (LAN)**: A network that spans a small area like an office building, a school, or a home.

**Wide area network (WAN)**: A network that spans a large geographic area like a city, state, or country.

Physical tools

**Hub**: A network that broadcasts information to every device on the network

**Switch**: A device that makes connections between specific devices on a network by sending and receiving data between them

**Router**: A network device that connects multiple networks together

**Modem**: A device that connects your router to the internet and brings the internet to the LAN

**Virtualization tools**: Pieces of software that preform network operations

Cloud service providers offer

- On-demand storage
- Processing power
- Analytics.

**Data packet**: A basic unit of information that travels from one device to another within a network

Data packets are similar to sending mail, you would write the address of the destination and the return address of the sender.

The header contains the IP address, MAC address, and protocol number. The Body contains the message that need to be sent to the receiving device. The footer signals that the receiving package has been finished.

**Bandwidth**: The amount of data a device receives every second

**Speed**: the rate at which the data packet are received or downloaded

**Packet sniffing**: The practice and inspecting data packets across a network

**Internet protocol (IP)**: A set of standards used for routing and addressing data packets as they travel between devices on a network

Port: A software-based location that organizes the sending and receiving of data between devices on a network

**TCP/IP model**: A framework used to visualize how data is organized and transmitted across the network

Layers of the TCP/IP model

1. Network access layer: Deals with creation of data packets.
2. Internet layer: Where IP addresses are attached to data packets to indicate the location of the sender and receiver. This layer also focuses on how networks connect to each other. For example, being sent on LAN, or be sent to a remote network, like the Internet.
3. Transport layer: Includes protocols to control the traffic across a network. (Ensures smooth travel of information)
4. Application layer: Protocols determine how data packets will interact with receiving devices. 

**Internet protocol (IP) address**: A unique string of characters that identifies the location of a device on the internet

IP addresses

- IP version 4 (IPv4)

EX: 19.117.63.126 (IP version 4)

- IP version 6 (IPv6)

EX: 684D:1111:222:3333:4444:5555:6:77 (IP version 6)

All devices used to use the IPv4, but as more people and more devices joined the internet, the amount of IPs was diminishing; This led to the current use of IPv6, which has many numbers for more people.

**MAC address**: A uniques alphanumerical identifier that is assigned to each physical device on a network

Rules ensure data sent over the network gets to the right place. These are called network protocols.

**Network protocols**: A set of rules by two or more devices on a network to describe the order of delivery and structure of data

**Transmission Control protocol (T.C.P.)**: An internet communications protocol that allows two devices to form a connection and stream data

The T.C.P. process also verifies both devices before allowing any further communications to take place, this is referred to as a “Handshake”

Address Resolution Protocol (A.R.P.): A network protocol used to determine the MAC address of the next router or device on the path

**Hyper Text Transfer Protocol Secure (HTTPS)**: A network protocol that provides a secure method of communication between clients and website servers

**Domain Name System (D.N.S.)**: A network that translates internet domain names into IP addresses

![Screen Shot 2023-10-03 at 7.46.59 PM.png](Screen_Shot_2023-10-03_at_7.46.59_PM.png)

IEEE 802.11 (WiFi): A set of standards that define communication for wireless LAN's

IEEE stands for Institute of Electrical and Electronics Engineers. This is the organization that maintains WiFi standards

WiFi Protected Access (W.P.A.): A wireless security protocol for devices to connect to the Internet

**Firewall**: A network security device that monitors traffic to and from your network

**Port filtering**: A firewall function that blocks or allows certain port numbers to limit unwanted communication

Hardware firewalls are known as the most basic way to protect against threats in the network. It inspects every data packet before it enters the network, software firewalls have the same functions as a hardware firewall, just not as a physical device. Instead, it's a software file saved on a computer, when downloaded, it will protect all devices connected to its server.

**Cloud-based firewalls**: Software firewalls that are hosted by a cloud service provider

**Stateful**: A class of firewall that keeps track of information passing through it and proactively filters out threats

**Stateless**: A class of firewall that operates on predefined rules and does not keep track of information from data packets

Stateless firewalls are regarded as more secure because it doesn't store or analyze information.

Benefits of next generation firewalls (NGFWs) - 

- Deep packet inspection
- Intrusion protection
- Threat intelligence

**Virtual Private Network (VPN)**: A network security service that changes your public IP address and hides your virtual location so that you can keep your data private when you are using a public network like the Internet

**Security zone**: A segment of a network that protects the internal network from the internet

**Network segmentation**: A security technique that divide the network into segments

**Uncontrolled zone**: Any network outside the organization's control

**Controlled zone**: A subnet that protects the internal network from the uncontrolled zone

**Proxy server**: A server that fulfills the request of a client by forwarding them onto other servers (uses temporary memory so that you don't need to go directly into the companies servers)

**Reverse proxy server**: regulates and restricts the Internets access to an internal server 

Common intrusion attacks

**Malware**: 

**Spoofing**: A network attack preformed when an attacker changes the source IP of a data packet to impersonate an authorized system and gain access to a network

**Packet sniffing**: 

**Packet flooding**: 

**Denial-of-service attack (DoS)**: An attack that targets a network or server and floods it with network traffic

**Distributed denial-of-service attack (DDoS)**: A type of denial-of-service attack that uses multiple devices or servers in different locations to flood the target network with unwanted traffic

**SYN (synchronize) flood attack**: A type of DoS attack that simulates a TCP connection and floods a server with SYN packets

**Internet Control Message Protocol (ICMP)**: An internet protocol used by devices to tell each other about data transmission errors across the network

**Internet Control Message Protocol (ICMP) flood**: A type of DoS attack preformed by an attacker repeatedly sending ICMP packets to a network server

**Ping of death**: A type of DoS attack caused when a hacker pings a system by sending it an oversized ICMP packet that is bigger than 64KB

**Passive packet sniffing**: A type of attack where data packets are read in transit

**Active packet sniffing**: A type of attack where data packets are manipulated in transit

**IP spoofing**: A network attack preformed when an attacker changes the source IP of a data packet to impersonate an authorized system and gain access to a network

**On-path attack**: An attack where a malicious actor places themselves in the middle of an authorized connection and interprets or alters the data in transit

**Replay attack**: A network attack preformed when a malicious actor intercepts a data packet in transit and delays it or repeats in at another times

**Smurf attack**: A network attack preformed when an attacker sniffs an authorized user's IP address and floods it with packets

Firewalls are a good way to protect against IP spoofing.

**Security hardening**: The process of strengthening a system to reduce its vulnerability and attack surface

**Security hardening is conducted on…**

- Hardware
- Operating systems
- Applications
- Computer networks
- Databases

**Penetration test**: A simulated attack that helps identify vulnerabilities in systems, networks, websites, applications, and processes

**Operating system (OS)**: The interface between computer hardware and the user

**Patch Update**: A software and operating system update that addresses security vulnerabilities within a program or product

**Baseline configuration (baseline image)**: A documented set of specifications within a system that is used as a basis for future builds, releases, and update

**Multi-factor authentication (MFA)**: A security measure which requires a user to verify their identify in two or more ways to access a system or network

Network security hardening

- Port filtering
- Network access privilege
- Encryption

Tasked performed

- Firewall rules maintenance
- Network log analysis
- Patch updates
- Server backups

**Security Information and Event Management tool (SIEM)**: An application that collects and analyzes log data to monitor critical activities in an organization

**Port filtering**: A firewall function that blocks or allows certain port numbers to limit unwanted communication

Cloud Network: A collection of servers or computers that stores resources and data in remote data centers that can be accessed via the internet

[A.I. Video Three](A%20I%20Video%20Three.md)
