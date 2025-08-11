---
title : "Setup batch AWS into Project"
date : "2024-01-01"
weight : 4 
chapter : false
pre : " <b> 4. </b> "
---

#### BATCH AWS TO OPTIMIZE
![31](/workshop/images/aws/1.31.png)
- Create a new permission role 
- Search **Batch** and create a batch on AWS
![32](/workshop/images/aws/1.32.png)
 {{% notice info %}}
   {
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Action": [
                "sts:AssumeRole"
            ],
            "Principal": {
                "Service": [
                    "batch.amazonaws.com"
                ]
            }
        }
    ]
}
{{% /notice %}}
![33](/workshop/images/aws/1.33.png)
- After that move to **AWS BATCH** and create a new batch
- Create a Job queue
- Configure **BATCH**
![34](/workshop/images/aws/1.34.png)
![35](/workshop/images/aws/1.35.png)
![36](/workshop/images/aws/1.36.png)
![37](/workshop/images/aws/1.37.png)
![38](/workshop/images/aws/1.38.png)
![39](/workshop/images/aws/1.39.png)
![40](/workshop/images/aws/1.40.png)
- When you done it will show you a dashboard
- This batch keep you testing all datas you added and it shows you the percentage of the data when input
- This is a demo when you input data into BATCH
![41](/workshop/images/aws/1.40.png)
![42](/workshop/images/aws/1.40.png)
![43](/workshop/images/aws/1.40.png)
![44](/workshop/images/aws/1.40.png)
![45](/workshop/images/aws/1.40.png)
