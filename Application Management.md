#### Benefits of Monitoring :<br>
1. Respond to operational issues proactively before your end users are aware of them.<br>
2. Improve the performance and reliability of your resources.<br>
3. Recognize security threats and events.<br>
4. Make data-driven decisions for your business.<br>
5. Create more cost-effective solutions.<br>

For monitoring , AWS has application named **"Amazon CloudWatch"** <br>
Amazon CloudWatch is a monitoring and observability service that collects data & provides actionable insights into your applications, and enables you to respond to system-wide performance changes, optimize resource usage, and get a unified view of operational health.<br>

![CloudWatch Working](https://github.com/arjun1131/AWS-SAA-C-03-Notes/blob/main/AWS%20Images/CloudWatch.PNG)

#### Use cases of CloudWatch:<br>
1. Detect anomalous behavior in your environments<br>
2. Set alarms to alert you when something is not right<br>
3. Visualize logs and metrics with the AWS Management Console<br>
4. Take automated actions like scaling<br>
5. Troubleshoot issues<br>
6. Discover insights to keep your applications healthy<br>

**All instance level metrics will be collected by CloudWatch automatically**<br>

**Custom metrics** will publish our own metrics.<br>
Examples of Custom metrics :<br>
1. Web page load times<br>
2. Request error rates<br>
3. Number of processes or threads on your instance<br>
4. Amount of work performed by your application<br>

## CloudWatch Dashboards:
Dashboards are customizable home pages that you use for data visualization for one or more metrics through the use of widgets, such as a graph or text.<br>
CloudWatch aggregates statistics according to the period of time that you specify when creating your graph or requesting your metrics. You can also choose whether your metric widgets display live data. Live data is data published within the last minute that has not been fully aggregated.<br>
You can control who has access to view or manage your CloudWatch dashboards through AWS Identity and Access Management (IAM) policies that get associated with IAM users, IAM groups, or IAM roles.<br>

## CloudWatch Logs:
CloudWatch Logs can monitor, store, and access your log files from applications running on Amazon EC2 instances, AWS Lambda functions, and other sources.<br>
CloudWatch Logs allows you to query and filter your log data. You also set up metric filters on logs, which turn log data into numerical CloudWatch metrics that you can graph and use on your dashboards.<br>
#### Terminology used in Logs:
Log event: A log event is a record of activity recorded by the application or resource being monitored, and it has a timestamp and an event message.<br>
Log streams : It's group of log events which belongs to same resource.<br>
Log groups: It's group of log streams of resources which has same permission settings.<br>


## CloudWatch alarms:
It can automatically initate a trigger or sending out information to certain admins when any metric is crossing its threshold value.
It has three stages<br>
1. OK - Everything on that particular metric is smooth<br>
2. Insufficient - state where CloudWatch don't have data to decide anything <br>
3. In alarm - Particular metric is gone behind threshold value given.<br>

To improve application availability , we should avoid single point of failure by adding another instance in another AZ.<br>
Scaling of EC2 instance can be done in two ways.<br>
1. Horizontal - Adding n number of instances<br>
2. Vertical - Increasing EC2 instance size<br>

### Load Balancing :

![Load Balancer](https://github.com/arjun1131/AWS-SAA-C-03-Notes/blob/main/AWS%20Images/Load%20Balancer.PNG)

Load balancer is used to send requests to instances with respect of their load status.
There are 3 load balancer 
1. Application Load Balancer - Works on application layer (http/https) 
2. Network Load Balancer - Works on Network layer(TCP/IP/TLS)
3. Gateway Load balancer - Works on Gateway level


