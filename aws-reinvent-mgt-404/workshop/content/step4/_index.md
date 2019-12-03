+++
title = "Setting up an Application"
date = 2019-07-08T14:37:08+01:00
weight = 4
chapter = false
pre = "<b>4 </b>"
draft = false
+++

##  Setting up an Application

You can view the official documentation at https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/appinsights-setting-up.html

In this step we are going to setup an application that we will use in our Application Insights for .NET & SQL Server demo.

•	From the AWS Management Console, Open the **CloudWatch** console landing page.
•	From the left navigation pane, choose **Settings**.
•	From the Settings page, choose **Application Insights for .NET and SQL Server** > **View applications** to get started.

![Application Insights](images/image3.png)

Click the **Add an Application** button

![Add an Application](images/image35.png)

On the **Add an Application** screen select the drop down to *Choose Resource Group* and add the **Resource Group** that you created in Step 2 of this guide.

Finally, click the Add Application button.

On the next screen, Application Insights will show you the individual components that make up your application stack inside your Resource Group.

![Overview](images/image5.png)

Select one of the EC2 Instances that make up your application stack and click the Manage Monitoring button.

![Enable Monitoring](images/image6.png)

Click **Enable Monitoring** and then Select one of the following Application Tier Components you wish to monitor -
![Components](images/image7.png)

Application Insights will then provide you a base level of monitoring dependent on your selection.  
You have the ability in each section to change existing or add additional logs or events and metrics.

![Logs](images/image8.png)

Click the **Save** button once you have added the monitoring you require.
On the Applications Monitored screen, Select your Resource Group and Click **View Insights**

Application Insights for .NET and SQL Server provides you with meaningful data that helps you reduce the MTTR (Mean Time to Repair), for your application stacks running on the AWS Cloud.
