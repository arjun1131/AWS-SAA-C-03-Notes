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





