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
  
  ## Amazon S3 :
  
  In S3, containers are called as buckets. Before adding data , we have to create buckets first.<br>
  You need two details to create bucket – the AWS Region you want the bucket to reside in and the bucket name.<br>
  Level of redundancy is designed to provide Amazon S3 customers with 99.999999999% durability and 99.99% availability for objects over a given year.<br>
  
  ![S3 URL](https://github.com/arjun1131/AWS-SAA-C-03-Notes/blob/main/AWS%20Images/S3%20URL.png)
  
  Every thing in S3 is private. If you want to make it public, you have to add it as public resource where everyone in internet can see.
  
  ### Amazon S3 encryption:
  **Server-side encryption:** This allows Amazon S3 to encrypt your object before saving it on disks in its data centers and then decrypt it when you download the objects.<br>
  **Client-side encryption:** You can encrypt your data client-side and then upload the encrypted data to Amazon S3. In this case, you manage the encryption process, the encryption keys, and all related tools.<br>
  
  ### Amazon S3 versioning:
  If you don’t use Amazon S3 versioning, every time you upload an object called employee.jpg to the employees folder, it will overwrite the original file.<br>
  If you enable versioning for a bucket, Amazon S3 automatically generates a unique version ID for the object.<br>
  Buckets can be in one of the following three states:<br>
    1. Unversioned (default): No new and existing objects in the bucket have a version.<br>
    2. Versioning-enabled: Versioning is enabled for all objects in the bucket.<br>
    3. Versioning-suspended: Versioning is suspended for new objects. All new objects in the bucket will not have a version. However, all existing objects keep their object versions.<br>
  

