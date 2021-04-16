THREE DIFFERENT COMPANIES NETWORKING DESIGN 

I designed this **network configuration for the network of three companies**, given some constraints. This problem was presented in our  Computer Networks Lab (CL307) Final. The main role was to **subnet the IP addresses** correctly.

Its an interesting problem demonstrating the concepts of **Classless IP Subnetting** and using **RIPv2 Protocol**. I am sharing this **working solution** so that it might be of help to others looking to learn these concepts with a practical real world example.


INTRODUCTION 
 
Without a proper network design between Different Companies in partnership with each other, poor linkage takes place and there comes the communicating barriers and problems between different departments of the companies while sending the data. So a manual procedure is followed to send the data (documents, applications etc).
 
1.1 	Problem Statement 
 
                   Any employee who needed to share web, information or to send any record, due to no or poor linkage between different systems in all departments of companies one must go from one department to another or one company to other for this purpose. Resulting in inaccuracy, time and cost inefficiency. 
 
1.2 	Aims & Objectives 
Our aim is to Network design for Three different Companies to overcome the linkage barrier so that data sharing will be held between departments and between companies via networking.
Our objective is to use the Cisco Packet Tracer tool to design the Companies network.
            
1.3 	Tools used/to be used for implementation 
 
 
⦁	Cisco Packet Tracer 7.0 (Networking software) 
⦁	High quality fiber optic cables, Routers, Switches (Hardware Requirements) 
CHAPTER 2:
METHODOLOGY

 

RIPv2 Protocol
RIPv2 is a classless, distance vector routing protocol as defined in RFC 1723. Being a classless routing protocol, means, it includes the subnet mask with the network addresses in its routing updates.
As with other classless routing protocols, RIPv2 supports CIDR supernets, VLSM and discontiguous networks.

Working 
The companies are named as SCP X, SCP Y and SCP Z.
⦁	SCP X has 5 Rooms with 1 PC in each room.
⦁	SCP Y has 3 Rooms with 3 PCs in each room.
⦁	SCP Z has 2 Rooms with 4 PCs in each room.
We have assigned the following IP network addresses to each of the company:
⦁	SCP X: 144.186.96.0/19
⦁	SCP Y: 50.152.0.0/15
⦁	SCP Z: 210.98.169.64/26
All the PCs in a single room are on the same sub network and all the rooms of a single company are on a different sub-network which are assigned after sub-netting the assigned network address only for the relevant company (no outside network or the network of other company is accepted) e.g, each room for SCP X is assigned a different sub-network after sub-netting the address of 144.186.96.0/19 only and not any other network address. The companies can extend the number of their PCs in each room in the future.
We, begun cleverly economical, decide to install old switces (Generic Switches in Cisco Packet Tracer) with only three Ethernet ports working out of four and routers (Generic Routers in Cisco Packet Tracer) to configure the network for three companies in such a way that you use as much less routers and switches as possible.
We have also the IP network address for the serial communication between different routers which connect different Inter-Company and Intra-Company subnets. We formed the subnets of the following address in order to cater the serial communication between all the routers: Routers Serial Communication: 199.210.121.160/28
Constraints
We, being very cautious, decide to simulate the topology on Cisco Packet Tracer in order to optimally design the network considering the number of devices (switches, routers etc.) used to maximize the profit margins of our company. However, we have simulated the topology strictly following rules and regulations described below:
1- Used Straight Through wires, Cross Over cables or Serial DCE wires where necessary and applicable.
2- Used Generic Router and Generic PCs for your design
3- Used Generic Switches such that we attach only 3 of the 4 available Ethernet Interfaces for a single switch, however, we could have attached as many switches considering optimal design.
4- We assigned IPs to the PCs using Static IP allocation.
5- Although We have to used GUI of the router to configure its interfaces but we also used CLI of the router to configure the RIPv2 Protocol for Classless Subnet Addressing.


TOPOLOGY
![a](../master/network-screenshot.PNG)

CONCLUSION
 
Arrange design and its security are essential for any association. On the off chance that we take after the various leveled arrange configuration, system will be versatile, execution and security will be expanded, and the system will be anything but difficult to keep up. In this work, we proposed a minimal financially savvy secure grounds organize configuration in view of the workplace of different companies with their departments and required adaptability, security and different perspectives. 
  
REFERENCES 
⦁	www.cisco.com
⦁	https://www.orbit-computer-solutions.com/ripv2/#:~:text=RIPv2%20is%20a%20classless%2C%20distance,supernets%2C%20VLSM%20and%20discontiguous%20networks.

## How to Run
Install [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer) and then simply open the [main file.pkt](../master/main/main%20file.pkt). The whole network is in working condition. You can check it by sending a packet from one system to another or through using the PING command in the Cisco Packet Tracer.

This solution works for version 6.2 or above of Cisco Packet Tracer.
