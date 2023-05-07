## EBS Volume :
  Elastic Block Storage Volume is network drive which you can attach to your instances when they are running.<br>
  Its bound within single AZ (if EBS is created on one AZ , it cannot be used in another AZ)<br>
  They can mounted to one instance at time (CCP level). It allows to persist your data after termination of instances.<br>

![EBS Volume]()

Delete on Termination attribute determines behavior of EBS volume when its terminated.<br>
It's ON for root EBS volume and user created EBS volume can be select its own behavior<br> 
