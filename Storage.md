# Storage Types:

Generally , storage are broadly classified into
1. File Storage - Files are organized in a tree-like hierarchy that consists of folders and subfolders. 
2. Object Storage - Block storage splits files into fixed-size chunks of data called blocks that have their own addresses. Since each block is addressable, blocks can be retrieved efficiently.
3. Block Storage - treated as a single unit of data when stored.

## Amazon EC2 Storage Types

1. EC2 instance store
2. EC2 block store

## Amazon EC2 instance store:
1. It provides temporary block storage to EC2 instance.
2. Lifecycle of instance store ties with lifecycle of EC2 instance.
3. Instance store is considered **ephemeral storage**
4. Having the speed of locally attached volumes and the resiliency of replicated data helps you achieve data distribution at high performance.

## Amazon Elastic Block Storage (Amazon EBS):
1. It's external storage which can be added to EC2 instance.
2. Most Amazon EBS volumes can only be connected with one computer at a time. Most EBS volumes have a one-to-one relationship with EC2 instances, so they cannot be shared by or attached to multiple instances at one time.
3. Scaling can be happen in two ways.<br>
  a. Increase the volume size, as long as it doesn’t increase above the maximum size limit.<br>
  b. Attach multiple volumes to a single Amazon EC2 instance. <br>
4. EBS has two types of storages<br>
  a. HDD backed EBS<br>
  b. SSD backed EBS<br>
  
  ![EBS Types](https://github.com/arjun1131/AWS-SAA-C-03-Notes/blob/main/AWS%20Images/EBS_Types.png)
  
  

