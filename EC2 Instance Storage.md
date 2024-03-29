## EBS Volume :
  Elastic Block Storage Volume is network drive which you can attach to your instances when they are running.<br>
  Its bound within single AZ (if EBS is created on one AZ , it cannot be used in another AZ)<br>
  They can mounted to one instance at time (CCP level). It allows to persist your data after termination of instances.<br>

![EBS Volume]()

Delete on Termination attribute determines behavior of EBS volume when its terminated.<br>
It's ON for root EBS volume and user created EBS volume can be select its own behavior<br> 

## EBS Snapshots :
It is backup option for EBS Volumes. We can create a snapshot of data and use it for backup purposes.<br>
After creating snapshot , you can re create the setup in another AZ's also.<br>
![EBS Features]()

## Amazon Machine Images :
AMI's are customized EC2 instance where you select from AWS made AMI/from AWS Marketplace (sold by some other AWS users)/ you can create your own AMI.<br>
Own AMI will be having faster reboot time because everything needed will be configured while creating AMI itself.
AMI Process :
1. Create a instance and customize it
2. Stop instance
3. Build AMI - EBS Snapshot
4. Launch instance from AMI's

## EC2 Instance Store :
Its temporary cache storage to EC2 instance which can be used for high performance/high speed IOPS.<br>
EC2 Instance store has IOPS levels upto 3.3 million read IOPS and 1.4 million IOPS.<br>
Once instance is terminated , data will be lost. So backup and replication should be taken care.<br>

## EBS Volume Types :
General Purpose SSD :
1. Cost effective , low latency upto 3000 IOPS
2. Used for development enviroments
3. 1 GiB - 16 TiB

Provisioned IOPS :<br>
io1/io2 : 
1. Used for applications having more than 16000 IOPS.
2. 4TiB - 16TiB
3. Max PIOPS - 64k for Nitro & 32 k for others
io2 Block Express :
1. size - 4 TiB to 16 TiB
2. Max PIOPS - 2,56,000

Hard Disk Drive (HDD)
1. Can't be boot volume
2. 125GiB - 16TiB
   
![EBS - HDD](https://github.com/arjun1131/AWS-SAA-C-03-Notes/blob/main/AWS%20Images/EBS%20-%20HDD.png)

## EBS  Multi Attach :
1. This type of EBS can attached to multiple EC2 which is on same AZ's.
2. Each instance has full read and write permissions on EC2 intance which they connected with
3. Use case - Teradata , managing concurrent read and write transactions.

## EFS - Elastic File System :
It's a network file system which can be mounted on EC2 instance.
It can work on EC2 instance in different AZ's
Expensive(3*gp2) instance , pay per use.



