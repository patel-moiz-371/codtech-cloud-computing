# Task 2: Cloud Monitoring and Alerts

## Project Overview
This project focuses on setting up automated cloud infrastructure monitoring and alert systems using Amazon Web Services (AWS) CloudWatch. 

## Implementation Steps
1. **Metric Tracking**: Implemented AWS CloudWatch to monitor metrics related to the Cloud Storage infrastructure deployed in Task 1.
2. **Alarm Configuration**: Created a metric alarm (`S3-Bucket-Size-Alarm`) configured to watch the `BucketSizeBytes` metric. The threshold triggers immediately if data footprints change.
3. **Notification System**: Configured an Amazon SNS (Simple Notification Service) topic integrated with an email endpoint. The alert state automatically routes a critical notification message to the administrator's email.
4. **Dashboard Deployment**: Created a visual metrics dashboard (`S3-Storage-Dashboard`) featuring line graph widgets to display infrastructure resource trends.

## Deliverables
- **Screenshots**: Located in the `/screenshots` directory, showcasing the live metric dashboard and the configured active alarm.
