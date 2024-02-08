# AWS-Task

For My AWS Projects Documentation

### AWS IAM Configuration Documentation

Introduction

This document outlines the steps taken to configure AWS Identity and Access Management (IAM) for different departmental groups within our organization, ensuring appropriate access levels as per their operational needs.

## Objective

to configure AWS IAM (Identity and Access Management) to establish secure access protocols for different departments within our organization, ensuring appropriate access levels are granted according to departmental functions and responsibilities.


## Task 1 DevOps Group Configuration
         
        **Group Details
 
       - Group Name: DevOps
       - Users Added:
            User1
            User2
       - Access Level: Administrator Access
       - Policy Attached: AdministratorAccess
       - Justification: Requires full access to manage and configure all AWS services.

 ## Steps Taken:

           1. Created a group in IAM named DevOps_Group.
           2. Assigned the AdministratorAccess policy to the DevOps_Group, granting administrative access.
           3. Created two IAM user accounts (User1 and User2).
           4. Added User1 and User2 to the DevOps_Group to enable them to perform administrative tasks.

## Task 2 Development Group Configuration
         
        **Group Details
 
       - Group Name: Development
       - Users Added:
            User1
            User2
            User3
            User4
       - Access Level: Full access to Amazon S3 and DynamoDB, along with the ability to start EC2 instances without the permission to stop them.
       - Policy Attached: Custom policies granting access to S3, DynamoDB, and limited access to EC2 services.
       - Justification: Requires access to work with S3 and DynamoDB for development purposes, as well as the ability to start EC2 instances for testing.

 ## Steps Taken:

           1. Created a group in IAM named Development_Group.
           2. Created policy called EC2StartOnlyPolicy (which allows user to only start EC2 instances)
           3. Assigned the AmazonS3FullAccess, AmazonDynamoDBFullAccess and EC2StartOnlyPolicy
           4. Created two IAM user accounts (User1, User2, User3 and User4), then added the user to the Development_Group to enable them have access to the services. 
          
           

