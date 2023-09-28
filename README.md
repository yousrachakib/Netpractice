# Netpractice
This project is a general practical exercise to discover networking.

## OSI Model (Open Systems Interconnection model)
 ### Purpose of Networking:
 .Allow two hosts to share data with one another.
 ### Hosts must follow set of rules :
  .The rules for networking are divided into seven layers:
## OSI Model :
  .each layer serves a specific function.
  .if all layer are functionning, hosts can share data
  ### Physical Layer: (transporting bits)
      => Computer data exists in the form of Bits (1's and 0's)
      => Someting has to transport those bits between hosts
      => L1 Technologies does the job : Cables (twisted pair, coaxial, fiber),           Wifi, Repeaters.
  ### Data Link Layer : (Hop to hop delivery)
      => Interact with the wire (physical layer)
      => NIC-Network Interface Cards / Wifi Acess Card
      => Hop to hop using Adressing Scheme - MAC adresses
      => L2 Technologies : NIC's , Switches
      => Often communication between hots require multiple hops
  ### Network Layer : (End to end delivery)
      => Adressing Scheme - IP Adresses
      => IP adress : 32bits, represented as 4 octets , each 0-255
      => L3 Technologies : Routers, Hosts, (anything with an IP)
*****>>  What L3 does add the source IP address and the destination to a data sent by an APP then L2 adds the source MAC adress and the destination MAC <<*****

  ### Transport Layer : (Service to service)
      => Distinguish data streams
      => Adressing scheme - Ports
       ** 0 - 65535 TCP
       ** 0 - 65535 UDP
      => Clients select random Port for each connection
       ** Response traffic will arrive on this port
  ### Layer 5,6,7 - Session, Presentaion, Application :
      => Distinction in these layers is somewhat vague 
 *****>> the process of Sending is called - Encapsulation , on the other hand the process of Receiving is called De-capsulation <<*****
  ### Subnet Mask Definition :
     => A subnet mask is a 32-bit value used in IP (Internet Protocol) networking to divide an IP address into a network portion and a host portion. 
     It helps determine which part of an IP address represents the network ID and which part represents the host ID.
 ### IP Adress :
     => In IPv4, an IP address is a 32-bit binary number typically represented in decimal form, separated into four octets.
 *****>> When an IP address and subnet mask are bitwise ANDed together, the result is the network ID. The remaining bits represent the host ID. <<*****
 
     => The subnet mask helps determine the range of IP addresses that belong to the same network.
     => Subnet masks are primarily used for subnetting, which involves dividing a large network into 
     smaller logical subnetworks (subnets) for more efficient use of IP addresses and improved network management.
 ### Private Networks range : (Private networks use IP addresses from specific ranges that are reserved for internal use and are not routable on the public internet.)
     => 10.0.0.0 to 10.255.255.255 (10.0.0.0/8)
     => 172.16.0.0 to 172.31.255.255 (172.16.0.0/12)
     => 192.168.0.0 to 192.168.255.255 (192.168.0.0/16)
 ### Local IP range (special range reserved for loopback addresses in IPv4 used to test network connectivity on an individual device without actually sending data over a physical network.):
     => 127.0.0.1 to 127.255.255.254
### Router and switch :
     => Router: A router is a networking device that connects multiple networks together and forwards data packets between them.
     => Switch :A switch is a networking device that connects multiple devices within a local area network (LAN).
