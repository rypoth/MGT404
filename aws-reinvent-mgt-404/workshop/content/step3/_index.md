+++
title = "Resource Groups"
date = 2019-07-08T13:08:10+01:00
weight = 2
chapter = true
pre = "<b>2 </b>"
draft = false
+++

## Resource Group

What Are Resource Groups?

In AWS, a resource is an entity that you can work with.
Examples include an Amazon EC2 instance, an AWS CloudFormation stack, or an Amazon S3 bucket.
If you work with multiple resources, you might find it useful to manage them as a group rather than move from one AWS service to another for each task.
If you manage large numbers of related resources, such as EC2 instances that make up an application layer, you likely need to perform bulk actions on these resources at one time.

Examples of bulk actions include:
•	Applying updates or security patches.
•	Upgrading applications.
•	Opening or closing ports to network traffic.
•	Collecting specific log and monitoring data from your fleet of instances.

A resource group is a collection of AWS resources that are all in the same AWS region, and that match criteria provided in a query.
In Resource Groups, there are two types of queries on which you can build a group.
Both query types include resources that are specified in the format AWS::service::resource.

•	Tag-based
Tag-based queries include lists of resources and tags. Tags are keys that help identify and sort your resources within your organization. Optionally, tags include values for keys.

•	AWS CloudFormation stack-based
In an AWS CloudFormation stack-based query, you choose an AWS CloudFormation stack in your account in the current region, and then choose resource types within the stack that you want to be in the group. You can base your query on only one AWS CloudFormation stack.
Resource groups can be nested; a resource group can contain existing resource groups in the same region
