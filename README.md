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

      
