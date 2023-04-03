**Confidentiality** : Limiting access to authorized people, restricting access to unauthorized people.<br>
**Integrity** : It includes consistency, accuracy and trustworthiness of data.<br>
**Availability** : Readiness of information resources.<br>

## Security Design Principles :<br>

1. Implement a strong identity foundation - Grant access to data and other resources to only the people who really need that access.<br>
2. Enable traceability - Knowing what workloads are deployed and operational allows you to audit and ensure that the environment is operating at the security governance levels expected and demanded by the security standards.<br>
3. Apply Security at all levels - Should apply security protocols in all level (Application, Network, Data)<br>
4. Automate security best practices.<br>
5. Protect data in transit and at rest.<br>
6. Minimize your attack surface.<br>
7. Prepare for security events.<br>

# AWS Well Architected Framework:

The framework consists of six pillars 

![Framework](https://github.com/arjun1131/AWS-SAA-C-03-Notes/blob/main/AWS%20Images/6%20pillars%20of%20AWS.png)

## Security :<br>

The security pillar is made up of five different areas for security in the cloud. All AWS security services can be categorized by these five areas.

![Security](https://github.com/arjun1131/AWS-SAA-C-03-Notes/blob/main/AWS%20Images/AWS%20Security.png)

## Identity and Access Management :<br>

**Authentication** - Process of validating users are who they are claim to be. Ex : Logging into web by password<br>
**Authorization** - Process of giving the user permission to access a specific resource or function.<br>

# AWS Services for Identity & Access Management :

## AWS IAM :

1. IAM services are used to create roles , users and permissions. IAM users can be created from root account and users can use AWS services which they are authorized to. <br>
2. IAM provides the granularity to control a user’s access to specific AWS services and resources using permissions.<br>
3. Grant only least privilege to each IAM entity by starting with no access and gradually granting appropriate rights.<br>
4. IAM is integrated into most AWS services.<br>

## Amazon Cognito for Mobile Authencation :

1. Amazon Cognito is authencation service which used on mobiles, it creates unique pools and identity for users.<br>
2. Amazon Cognito supports MFA and encryption of data at rest and data in transit, meeting compliance requirements from several compliance organizations.<br>

![Cognito](
