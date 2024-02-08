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
            DevOps_User1
            DevOps_User2
       - Access Level: Administrator Access
       - Policy Attached: AdministratorAccess permission
       - Justification: Requires full access to manage and configure all AWS services.

 ## Steps Taken:

           1. Created a group in IAM named DevOps_Group.
           2. Assigned the AdministratorAccess policy to the DevOps_Group, granting administrative access.
           3. Created 2 IAM user accounts (DevOps_User1 and DevOps_User2), then added users to the DevOps_Group to enable them to perform administrative tasks.

## Task 2 Development Group Configuration
         
        **Group Details
 
       - Group Name: Development
       - Users Added:
            Dev_User1
            Dev_User2
            Dev_User3
            Dev_User4
       - Access Level: Full access to Amazon S3 and DynamoDB services, along with the ability to start EC2 instances without the permission to stop them.
       - Policy Attached: AmazonS3FullAccess, AmazonDynamoDBFullAccess and EC2StartOnlyPolicy permission.
       - Justification: Requires access to work with S3 and DynamoDB for development purposes, as well as the ability to start EC2 instances for testing.

 ## Steps Taken:

           1. Created a group in IAM named Development_Group.
           2. Created policy called EC2StartOnlyPolicy (which allows user to only start EC2 instances)
           3. Assigned the AmazonS3FullAccess, AmazonDynamoDBFullAccess and EC2StartOnlyPolicy permission.
           4. Created 4 IAM user accounts (Dev_User1, Dev_User2, Dev_User3 and Dev_User4), then added the users to the Development_Group to enable them have access to the services. 
          
           

## Task 3 Sales-marketing Group Configuration
         
        **Group Details
 
       - Group Name: Sales-marketing
       - Users Added:
            Sale_User1
            Sale_User2
            Mar_User1
            
       - Access Level: Read-only access to the S3 services.
       - Policy Attached: AmazonS3ReadOnlyAccess 
       - Justification: Requires access to read documents and files stored on the S3 services

 ## Steps Taken:

           1. Created a group in IAM named Sales-marketing_Group.
           2. Assigned the AmazonS3ReadOnlyAccess permission
           3. Created 3 IAM user accounts (Sale_User1, Sale_User2 and Mar_User1), then added the users to the Sales-marketing to enable them have access to the services. 


## Task 4 Finance-Accounting Group Configuration
         
        **Group Details
 
       - Group Name: Finance-Accounting
       - Users Added:
            Fin_User1
                        
       - Access Level: Access to view account activity and usage reports.
       - Policy Attached: AWSAccountUsageReportAccess permissions 
       - Justification: Requires access to read documents and files stored on the S3 services

 ## Steps Taken:

           1. Created a group in IAM named Finance-Accounting_Group.
           2. Assigned the AmazonS3ReadOnlyAccess permission
           4. Created 1 IAM user accounts (Fin_User1), then added the users to the Finance-Accounting to enable them have access to the services. 
          