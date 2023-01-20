Networking is how you connect another computer with another set of computers and communicate with them.
Routing is process of selecting a path across one or more networks.

**IPv4 notation :**
The 32 bits are grouped into groups of 8 bits, also called octets. Each of these groups is converted into decimal format separated by a period.
We need this to when we try to communicate.

## Classless Inter-Domain Routing:

CIDR notation specifies an IP address, a slash ('/') character, and a decimal number. The decimal number is the count of consecutive leading 1-bits (from left to right) in the network mask. The number can also be thought of as the width (in bits) of the network prefix. The IP address in CIDR notation is always represented according to the standards for IPv4 or IPv6. 
The number of addresses inside a network or subnet may be calculated as 2^address length − prefix length^, where address length is 128 for IPv6 and 32 for IPv4.

## Amazon Virtual Private Cloud :

For creating Amazon VPC , we need to declare two things.
1. Region
2. IP Range

Inside VPCs, we will having subnets. Subnets are used to give granual controls to resources. We need 3 things to create subnets
1. IP Range(Subset of VPC IP)
2. VPC
3. Availability Zones

**Internet Gateway :** For connecting with Internet , we need Internet Gateway and it should be attach with VPC.

**Virtual Private Gateway :** A virtual private gateway connects your AWS VPC to another private network. Once you create and attach a virtual private gateway to a VPC, the gateway acts as anchor on the AWS side of the connection. A customer gateway device is a physical device or software application on your side of the connection

For accessing correct subnets, we need to create route table which has rules for subnets 
