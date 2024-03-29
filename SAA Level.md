### Public IP : <br>
  IP address which can be located in Internet and open to anyone.<br>
  
### Private IP :<br>
  IP address which can be communicate within themselves and connect to Internet through NAT device or Internet Gateway.<br>
  
### Elastic IP :<br>
  It's a public IP which is within Amazon's IP pool which can associated to instance or network device till its deletion.<br>
  
### EC2 Placement Groups :<br>
1. Cluster - The placement group is used for low latency and high network throughput applications.<br>
The risk of single point of failure increases in this placement group. If rack goes down, the entire set of instances will go down.<br>

![Cluster](https://github.com/arjun1131/AWS-SAA-C-03-Notes/blob/main/AWS%20Images/Cluster.PNG)

2. Spread :<br>
  The placement group is used in cases of high availability and critical applications where it must be isolated from single point of failure.<br>
  
  ![Spread](https://github.com/arjun1131/AWS-SAA-C-03-Notes/blob/main/AWS%20Images/Spread.PNG)
  
3. Partition :<br>
   It's used as partitions in AZ's . Upto 7 partitions we can create in single AZ's<br>
   A partition can hold upto 100s of EC2 instances.<br>
   Instance in partition won't share physical rack.<br>
   
  ![Partition](https://github.com/arjun1131/AWS-SAA-C-03-Notes/blob/main/AWS%20Images/Partition.PNG)
