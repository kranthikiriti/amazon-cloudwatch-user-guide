# Amazon CloudWatch User Guide

-----
*****Copyright &copy; 2019 Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

-----
Amazon's trademarks and trade dress may not be used in 
     connection with any product or service that is not Amazon's, 
     in any manner that is likely to cause confusion among customers, 
     or in any manner that disparages or discredits Amazon. All other 
     trademarks not owned by Amazon are the property of their respective
     owners, who may or may not be affiliated with, connected to, or 
     sponsored by Amazon.

-----
## Contents
+ [What is Amazon CloudWatch?](WhatIsCloudWatch.md)
   + [How Amazon CloudWatch Works](cloudwatch_architecture.md)
   + [Amazon CloudWatch Concepts](cloudwatch_concepts.md)
   + [Amazon CloudWatch Resources](RelatedResources.md)
+ [Getting Set Up](GettingSetup.md)
+ [Getting Started with Amazon CloudWatch](GettingStarted.md)
   + [See Key Metrics From All AWS Services](CloudWatch_Automatic_Dashboards_Cross_Service.md)
   + [Focus on Metrics and Alarms in a Single AWS Service](CloudWatch_Automatic_Dashboards_Focus_Service.md)
   + [Focus on Metrics and Alarms in a Resource Group](CloudWatch_Automatic_Dashboards_Resource_Group.md)
+ [Using Amazon CloudWatch Dashboards](CloudWatch_Dashboards.md)
   + [Create a CloudWatch Dashboard](create_dashboard.md)
   + [Add or Remove a Graph from a CloudWatch Dashboard](add_remove_graph_dashboard.md)
   + [Move or Resize a Graph on a CloudWatch Dashboard](move_resize_graph_dashboard.md)
   + [Edit a Graph on a CloudWatch Dashboard](edit_graph_dashboard.md)
   + [Graph Metrics Manually on a CloudWatch Dashboard](add_old_metrics_to_graph.md)
   + [Rename a Graph on a CloudWatch Dashboard](rename_graph_dashboard.md)
   + [Add or Remove a Text Widget from a CloudWatch Dashboard](add_remove_text_dashboard.md)
   + [Add or Remove an Alarm from a CloudWatch Dashboard](add_remove_alarm_dashboard.md)
   + [Monitor Resources in Multiple Regions Using a CloudWatch Dashboard](cross_region_dashboard.md)
   + [Link and Unlink Graphs on a CloudWatch Dashboard](link_unlink_graph_dashboard.md)
   + [Add a Dashboard to Your Favorites List](add-dashboard-to-favorites.md)
   + [Change the Period Override Setting or Refresh Interval for the CloudWatch Dashboard](change_dashboard_refresh_interval.md)
   + [Change the Time Range or Time Zone Format of a CloudWatch Dashboard](change_dashboard_time_format.md)
+ [Using Amazon CloudWatch Metrics](working_with_metrics.md)
   + [Viewing Available Metrics](viewing_metrics_with_cloudwatch.md)
   + [Searching for Available Metrics](finding_metrics_with_cloudwatch.md)
   + [Getting Statistics for a Metric](getting-metric-statistics.md)
      + [Getting Statistics for a Specific Resource](US_SingleMetricPerInstance.md)
      + [Aggregating Statistics Across Resources](GetSingleMetricAllDimensions.md)
      + [Aggregating Statistics by Auto Scaling Group](GetMetricAutoScalingGroup.md)
      + [Aggregating Statistics by Amazon Machine Image (AMI)](US_SingleMetricPerAMI.md)
   + [Graphing Metrics](graph_metrics.md)
      + [Graphing a Metric](graph_a_metric.md)
      + [Modifying the Time Range or Time Zone Format for a Graph](modify_graph_date_time.md)
      + [Modifying the Y-Axis for a Graph](switch_graph_axes.md)
      + [Creating an Alarm from a Metric on a Graph](create_alarm_metric_graph.md)
   + [Publishing Custom Metrics](publishingMetrics.md)
   + [Using Metric Math](using-metric-math.md)
   + [Using Search Expressions in Graphs](using-search-expressions.md)
      + [CloudWatch Search Expression Syntax](search-expression-syntax.md)
      + [CloudWatch Search Expression Examples](search-expression-examples.md)
      + [Creating a CloudWatch Graph with a Search Expression](create-search-expression.md)
+ [Using Amazon CloudWatch Alarms](AlarmThatSendsEmail.md)
   + [Set Up Amazon SNS Notifications](US_SetupSNS.md)
   + [Create a CloudWatch Alarm Based on a CloudWatch Metric](ConsoleAlarms.md)
   + [Create a CloudWatch Alarm Based on a Metric Math Expression](Create-alarm-on-metric-math-expression.md)
   + [Edit a CloudWatch Alarm](Edit-CloudWatch-Alarm.md)
   + [Create a CPU Usage Alarm that Sends Email](US_AlarmAtThresholdEC2.md)
   + [Create a Load Balancer Latency Alarm that Sends Email](US_AlarmAtThresholdELB.md)
   + [Create a Storage Throughput Alarm that Sends Email](US_AlarmAtThresholdEBS.md)
   + [Create Alarms to Stop, Terminate, Reboot, or Recover an Instance](UsingAlarmActions.md)
   + [Create a Billing Alarm to Monitor Your Estimated AWS Charges](monitor_estimated_charges_with_cloudwatch.md)
   + [Hide Amazon EC2 Auto Scaling Alarms](hide-autoscaling-alarms.md)
+ [Collecting Metrics and Logs from Amazon EC2 Instances and On-Premises Servers with the CloudWatch Agent](Install-CloudWatch-Agent.md)
   + [Installing the CloudWatch Agent](install-CloudWatch-Agent-on-EC2-Instance.md)
      + [Installing the CloudWatch Agent Using the Command Line](installing-cloudwatch-agent-commandline.md)
         + [Download and Configure the CloudWatch Agent Using the Command Line](download-cloudwatch-agent-commandline.md)
         + [Create IAM Roles and Users for Use With CloudWatch Agent](create-iam-roles-for-cloudwatch-agent-commandline.md)
         + [Installing and Running the CloudWatch Agent on Your Servers](install-CloudWatch-Agent-commandline-fleet.md)
      + [Installing the CloudWatch Agent Using SSM](installing-cloudwatch-agent-ssm.md)
         + [Create IAM Roles and Users for Use with the CloudWatch Agent](create-iam-roles-for-cloudwatch-agent.md)
         + [Download and Configure the CloudWatch Agent](download-CloudWatch-Agent-on-EC2-Instance-SSM-first.md)
         + [Installing the CloudWatch Agent on EC2 Instances Using Your Agent Configuration](install-CloudWatch-Agent-on-EC2-Instance-fleet.md)
         + [Installing the CloudWatch Agent on On-Premises Servers](install-CloudWatch-Agent-on-premise.md)
      + [Installing the CloudWatch Agent Using AWS CloudFormation](Install-CloudWatch-Agent-New-Instances-CloudFormation.md)
      + [Verifying the Signature of the CloudWatch Agent Package](verify-CloudWatch-Agent-Package-Signature.md)
   + [Create the CloudWatch Agent Configuration File](create-cloudwatch-agent-configuration-file.md)
      + [Create the CloudWatch Agent Configuration File with the Wizard](create-cloudwatch-agent-configuration-file-wizard.md)
      + [Manually Create or Edit the CloudWatch Agent Configuration File](CloudWatch-Agent-Configuration-File-Details.md)
         + [Collect Process Metrics with the procstat Plugin](CloudWatch-Agent-procstat-process-metrics.md)
         + [Retrieve Custom Metrics with StatsD](CloudWatch-Agent-custom-metrics-statsd.md)
         + [Retrieve Custom Metrics with collectd](CloudWatch-Agent-custom-metrics-collectd.md)
   + [Metrics Collected by the CloudWatch Agent](metrics-collected-by-CloudWatch-agent.md)
   + [Common Scenarios with the CloudWatch Agent](CloudWatch-Agent-common-scenarios.md)
   + [Troubleshooting the CloudWatch Agent](troubleshooting-CloudWatch-Agent.md)
+ [AWS Services That Publish CloudWatch Metrics](aws-services-cloudwatch-metrics.md)
+ [Monitor Applications Using AWS SDK Metrics](CloudWatch-Agent-SDK-Metrics.md)
   + [Metrics and Data Collected by AWS SDK Metrics for Enterprise Support](metrics-collected-by-SDK-Metrics.md)
   + [Configure the CloudWatch Agent for SDK Metrics](Configure-CloudWatch-Agent-SDK-Metrics.md)
   + [Set IAM Permissions for SDK Metrics](Set-IAM-Permissions-For-SDK-Metrics.md)
+ [CloudWatch Tutorials](CloudWatch-tutorials.md)
   + [Scenario: Monitor Your Estimated Charges Using CloudWatch](gs_monitor_estimated_charges_with_cloudwatch.md)
   + [Scenario: Publish Metrics to CloudWatch](PublishMetrics.md)
+ [Using CloudWatch with Interface VPC Endpoints](cloudwatch-and-interface-VPC.md)
+ [Authentication and Access Control for Amazon CloudWatch](auth-and-access-control-cw.md)
   + [CloudWatch Dashboard Permissions Update](dashboard-permissions-update.md)
   + [Overview of Managing Access Permissions to Your CloudWatch Resources](iam-access-control-overview-cw.md)
   + [Using Identity-Based Policies (IAM Policies) for CloudWatch](iam-identity-based-access-control-cw.md)
   + [Using Service-Linked Roles for CloudWatch Alarms](using-service-linked-roles.md)
   + [Amazon CloudWatch Permissions Reference](permissions-reference-cw.md)
+ [Logging Amazon CloudWatch API Calls with AWS CloudTrail](logging_cw_api_calls.md)
+ [CloudWatch Limits](cloudwatch_limits.md)
+ [Document History](DocumentHistory.md)