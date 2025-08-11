---
title : "Getting support for Account Authentication"
date : "2024-01-01"
weight : 5
chapter : false
pre : " <b> 5. </b> "
---
#### CLEAN RESOURCES
- 1.Terminate EC2 instance:
    - Go to EC2 Management Console
    - On the left navigation bar, select Intances
    - Select all relevant EC2 Instances.
    - Click Actions.
    - Click Manage Instance State.
    - Select Terminate.
    - Click Change State
- 2.Delete S3 Bucket    
    - Go to AWS S3.
    - In the Bucket name list, select the relevant bucket.
    - Select Empty.
    - On the Empty bucket page, confirm and select Empty.
    - Select Delete bucket
- 3.Delete Cloudfront Distribution
    - Go to Cloudfront Management Console
    - On the left navigation bar, select Distribution
    - Select the relevant Distribution.
    - Select Delete
- 4.Delete Launch Template:
    - Go to EC2 Management Console
    - On the left navigation bar, select Launch Templates
    - Select the relevant Launch Template.
    - Click Actions.
    - Click Delete template
    - Type delete in the blank box and press delete
- 5.Delete Batch
    - Go to Batch 
    - On the left navigation bar, select Dashboard
    - On the left navigation bar, select Job queue overview
    - Select the relevant Jobs
    - Click Delete on the right side