# Serverless Computing Services

In serverless computing , you don't need to think about your underlying implementation like OS, Hardware. You need to take care of hosting your application.
On Shared security responsibility model, AWS will take care of till OS patching , firewall maintainence but still you have to take care of data encryption and access management

One such serverless computing service is **AWS Lambda**

## AWS Lambda :
Lambda is one of serverless service available in AWS.
You just need to upload source code and Lambda takes care of rest of things. 
For creating successful Lambda function , you need source code , trigger and configuration.

**Picture need to be inserted - AWS Lambda Working Explanation**

**Code** can be created by three ways
1. You can create from scratch.
2. You can use a blueprint of AWS
3. You can use from Amazon Serverless Application repo

**Trigger** should be given to initate Lambda function. 
A trigger integrates your Lambda function with other AWS services, enabling you to run your Lambda function in response to certain API calls that occur in your AWS account.
This increases your ability to respond to events in your console without having to perform manual actions.

**Picture to be inserted - AWS Lambda Explanation**

AWS Lambda function handler is method which invokes Lambda function once it receives trigger.
When your function is invoked, Lambda runs the handler method. When the handler exits or returns a response, it becomes available to handle another event. 

### Lambda function Naming :
The name of Lambda function will be derived from two things
1. Name of the file in which the Lambda handler function is located
2. Name of the Python handler function
For example : resize.lambda_function where resize is name of file location & lambda_function is name of python function.

It has 1ms billing granularity.




