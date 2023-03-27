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
