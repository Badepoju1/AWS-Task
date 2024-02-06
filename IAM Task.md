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
           

