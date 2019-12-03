+++
title = "Prerequisites"
date = 2019-07-08T13:08:10+01:00
weight = 1
chapter = true
pre = "<b>1 </b>"
draft = false
+++

## PREREQUISITES

CloudWatch Application Insights for.NET and SQL Server supports:
•	Front‐end: Microsoft Internet Information Services (IIS) Web Server
•	Worker-tier: .NETCore
•	Worker‐tier: .NET Framework
•	Database: Microsoft SQL Server running on RDS or EC2
https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/appinsights-what-is.html

Each EC2 Instance in your application stack must have the latest SSM Agent installed.
Create the following IAM Policy and attach it to the EC2 Instance at launch.
```
    {
        "Version": "2012-10-17",
          "Statement": [
            {
                "Action": [
                    "applicationinsights:*",
                    "iam:CreateServiceLinkedRole",
                    "iam:ListRoles"
                          ],
                  "Effect": "Allow",
                  "Resource": "*"
              }
                          ]
      }
```
