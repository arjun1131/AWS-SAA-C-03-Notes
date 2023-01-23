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

For accessing correct subnets, we need to create route table which has rules for subnets. There are 2 route tables 
1. Main route table
2. Custom route table

### Main route table :
  When an Amazon VPC is created , it will create it a route table which contains set of rules called routes, that are used to determine where network traffic is directed.
  **The default configuration of the main route table is to allow traffic between all subnets in the local network**
  
  The destination and target are two main parts of this route table.

   1. The destination is a range of IP addresses where you want your traffic to go. In the example of sending a letter, you need a destination to route the letter to the appropriate place. The same is true for routing traffic. In this case, the destination is the VPC network's IP range.
   2. The target is the connection through which to send the traffic. In this case, the traffic is routed through the local VPC network.

### Custom route table :
  If you associate a custom route table with a subnet, the subnet will use it instead of the main route table. Each custom route table you create will have the local route already inside it, allowing communication to flow between all resources and subnets inside the VPC. The local route cannot be deleted.
  
  ![Route Tables](https://github.com/arjun1131/AWS-SAA-C-03-Notes/blob/main/AWS%20Images/Route%20tables.PNG)
  
  
