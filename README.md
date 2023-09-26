# Netpractice
This project is a general practical exercise to discover networking.

## TCP (Transmission control protocol)
### Transport Layer
TCP (Transmission Control Protocol) is one of the core protocols of the TCP/IP network protocol suite. It provides reliable, connection-oriented communication between devices over an IP network. TCP ensures that data packets are delivered in the correct order and without errors. Here are some key aspects of TCP:
### 1.Connection-oriented:
TCP establishes a connection between two devices before data transmission. This connection is a virtual communication channel that allows reliable and ordered data transfer.
### 2.Reliability:
TCP guarantees reliable data delivery. It achieves this through mechanisms such as acknowledgment, retransmission, and error detection. When a sender sends a segment, it waits for an acknowledgment from the receiver. If no acknowledgment is received within a specified time, the sender retransmits the segment.
### 3.Flow control:
TCP performs flow control to prevent a fast sender from overwhelming a slow receiver. It uses a sliding window mechanism to dynamically adjust the amount of data that can be sent before receiving acknowledgments.
### 4.Congestion control:
CP employs congestion control mechanisms to manage network congestion and prevent network overload. It dynamically adjusts the transmission rate based on network conditions to maintain optimal performance.
### 5.Full-duplex communication:
TCP supports full-duplex communication, allowing simultaneous bi-directional data transfer. Each connection consists of two communication channels, one for data transmission in each direction.
### 6.Segmentation and reassembly:
TCP breaks the data stream into smaller units called segments for transmission. It reassembles these segments at the receiving end to reconstruct the original data stream.
### 7.Port numbers:
TCP uses port numbers to identify specific applications or services running on devices. Port numbers allow multiple applications to use TCP simultaneously on the same device.
### 8.Three-way handshake:
Before data transmission begins, TCP establishes a connection using a three-way handshake. This involves a series of messages exchanged between the sender and receiver to synchronize sequence numbers and establish communication parameters.
### 9.Connection termination:
TCP ensures a reliable connection termination process. It uses a four-way handshake to gracefully close the connection, allowing both sides to acknowledge the termination and complete any remaining data transfers.

##IP:
IP (Internet Protocol): IP is responsible for addressing and routing packets of data across networks. It provides the basic structure and rules for transmitting data packets from a source IP address to a destination IP address. IP is a connectionless protocol, which means it does not establish a dedicated connection before sending data. Instead, each packet is treated independently and can take different paths to reach its destination. IP is designed to work with other protocols, such as TCP, to enable communication between devices on a network.

##UDP vs TCP
On the other hand, UDP is a simpler and connectionless protocol that operates at the transport layer of the TCP/IP protocol suite. Unlike TCP, UDP does not establish a connection before transmitting data and does not provide the same level of reliability and error-checking mechanisms. UDP is often referred to as a "fire and forget" protocol because it sends packets without worrying about acknowledgment or retransmission. It is faster and more lightweight than TCP but offers no guarantees regarding packet delivery, ordering, or integrity. UDP is commonly used for applications where speed and reduced overhead are more important than reliability, such as real-time streaming, online gaming, DNS (Domain Name System), and VoIP (Voice over IP).

In summary, the main differences between TCP/IP and UDP are:

Connection-oriented vs. connectionless: TCP is connection-oriented, establishing a reliable connection before transmitting data, while UDP is connectionless, sending packets without establishing a connection.

Reliability: TCP provides reliable data delivery with error-checking, retransmission, and ordered packet delivery. UDP does not guarantee reliability and does not include built-in mechanisms for error recovery or ordering.

Overhead: TCP has more overhead due to its reliability mechanisms, while UDP has less overhead, making it faster and more efficient.

The choice between TCP and UDP depends on the specific requirements of the application. If reliability and accuracy are crucial, TCP is preferred. If speed and low latency are more important, UDP may be a better choice.

##ROUTER and SWITCH

A router and a switch are both networking devices used in computer networks, but they serve different purposes and are used in different scenarios.

###Router: A router is a networking device that connects multiple networks together and forwards data packets between them. It operates at the network layer (Layer 3) of the OSI (Open Systems Interconnection) model. Routers are commonly used in homes, offices, and internet service providers (ISPs) to enable communication between devices on different networks, such as connecting a local network to the internet.

Key functions of a router include:

Packet forwarding: Routers examine the destination IP address of incoming packets and determine the best path to forward them to their destination across different networks. They maintain routing tables to make these forwarding decisions.

Network address translation (NAT): Routers can perform NAT, which allows multiple devices on a local network to share a single public IP address. NAT translates private IP addresses used within the local network to the public IP address when communicating with devices on the internet.

Firewall: Routers often include firewall capabilities to provide security by filtering incoming and outgoing network traffic based on predefined rules.

DHCP server: Routers can act as DHCP (Dynamic Host Configuration Protocol) servers to assign IP addresses and other network configuration parameters to devices on the local network.

###Switch: A switch is a networking device that connects multiple devices within a local area network (LAN). It operates at the data link layer (Layer 2) of the OSI model. Switches are commonly used in homes, offices, and data centers to facilitate communication between devices within the same network.

Key functions of a switch include:

Frame forwarding: Switches examine the destination MAC address of incoming Ethernet frames and forward them to the appropriate port based on the MAC address table. This allows devices to communicate directly with each other within the same network without requiring all devices to receive every network packet.

MAC address learning: Switches dynamically build and update the MAC address table by learning the MAC addresses of devices connected to each port. This helps the switch determine the correct port to forward frames to based on the destination MAC address.

VLAN support: Switches often support virtual LANs (VLANs) to logically segregate devices into different broadcast domains. VLANs provide improved security, performance, and flexibility by separating network traffic.

Quality of Service (QoS): Switches may support QoS features to prioritize certain types of traffic, such as voice or video data, to ensure better performance for time-sensitive applications.

In summary, routers are used to connect multiple networks together, such as connecting a local network to the internet, while switches are used to connect multiple devices within a single network. Routers operate at the network layer and forward packets between networks, while switches operate at the data link layer and facilitate communication within a network.
