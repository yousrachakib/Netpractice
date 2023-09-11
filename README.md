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

